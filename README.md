# Unix info

## System directories

* /bin - binary, executable files located here, available to all users
* /dev - device, all hardware device drivers
* /etc - etcetera,
  * configuration tables (cron, fstab, etc)
  * running configurations
  * config files
  * access / deny tables
  * others
* /lib - libraries, for compilers and such

## Shell concepts

* input redirection - `command < input-file`
  * memory trick- less than looks like a funnel, liquid goes in wide end to the
narrow end, data always flows to where it's pointed

* output redirection - `command > output-file`
  * Warning, this will overwrite the existing file

* output redirection with append - `command >> output-file`
  * if file doesn't exist it will be created

* TIP: input and output can happen simultaneously
  * command < input-file > output-file

* character tricks
  * wildcards
    * `?` - any 1 character
    * `*` - zero or more characters
    * `[a-z]` - brackets can be used to specify chars or a range

* Jobs - all current jobs
  * jobs command shows all current jobs
  * jobs exist in either foreground or background
  * bg - background
  * fg [n]- bring job with pid n to foreground
  
## Notable Commands

* cat - catenate, write each files contents to the screen

* cd - change directory, moving around

* chmod - change mode, used to change access permissions
  * can be expressed numerically if you consider the binary for each group
111-101-011 would be chmod 753 filename. 7 is full access, 5 is read and
execute, 3 is read and write.

* cp - copy a file or directory `cp <item> <destination>`

* grep - file pattern searcher
  * grep string file - search for a string in file
  * grep -l string files - list file names that contain string

* mkdir - make directory
  * -p make intermediary directories as needed

* mv - move files, rename files
  * mv <original> <destination>

* passwd - change your password

* ps - process status

* pwd - print working directory

* rm - remove file

* rmdir - remove empty directory

* tail - display last 10 lines (default) of a file, useful for watching a log

* tr - translate characters
  * `tr a b file` - in file, change every a to b

* wc - word count

* whatis - what is <command>

* who - who is logged in

* xset - user preferences for x org
  * b option for beep, `xset b off` turns off system beep


## File access

Basic permissions are (r)ead, (w)rite, and e(x)ecute. File access falls into
groups: (u)ser, (g)roup, and (o)ther.

Using the `ls -l` command you can view access listings such as `rwxr-xr-x`  
the 1st items are for the user, 2nd are for group, and 3rd is other.

## Acronym helper
*
