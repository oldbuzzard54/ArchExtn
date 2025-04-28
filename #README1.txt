THIS IS THE ARCHEXTN V1.2.2 INSTALL PACKAGE ISSUED APRIL 22,2025

 ======> THESE INSTRUCTION APPLY TO TK5 UPDATE 4 OR LATER ONLY <======

This is a complete replacement of ARCHEXTN V1.x.x as well as an
install for ARCHEXTN V1.2.2.

OTHER REQUIRED SOFTWARE:
    UNZIP program

INSTRUCTIONS:
1)  you already downloaded your.download.ZIP to your pc since this
    file is part of it!  extract all the members from this .ZIP.
    You should have the following 6 files:
        $README.txt
        $README1.txt
        $README2.txt
        RESTOTHR.txt
        ARCHEXTN.ZIP
        ARCHEXTE.pdf

2)  Create a dataset on your TK5 system 'TK5.ED-LISS.ARCHEXTN.ZIP'
    DCB=(RECFM=V,LRECL=15046,BLKSIZE=15050) on volume TK5001
    with at least 12 tracks of space.

3)  Binary transfer TK5.ED-LISS.ARCHEXTN.ZIP from the pc to mvs
    dataset created in step 2 ('TK5-ED-LISS-ARCHEXTN.ZIP')

4)  Start RPF and go to option 3.4 - DS List

5)  Find the zip file you just uploaded to and select it with b.

6)  You will be presented with a list of items.  you can edit
    but changes will not be saved.
       $README
       $README1
       $README2
       #README
       #README1
       #README2
       ARCHEXTE
       FINISH
       PDS
       RESTOTHR
       RESTTK5

7)  On this list you will see 3 #READMEs. These are the same as the
    ones on the pc except in ASCII.

8)  Edit member RESTTK5 and make any changes to the JCL.  Submit it.
    This will delete the old version of ARCHEXTN and install the new
    version.

9)  Now it is time to commit ARCHEXTN V1.2.2  Select and edit member
    FINISH.  Submit it to update the TK5 system and clean up.

13) That is it.  All done!
