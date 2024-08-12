# ArchExtn V1 R2 M0 Patch 1
Utility Programs to extend Archiver Files For MVS 3.8j

Module ARCHRST has a bug that looks for a specific dataset name.  ARCHRST will
run but produce strange results if it does not fail.  This is a patch to
correct this problem.

Only 1 line of the PLI source was changed.  If you want to apply the fix to the
source, find the line with "VSAM1DSN=HERC01.SLIMVER.ARCHIVE" and change it 
to "VSAM1DD=ARCHIVE".

The patch is in:
       
    ArchExten-PATCH01.xmi 
    RESTK5P1.txt  - installs the patch to a TK5 system or systems with NJE38 
                    installed.


