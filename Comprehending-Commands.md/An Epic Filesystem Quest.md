# An Epic Filesystem Quest
This challege asks me to fetch my file by following the instructions by the shell using ls, cat and cd.

## My Solve
**Flag:** 'pwn.college{MtzDs1G60U-zq2GZYFFZ7KMZZAP.QX5IDO0wiN2AzNzEzW}'

I used cd to enter into the path provided, ls to list out the files in it and cat to read the. In case, the shell asked me not to use cd and yet find the file, I used ls -a /path to list out the files and cat /path_to_the_file to read it. Using these I found my flag.
```
 cd /
ls
cat TIP

 cd /usr/share/gap/doc/hpc
ls
cat CLUE

 cd /usr/lib/debug/.build-id/16
ls
cat TRACE

 ls -a /opt/linux/linux-5.4/arch/microblaze/kernel/syscalls
cat /opt/linux/linux-5.4/arch/microblaze/kernel/syscalls/SNIPPET-TRAPPED

 ls -a /usr/share/racket/pkgs/htdp-lib/htdp/isl+/lang
cat /usr/share/racket/pkgs/htdp-lib/htdp/isl+/lang/.INSIGHT

 cd /usr/share/zoneinfo/right
ls
cat WHISPER

 cd /usr/local/lib/python3.8/dist-packages/jupyter_server/templates
ls
cat BLUEPRINT

 ls -a /usr/lib/ruby/2.7.0
cat /usr/lib/ruby/2.7.0/.SPOILER

 ls -a /usr/lib/python3/dist-packages/IPython/testing/tests/__pycache__
cat /usr/lib/python3/dist-packages/IPython/testing/tests/__pycache__/DOSSIER-TRAPPED
```

## What I Learned
Familiarised myself with catting and listing files and hidden files as well.

## References
Pretext
