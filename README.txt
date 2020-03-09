This repository is designed to allow MacOS users to run GEOCHEM-EZ.

To use, make sure you have Docker and java installed then run `java -jar GeoChem-EZ.jar`

See below for original GEOCHEM-EZ documentation.


/*******************************************************
*		GEOCHEM-EZ README		       *
*						       *
*		USDA-ARS, 2008                         *
*	Ben  Schultz, Jon Shaff & Eric Craft           *
*                                                      *
********************************************************/
 -------------------------------------------------------
|		Installing GeoChem-EZ			|
 -------------------------------------------------------

Install GeoChemEZ by copying the contents of this zip file
into your home directory: 

cd $HOME 
unzip Geo3D.zip 

 -------------------------------------------------------
|		Running GeoChem-EZ			|
 -------------------------------------------------------

To launch GeoChem-EZ simply type:

java -jar GeoChemEz.jar 

GeoChem requites Java SE6 or higher, which is available for down- load
from Sun Microsystems


 ------------------------------------------------------
|		Using GeoChem-EZ		       |
 ------------------------------------------------------

To get a feel for how EZ works, it's best to take a look
at the help. To get there run EZ, then go to help>launch
help and our guide should launch  in your browser. If you
are a seasoned GEOCHEM-PC user, you can simply load your
old dat files and get to work.

 ------------------------------------------------------
|		Critical Files			       |
 ------------------------------------------------------

As expected, if the files within GeoChem's directory are 
tampered with, GeoChem-EZ may crash. The files you may see
in this directory and not touch are:

1) georun

This contains is the executable for GEOCHEM-PC, which is
run by GeoChem-EZ. 

2) GEOCHEM.CFG

This is used by georun and is written anew every run
by GeoChem-EZ.

3) interface.cfg

This file saves all the databases the user selects, along
with their default work directory and template. If this is
deleted, GeoChem-EZ will revert to a default configuration
and generate new file

4) GeoChemEZ.jar

This contains all the precompiled Java files to run GeoChem-EZ.

5)metlig.MLW

An exception to the do not touch rule, this a database which
stores the molecular weights of all the metals and ligands 
in the GEODAT-A.LIG database. If you expand on this database
and wish to use g/L and mg/L in GeoChem-EZ, you can edit this
database with any ASCII editor. The format is simply <m/l>
<code#><molecular weight>.

6)Resources Directory

This directory contains the default SALTS and LIG databases
as well as the entire help system and some images used by EZ.
All content in this directory should be accessed only through
GeoChem-EZ

7)MyData Directory

Default directory to store all of the users *.geo files. Upon
installation, it contains examples from GEOCHEM-PC in DAT and
GEO formats.

There are also a number of temporary files with EZ in its run of
GEOCHEM-PC. Destroy these at will.


 ------------------------------------------------------
|		Error Reporting			       |
 ------------------------------------------------------

If you find bugs or are experiencing glitches, please
report them to <insert email here>


