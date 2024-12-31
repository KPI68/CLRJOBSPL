# CLRJOBSPL
Clear Job Spooled File on IBM i

This utility provide a CLI to clear all spooled file a job has generated so far.

## Install
Once the package is cloned as a IFS folder under the user's home (~), or downloaded in zip then transmitted into an IFS folder, we are ready. For example, my home repo  /home/KPI68/CLRJOBSPL will be the [SOURCE_DIRECTORY].

```
cd [SOURCE_DIRECTORY]
sh setup.sh [TARGET_LIBRARY]
```
For example, sh setup.sh KPI681 will set the source physical file CLRJOBSPL in library KPI681. Obviously, the file CLRJOBSPL should NOT pre-exist in KPI681 or else the step fails.

Next use option 14 to compile INSTALLP from the source member. Then
```
call installp
```
The [TARGET_LIBRARY], where the command CLRJOBSPL will reside, obviously should be in the *LIBL. "CLRJOBSPL utility successfully installed." will show.



