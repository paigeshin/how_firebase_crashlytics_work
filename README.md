# how_firebase_crashlytics_work

https://stackoverflow.com/questions/48638964/firebase-crashlytics-custom-log-does-not-appear-in-the-console

The logging mechanism of Crashlytics isn't built for normal logging.

The logs that you put will show in crash reports, not as stand alone logs. Same goes for the user identifier information.

Try forcing a crash, you should see the logs captured before the crash in the crash report. If you want normal logging, you should look into Firebase analytics, it'll help you keep track of regular events and other analytics data.
