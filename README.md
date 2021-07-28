# AIX-lspwdage


[![LinkedIn][linkedin-shield]][linkedin-url]




<!-- ABOUT THE PROJECT -->
## About The Project

This script is used to generate a report on the `lastupdate` field in the `/etc/security/passwd` file for all users. 

You can choose to exclude system users (if you maintain a list of them) from both the report.


The `files` folder contains both the script and the man page.



### Built With

* ksh93 (KornShell) for AIX (UNIX).



### Prerequisites

If you wish to exclude system users, you must place a list of them somewhere on the system and add the path to the script (line 3) and preferably to the man page (line 71).

### Flags

This script will run as normal if it is run without any flags *unless* you maintain a list of system users. If you maintain a list of system users and do not specify a flag, you will be asked if you want to include them in the report.

The `-h` flag will display the help file (the man page).

The `-i` flag is used to `include` system users in the report. If you use this flag and do not have a list of system users, you will get the following error:
*"No system user list found, please see the man page."*

The `-e` flag is used to `exclude` system users from the report. If you use this flag and do not have a list of system users, you will get the following error:
*"No system user list found, please see the man page."*


### Usage

This script, although it will run fine in the terminal, 
is designed to be saved to a file.

	lspwdage -e > /home/phil/pwdage_report


 
## Contact

Phil Huxford - [![LinkedIn][linkedin-shield]][linkedin-url]

Project Link: [https://github.com/phil-huxford/AIX-lspwdage](https://github.com/phil-huxford/AIX-lspwdage)


[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/phillip-huxford/
