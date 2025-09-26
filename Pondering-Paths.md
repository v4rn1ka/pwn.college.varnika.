# 1. The Root
This challenge asks me to invoke the pwn program using its absolute path.

## My Solve
**Flag:** 'pwn.college{k3eO3Lwjp4-8iPj6rsNHdGR_mEx.QX4cTO0wiN2AzNzEzW}'

I typed the absolute path of pwn i.e. /pwn and recieved my flag.

## What I learned
I learnt that a program can be invoked by providing its path on the command line and also that the path that begins with the root directory(/) is the absolute path. So here, /pwn is the absolute path of the program pwn.

## References
Video in pwn.college



# 2. Program and Absolute Paths
This challenge asks me execute the file run which is inside the challenge directory.

## My Solve
**Flag:** 'pwn.college{c4v3WNrsAI-SuuNTV6ToxV6E5T8.QX1QTN0wiN2AzNzEzW}'

Here, I first provided the outer most directory which is the challenge directory. Next, I provided the file required that is run. So, the entire path to run program is:
/challenge/run

## What I learned
I learnt to write the path of a program which is present within a directory.

## References
Video in pwn.college



# 3. Position thy self
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



# 4. Position Elsewhere
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



# 5. Position Yet Elsewhere
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



# 6. Implict Relative Paths, from /
This challenge asks me to run /challenge/run using a relative path while having a current working directory of /.

## My Solve
**Flag:** 'pwn.college{0MGED8DxHrxyVJW9JaY0UfHjbrz.QXwUTN0wiN2AzNzEzW}'

Since it is mentioned that the cwd is the root directory, the implicit relative path would be the rest of it i.e. challenge/run. First, I changed the directory to the root directory and then I gave the relative path and got my flag.
Commands: cd /
          challenge/run

## What I Learned
I learned how relative paths are dependent on the current working directory and that implicit relative path need not mention the current working directory. 

## References
Video and slides in pwn.college



# 7. Explicit Relative Paths, from /
This challenge asks me to use '.' in the relative path to run /challege/run

## My Solve
**Flag:** 'pwn.college{0MGED8DxHrxyVJW9JaY0UfHjbrz.QXwUTN0wiN2AzNzEzW}'

First, I changed the directory to the root directory. Then, the explicit relative path would be ./challenge/run. Here, '.' implies that the rest of the path relates to the current working directory that is the root directory in this case.
Commands: cd /
          ./challenge/run

## What I learned
The only difference between implicit and explicit relative directories is that in implicit it is assumed that the path relates to the cwd while in explicit it is necessary to mention its source using '.' (signifying current directory) or '..' (signifying the directory that the cwd lives in). 

## References
Video and slides in pwn.college



# 8. Implicit Relative Path
This challenge asks me to explicitly execute a program in the current directory, using '.'.

## My Solve
**Flag:** 'pwn.college{4Y3h5O4kI7IB40tLnhOg3Q4Ml_0.QXxUTN0wiN2AzNzEzW}'

Initially I changed the directory to /challenge and then explicitely run the run program with ./run.
Commands: cd /challenge --> for changing the cwd to challenge
          ./run --> (.) implying to run it from the cwd

## What I learned
Using naked path could be unsafe as it might accidentally execute programs from the current directory which have the same name as the core system utilities. Using '.' makes it much safer.

## References
Pre-text from the challenge, slides in pwn.college.



# 9. Home Sweet Home
This challenge ask me to specify a file within /challenge/run as an argument on the commandline with the constraints: 
i.Argument must be an absolute path
ii. The path must be inside the home directory
iii. Before expansion, argument must be 3 characters or less.

## My Solve
**Flag:** 'pwn.college{0BWgfnJsusJif4iIn-CJXK0xzAg.QXzMDO0wiN2AzNzEzW}'

Considering the first 2 constraints, I came to the conclusion that the arguement must begin with ~/. Here, ~ is the home directory. These add up to 2 characters, which means I can add only one more character. Let that be v. This completes my argument (~/v). 
Commands: /challenge/run ~/v

## What I learned
` is the home directory which expands to /home/hacker.

## References
Pre text from the challenge.
