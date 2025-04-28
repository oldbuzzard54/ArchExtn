THIS IS THE ARCHEXTN V1.2.2 INSTALL PACKAGE ISSUED APRIL 22,2025

=====> APPLIES TO MVS SYSTEMS WHICH ARE NOT TK5 UPDATE 4 OR LATER <=====

This is a complete replacement of ARCHEXTN v1.x.x as well as an
install for ARCHEXTN v1.2.2.

OTHER REQUIRED SOFTWARE:
    ARCHIVER 6.1.8 or later
    unzip utility

Since there are possible so many variation of TK3, TK4, early TK5
as well as "home rolled" MVS systems, I can only supply suggestions
on how to install


INSTRUCTIONS:
1)  You already downloaded your.download.zip to your pc since this
    file is part of it!  extract all the members from this .zip.
    You should see the following 6 files:
        $README.txt
        $README1.txt
        $README2.txt
        RESTOTHR.txt
        ARCHEXTN.ZIP
        ARCHEXTN.pdf

2)  Create a dataset on your MVS such as 'HERC01.ARCHEXTN.ZIP' with
    DCB=(RECFM=V,LRECL=15046,BLKSIZE=15050).

3)  Create a dataset on your MVS such as 'HERC01.RESTOTHR.CNTL' with
    DCB=(RECFM=FB,LRECL=80,BLKSIZE=3120).

4)  BINARY transfer ARCHEXTN.zip from the pc to mvs dataset created
    in step 2.

5)  TEXT transfer RESTOTHR.txt from the pc to mvs dataset created
    in step 3.

6)  On TSO, edit the RESTOTHR.CNTL, make changes as indicated and
    then submit the job.
    This will delete the old version of ARCHEXTN and install the new
    version.

7)  That is it.  All done!
