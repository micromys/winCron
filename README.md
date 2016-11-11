# Currently Under Construction
## crontab.pyc
Crontab for windows

A Windows crontab.pyc program analogue to linux crontab utility

crontab.pyc supports almost all timing-arguments that Linux crontab supports, like:
* * for every every minute,hour,month,day of month,day of week
* comma (,) seperated arguments like 11,12,13 for 11th,12th,13th (minute,hour,mon,dom)
* hyphen (-) seperated arguments to specify a range like 12-16 for running jobs between 12:00 and 16:59
* empty lines or lines starting with # are ignored
* **@yearly, @daily, @hourly** are supported but internally converted to 0 0 1 1 *,0 0 * * *,0 * * * *
* @reboot (run at startup) is currently not supported

## Sample crontab.txt

**see crontab.txt**

## Install crontab.pyc (compiled from crontab.py)

* download crontab.pyc
* create crontab.txt or download crontab.txt and adapt it

## Running crontab.pyc

* Open CMD box
* [python path]python.exe [path]crontab.pyc [[path]crontab.txt [[path]crontab.log [[path]crontab.pid]]]
* all files are supposed to be in the same folder
* create shortcut on your desktop with: 
  * target: C:\Python27\python.exe crontab.pyc crontab.txt crontab.log crontab.pid
  * start in: "C:\Users\your name\Desktop"
  * Run: Minimised
  * optionally you can put the shortcut in the startup folder (C:\Users\yourname\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup) to start crontab.py on startup

The defaults filenames are crontab.txt,crontab.log,crontab.pid

## Start crontab.pyc using Windows Task Scheduler

* download crontab.xml
* edit to change "yourname" and "yourpath"
* Open CMD box
* schtasks /Create /TN winCron /XML crontab.xml

### Under construction

## Running crontab.pyc as a Service

### Under construction

