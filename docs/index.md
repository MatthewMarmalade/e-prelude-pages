# Inf1A-FP Haskell Installation

## 1. Installing Haskell
You may already have Haskell! That's excellent, you can skip right down to Step 2, installing EPrelude. To check, open a terminal and type "`ghci --version`" to see if you have "`ghci`" already installed on your computer. If not, install by following the link below and picking the **correct version** for your OS (Windows, OS X for Mac, Linux). Choose the **minimal installation**.  
[https://www.haskell.org/downloads#minimal](https://www.haskell.org/downloads#minimal)  
After following those instructions, congratulations! You have Haskell.

## 2. Installing EPrelude
With Haskell installed, you'll have a copy of Prelude, which is Haskell's standard library of useful functions. However, though Prelude is powerful, it is also complex. EPrelude is an alternative version of Prelude, containing simple and straightforward definitions of the standard functions with a restricted set of available types. It also automatically pretty-prints data structures, making it easier to read command-line output.

### Mac (OS X)/(UNIX) Instructions:
To install EPrelude, follow the link below to get the zip file.  
[EPrelude](https://github.com/MatthewMarmalade/e-prelude/archive/main.zip)  
You should download a file named `e-prelude-master.zip`. Unzip this file, and navigate a terminal to the `e-prelude-main` folder (likely within your Downloads folder). At the terminal, within the folder, run the command below:  
`$ sudo ./install.sh` *(This command will require root access.)*  
If it succeeded without any errors, you should be done! As a test, run the following command from a new terminal:  
`$ edhci`  
It should open up an interactive REPL with EPrelude loaded. Feel free to delete the `e-prelude-master` and `.zip` file. However, if you ever want to uninstall EPrelude, you can navigate to the same file (or re-download it if you've deleted it) and run the command below:  
`$ sudo ./uninstall.sh` *(This command will require root access.)*  
*-Note: Linux (and specifically DICE machine) hasn't been tested, nor has Windows with cygwn, though as the scripts are all UNIX-based there shouldn't be intractable difficulties -MM 14 Feb 2021*
#### Updating EPrelude:
To update EPrelude, download the newest version from the link above, follow the instructions for uninstalling and then reinstall.

## 3. Installing Required Packages
Several Tutorials will require the use of additional Haskell packages. These packages are QuickCheck, for automatically checking your functions for errors in all Tutorials, and HTTP, for accessing webpages in Tutorial 4.
*-Note: Intentionally incomplete for the moment. -MM 16 Feb 2021*
<!---
### Cabal
Cabal is a package manager for Haskell. It is probably the most straightforward method, but students have had problems with it before. If there any issues, consider the alternative methods. To install the Haskell packages we need, run the commands below from a terminal:  
`$ cabal update`  
`$ cabal install QuickCheck`
`$ cabal install HTTP`
-
### Stack - Awaits Analysis
Stack is a general workspace/project manager for Haskell that is also capable of managing packages and dependencies of projects. Its usage is more complicated, though it may be more reliable than cabal.
-
*-Note: In progress -MM 14 Feb 2021*
-
### Direct Dependency Download - Awaits Analysis
If the above truly aren't working, here is a way to directly download the modules in question so you can complete the tutorials. In general, the files you download will need to be placed in the same file as your tutorial file to be successfully imported.
-
*-Note: Potential option; has yet to be fully explored. -MM 14 Feb 2021*
-->
