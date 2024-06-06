gptsync
=======

Here's an OSX port and enhancement i made to help creating hybrid MBR partitions on GPT drive.

Code came from project rEFit: http://refit.sourceforge.net/

Usage: gptsync [OPTION]... DEVICE [PARTITION[+/-[TYPE]]] ...

gptsync fill hybrid MBR of GPT drive DEVICE.

Specified partitions will be a part of hybrid MBR. Up to 3 partitions are allowed.
+ means that partition is active (only one partition can be active).
TYPE is an MBR hexadecimal type (use -t option to list recognized types).

Valid options:
  -e, --empty             create an MBR containing only the EFI Protective partition
  -n, --nofill            don't try to protect unused partition
  -t, --types             list the MBR recognized type codes
  -h, --help              display this message and exit
  -V, --version           print version information and exit
