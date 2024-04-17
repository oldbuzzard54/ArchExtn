# ArchExtn V1 R0 M0
Utility Programs to extend Archiver Files For MVS 3.8j
Welcome to Archiver Extentions.  This is a group of programs designed
to provide additional feature for users of Archiver.  The full use of
ARCHIVER is out of scope of this document.  Archiver 6.1.5 is
pre-installed on TK5 systems.  TK5 systems include a copy of the user
guide is the DOC folder.  It is also can be found at cbttape.org
File # 147 ARCHIVER All your non-VSAM datasets to 1 VSAM file .

Archive is a program designed for storage of almost any type of
non-VSAM file.  The file is stored in a VSAM KSDS (Keyed Sequential
Data Set) in a compressed and encrypted format.  One possible use of
Archiver is for secured storage of production source code.

The collection (so far) consists of PL/I programs to:
     ARCHDIR -  Produces directory listings sorted in user selected
                sequences
     ARCHCOMP - Compares the indecies of two Archiver clusters to
                highlight differences
     ARCHUTIL - Unloads/Loads an Archive cluster to/from files
                suitable for transmission

This repository of the Archiver extensions is distributed as a 3 files.

    ArchExten-V1R0M0.xmi
    RESTTK5.txt  - restore to a TK5 system or systems with NJE38 installed.
    RESTOTHR.txt - restore to a system without NJE38 installed (uses RECV370).

    RESTZOS.txt - experimental restore to a Z/OS system.  Restores only
                  files to execute Z/OS plus PL/1 (F) runtime.  Tested on
                  Z/OS 2.05.  All code is the same 24 bit code as run
                  on TK5.

Select the appropriate REST file for you system.

The RESTxxxx JCL defaults the user id to HERC01 and the volume to create
the datasets is TSO002.  You man need to change these before you submit.
Be sure to remove the TYPRUN before you submit the RESTxxxx.txt.

Option: Submit the job in the .CNTL(CLEANUP) to install the program and
procs into the system libraries.
