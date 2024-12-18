This is a working fork of ELIOT's NIKA that works with Igor Pro 8.0.4.2 

To compare which files I've changed have a look at [this comparison](https://github.com/EliotGann/Eliots-NIKA/compare/master...mattgebert:Eliots-NIKA:master). 

Note: I've run into troubles, because files like CCDPlotting.ipf use symbols such as Å which change character codes in different encodings. 
To view these files in an editor like VSCode, you should use `Windows1252` encoding, instead of `UFT-8`.

-----------------------------------------------------------
### Matt's Simplified Instructions for Installation

I've included the XMLutils into this repository, so you don't need to download it yourself.

1. Clone this repository to a local directory (i.e. use [git](https://git-scm.com/) via cmd, or [github desktop](https://github.com/apps/desktop) GUI)

        git clone https://github.com/mattgebert/

2. Open Igor Pro 8.04 64-bit
3. Open the menu options:
    
    `Help` > `Show Igor Pro User Files`

4. Create shortcuts from the `Igor User Files` folders to the cloned local directory subfolders.

        User Procedures
        |- Shorcut1 ->  NISTRSoXSNIKA_Users
        
        Igor Procedures
        |- Shorcut2 -> NISTRSoXSNIKA_Igor

        Igor Extensions (64-bit)
        |- Shorcut3 -> XMLutils

5. Restart Igor Pro 64-bit.
6. If you want to update in the future, you can either pull/fetch changes using git via cmd inside the directory, or via github desktop GUI.

        git pull

-----------------------------------------------------------

# Eliot's-NIKA
Branch of NIKA which adds custom functionality for RSoXS and GIWAXS based in Igor Pro

developed by Eliot Gann originally at North Carolina State University, then at Monash university, NIST and currently Brookhaven National Lab with the help of many other people (most notably Brian Collins of NCSU and now WSU) contact Eliot Gann (egann@bnl.gov) with any questions.  The NIST RSoXS browser component is the only actively maintained part of the package, but I will probably be able to help with any reasonable requests.

These are a set of useful tools which I have used in my research since 2010, and which I made before I knew how to code properly.  I include the branched NIKA files which have been edited from the original signifigantly, but are still under that license.  Please cite NIKA properly if you use this to analyze any data.  (see https://usaxs.xray.aps.anl.gov/software/nika for how to cite NIKA as well as the much updated current version of NIKA which is  of course NOT compatible with any of these procedures anymore, but has also added some of these features over the years). This is not how software development should happen, so please feel free to make any changes you like to this code, but please just make them available to everyone by creating pull requests on this repository.

If you run into any problems, besides just emailing me, please create an issue in github as well, so others can try their hand at fixing it as well.

Suggested Installation Method:

1.) Clone this repository to your local machine.  (I strongly suggest to download github desktop, which makes this incredibly easy, unless you are a github expert already.  Just paste the repository address in and hit clone)

2.) Find out where the repository is stored on your local computer

3.) open your user files directory (from Igor Pro  select Help-> Igor Pro User Files)
    usually this is in the documents/wavemetrics/ folder
    (close Igor after this step)

4.) create a shortcut (windows) or alias (Mac) of the NISTRSoXSNIKA_Igor directory into the "Igor Procedures" directory

5.) create a shortcut or alias of the NISTRSoXSNIKA_Users directory into the "User Procedures" directory

6.) Install XMLUtils (https://www.wavemetrics.com/project/XMLutils)

7.) Restart Igor Pro, you should see the RSoXS menu appear

8.) to update to the latest version, just go to github desktop and click the fetch origin button when Eliots-NIKA is selected*


*NOTE If upgrading from a pre-Nov 26, 2019 version, re-install is required.  Delete all shortcuts in the NIKA folder and recreate them from the github directory.  They have all changed name to allow simultaneous operation with the modern version of NIKA (THANKS TO PETER BEAUCAGE FOR THIS)
