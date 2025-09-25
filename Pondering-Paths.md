# The Root
This challenge asks me to invoke the pwn program using its absolute path.

## My Solve
**Flag:** 'pwn.college{k3eO3Lwjp4-8iPj6rsNHdGR_mEx.QX4cTO0wiN2AzNzEzW}'

I typed the absolute path of pwn i.e. /pwn and recieved my flag.

## What I learned
I learnt that a program can be invoked by providing its path on the command line and also that the path that begins with the root directory(/) is the absolute path. So here, /pwn is the absolute path of the program pwn.

## References
Video in pwn.college



# Program and Absolute Paths
This challenge asks me execute the file run which is inside the challenge directory.

## My Solve
**Flag:** 'pwn.college{c4v3WNrsAI-SuuNTV6ToxV6E5T8.QX1QTN0wiN2AzNzEzW}'

Here, I first provided the outer most directory which is the challenge directory. Next, I provided the file required that is run. So, the entire path to run program is:
/challenge/run

## What I learned
I learnt to write the path of a program which is present within a directory.

## References
Video in pwn.college



# Position thy self
This challenge asks me to change my directory to the one that is provided and then invoking the path of the run file.

## My Solve
**Flag:** 'pwn.college{U7DDEt89t9vMmrhHN9xEq7LIpz3.QX2QTN0wiN2AzNzEzW}'

First I provided the path of the run file: /challenge/run. Then it mentioned that I had to change the directory to /var. So, I added the command cd /var which changed it to the var directory. After this I could rerun the challenge program and got my flag.
Steps: cd /var
       /challenge/run

## What I Learned
I learnt that the 'cd' command is used to change the'current working directory'. 
The command is give by cd /directory.

## References
Video in pwn.college



# Position Elsewhere
This challenge asks me to change my directory to the one that is provided and then invoking the path of the run file.

## My Solve
**Flag:** 'pwn.college{QiE2ncXzaCm1K6gHDT2t87Knrq8.QX3QTN0wiN2AzNzEzW}'

First I provided the path of the run file: /challenge/run. Then it mentioned that I had to change the directory to /proc/131. So, I added the command cd /proc/131 which changed it to the var directory. After this I could rerun the challenge program and got my flag.
Steps: cd /proc/131
       /challenge/run

## What I Learned
I learnt that the 'cd' command is used to change the'current working directory'. 
The command is give by cd /directory.

## References
Video in pwn.college



# Position Yet Elsewhere
This challenge asks me to change my directory to the one that is provided and then invoking the path of the run file.

## My Solve
**Flag:** 'pwn.college{g8NmAcLOEaS1sm8SLQdFZ25lPCd.QX4QTN0wiN2AzNzEzW}'

First I provided the path of the run file: /challenge/run. Then it mentioned that I had to change the directory to /proc/131. So, I added the command cd /proc/131 which changed it to the var directory. After this I could rerun the challenge program and got my flag.
Steps: cd /proc/131
       /challenge/run

## What I Learned
I learnt that the 'cd' command is used to change the'current working directory'. 
The command is give by cd /directory.

## References
Video in pwn.college



