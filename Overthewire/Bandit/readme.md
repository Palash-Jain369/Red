## [Detailed Guide](https://palash-jain369.github.io/posts/bandit/)

### Bandit wargame will let players experience following concepts:
- Workin with Command Line Interaface
- Navigate Linux File System: Finding a file, searching files, File Permissions, etc.
- Sockets, SSH,  Netcat, Port Scanners, TLS, etc.
- Encoding/Decoding, Encryption, Cryptography, Brute Forcing etc.
- Bash Scripting, Enviornment Variables, Running Subshell, Vim
- Git: Navigating branches and finding exploits.

QUick Commands(passwords may be deprecated)

level 0 - connect to server via ssh.
          - ssh -l bandit0 -p 2220  bandit.labs.overthewire.org(-l = login name)


Key to level 1 - NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL.  cat

Key to level 2 - rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi. standard input---> cat ./-

Key to level 3 - aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG.  cat 'file name'

Key to level 4 - 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe. ls -al

Key to level 5 - lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR. file ./* | grep ASCII

Key to level 6 -  P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU. find -size 1033c \! -executable.

Key to level 7 - z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S. find -user bandit7 -group bandit6 -size 33c 2>/dev/null| xargs(converting output to argument for next command) cat                 

Key to level 8 - TESKZC0XvTetK0S9xNwm25STk5iWrBvP. cat file | grep millionth.

Key to level 9 - EN632PlfYiZbn3PhVK3XOGSlNInNE00t. sort data.txt | uniq -u 

Key to level 10 - G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s. strings | grep =

Key to level 11 - 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM. base64 -d data.text

Key to level 12 - JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv. googled rot13 translator.

Key to level 13 - wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw. worst one - check type of compression with file command --> gunzip/bzcat/tar unzip ---> repeat.

Levl 14 - ssh on the same port with -i privatekey to login as bandit14 

Key to level 15 - jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt. nc(netcat) localhost 30000(port) ---> submit level 14 key 

Key to level 16 - JQttfApK4SeyHwDlI9SXGR50qclOAil1. nc --ssl/openssl s_client bandits.labs...:300001----> submit lvl 15 pass

Key to level 17 - nmap -A(all) -p '31000-32000'. ---> obtain private key ---> store in a file ---> ssh -p 2220 -i privatekey.ssh -l bandid17 bandit.labs.overthewire.org
 
Key to level 18 - hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg. diff file1 file2 ----> grep output in file1.

Key to level 19 - awhqfNnAbc1naukrpqDYcF95h7HoMTrC. ssh ssh://bandit18@....:2220 cat ./readme

Key to level 20 - VxCazJaVykI6W36BkBU0mJTCM8rR95XT. setuid-bandit20 user executables allowing to run a command with a specified elevated permissions.

Key to level 21 - NvEJF7oVjkddltPSrdKEFOllh9V1IBcq. nc -l [port] ----> connect to [port] from other machine/terminal-----> provide lvl20 password from server side terminal.

Key to level 22 - WdDozAdTM2z9DiFEQ2mGlwngMfj4EZff. running the cron script then catting the file.

Key to level 23 - QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G. changing variable in bash, so that script uses bandit23 instead of bandit22

Key to level 24 - VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar. Making a script to cat out password into a file name in /tmp/foler. Careful of enabling permissions for both script and /tmp/folder.

Key to level 25 - p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d. for loop[for i in {9999..999}; do echo "pass24 $i"] | nc localhost 30002 | password.

Key to level 26 - shell is set to a script. using a small screen size, enter vim as script executing 'more'. set shell to bash(:set shell=/bin/bash then run shell all inside vim). Some googling for this one.

Key to level 27 - YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS.

Key to level 28 - AVanL161y9rsbcJIsFHuw35rjaOM19nR. Git clone address with localhost:2220/home...

Key to level 29 - tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S. git log ---> git show

Key to level 30 - xbhV3HpNGlTIdnjUrdAlPzc2L6y9EOnS. git branch -a (showing remote branches). git swtich 'remote branch'.

Key to level 31 - OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt. explore .git folder.

Key to level 32 - rmCBvG56y58BXzv98yZGdO7ATVL5dW8y. git add -f(forcing over .gitignore) key.text---> git commit ----> git push.

Key to level 33 - odHo63fHiFqcWWJG9rLiLDtPm45KzUKy. script is running as a shell, giving the input in all caps to BOURNE SHELL. we can see that $1 is the command we type, and sh before that, so sh is $0 in this script, so $1 passes BOURNE SHELL to BOURNE SHELL, allowing us to enter the shell on top of running shell script. When we exit BOURNE SHELL, we return back to UPPERCASE SHELL as a proof.











 







