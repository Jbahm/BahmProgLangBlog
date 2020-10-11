# Using BNFC on windows
Similar to when I tried to install Haskell for the first time, I ran into enormous amounts of difficulty, spending hours trying various methods to run bnfc successfully on my machine
 After a while though, I found a solution that worked, and I wanted to share that solution to save others some trouble

## The workaround
I realized the biggest issue with installing bnfc was purely the fact that I was on windows, the program did not seem designed to be easily used on windows, but more targeted at UNIX based
systems like Mac and Linux. To solve this issue, I set up a linux container on my machine using a program called [Docker](https://www.docker.com/)  
For those unfamiliar with the program, Docker essentially allows you to run a light-weight virtual machine of sorts in a command-prompt window on your computer!

## Setting up Docker
After downloading the windows exectuable, you will have access to the docker commands, however right now they are useless as you need to install and set up what is called a "Container".
To find a container, you simply go to [Docker Hub](hub.docker.com) and that will give you a list of availible images to use for it. In my case, I needed a linux based container, so I found a simple container running [Ubuntu](https://hub.docker.com/_/ubuntu).  
To install images/create the container, you simply need to run the command that is specified on the docker hub page of your image. 
In the case of the Ubuntu one I used, you need to open up a new command prompt window and run `docker pull ubuntu`  
Following the command being run, you need to go follow the guide on screen to set up your container.  

## Using your container
Once the container has been set up, you have to open a new command prompt window and run the following commands  
`docker start <container name>`  
`docker attach <container name>`  
After those commands have been run, you are now operating in the home directory of your docker container, which in this case is a linux environment

## Back to the initial problem
Now that we have a functional linux environment, installing BNFC and the other compilers necessary to assemble a context free grammar is extremly simple
In your docker container, you need the following commmands(in this order):  
`cabal-install` which will install the cabal package manager system(needed to install the compilers)  
`brew install bnfc` will install the bnfc compiler system  
`cabal install alex` will install the alex compiler system
`cabal install happy` will install the Happy compiler system  


## Testing BNFC
Once the 3 of those are installed, you should be able to compile a context free grammar!  
Navigate to the directory of the grammar in your docker container, and then from there you can run
`bnfc -m --haskell <filename>`
If the file compiles successfully, congrats, you have properly installed BNFC!
