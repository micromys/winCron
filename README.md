# winCron
Crontab for windows

A Windows crontab.py program analogue to linux crontab utility

winCron supports all timing-arguments that Linux crontab supports, like:
* * for every every minute,hour,month,day of month,day of week
* comma (,) seperated arguments like 11,12,13 for 11th,12th,13th (minute,hour,mon,dom)
* hyphen (-) seperated argument to specify a range like 12-16 for running jobs between 12:00 and 16:59
* other arguments are currently not supported

