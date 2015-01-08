pulsetranslator_monitor
--------

This app will listen to both the "raw" and the normalized exchanges and record
basic information from messages in order to correlate them.  The goal is to:

1. ensure each raw message is translated in a timely manner
2. there are no duplicate messages

If a certain time elapses without seeing the associated normalized message, or
if a duplicate is seen, a message is logged and an email is sent.
