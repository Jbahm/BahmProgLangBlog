# Navigating the difficult proccess of installing Haskell on Windows
After spending several hours attempting to get Haskell running on windows, I finally figured out how. I figured my first blog entry should try and save others the same difficulty!


## First Steps
Before we even install Haskell, you need to install a program called [Chocolatey](https://chocolatey.org/)  
Essentially, chocolatey is a program that allows you to do quick installations of other programs set up on their platform  
To install chocolatey, open powershell as an administrator and run the following command:  
`Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))`  

## Setting up Haskell
Once chocolately is installed properly, open up a new powershell window(once again as an administrator) and simply run:  
`choco install haskell-dev`  
Say yes to all the prompts, and once that finishes, haskell will be ready to use!

## Making sure it works
Once the installer finishes open a new command prompt window and run the commands:  
`ghc --version` and `ghci` 
If installed correctly, the console should respond with:  
`The Glorious Glasgow Haskell Compilation System, version 8.10.1` and `GHCi, version 8.10.1: https://www.haskell.org/ghc/ :? for help` respectivley  

Assuming you get the correct response, navigate to the directory where you store your programs  
You should now be able to compile and run haskell programs by using the following commands:  
`ghc <filename>.hs`  
`<filename>`  
Assuming the program runs, then you have successfully installed Haskell!

