# ArchExtn V1 R2 M2
Utility Programs to extend Archiver Files For MVS 3.8j
Welcome to Archiver Extentions.  This is a group of programs designed 
to provide additional feature for users of Archiver.  The full use of 
ARCHIVER is out of scope of this document.  Archiver 6.1.8 is 
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
     ARCHRST  - Reset Version numbers
     ARCHUTIL - Unloads/Loads an Archive cluster to/from files 
                suitable for transmission

There are ASCII readme files (#Readme.txt,#Readme1.txt and #Readme2.txt)
as well as EBCDIC version prefixed with $.  Both are ASCII and
EBCDID version are the same.  These are the official install instructions.