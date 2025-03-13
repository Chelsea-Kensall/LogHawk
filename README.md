# LogHawk
Log file scanner created for LHL Project 3
LogHawk 3.3 requires python to run

< What's it do: >

LogHawk is a script based log scanning tool designed to quickly scan logs for threats, errors, and unusual activity.

LogHawk check 4 logs for specific indicators of compromises:

/var/log/apache2.log
/var/log/auth.log
/var/log/kern.log
/var/log/cron.log
These log options may need to be changed according to your system set up, or can be customized via user input at the terminal* (Requires changes in LogHawk script, as detailed in code comments)

Looks for specific indicators:

Counts instances of http codes
Default: 404, 401, 200
Counts the number of times each unique IP has accessed the site
Scans login attempts for:
Authorization Failures
3 failed login attempts
Scans kernal logs for:
ERROR Alerts
CRITICAL Alerts LogHawk will automatically write a summary of these results to a .txt file called LogHawk3.2_(date)-(time) to ensure you always have an easy to read record of log activity.
Optional Customization includes:

 - An additional detailed summary of log lines that indicate errors or suspicious activity.
 - Print the LogHawk results directly to the terminal in addition to the .txt file.


< Updates: >
 - Added Cron Log searching features
 - Minor bug fixes to file closing
 - Default log paths and output file path updated
 - Welcome script updated

**LOGHAWK was created purely as a project and is not intended for or recommended for actual use. Seriously. Don't use it. **
