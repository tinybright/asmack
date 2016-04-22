## Enable DEBUG ##

This is the first thing you should do. Set the DEBUG variables in XMPPConnection/BOSHConnection to true

## Save a logcat session ##

This will contain all the stanzas going over the wire.

`adb logcat | tee connection_trace` is the correct way on linux.

## Remove your credentials ##

Look for `<auth>` packages that contain your credentials. Remove them.

## How to reproduce ##

Try to find a test server where we can tryout the problem, and add the code you are using (for open source project: point to the branch you are using, it's usually easier to do a build than trying to get a snipset bootstraped).