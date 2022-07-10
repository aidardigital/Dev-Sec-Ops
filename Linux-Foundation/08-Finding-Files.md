Here we learn Finding Files and Directories Theory

# Most Important Commands We Will Use :

find - find Command

find / -name t.txt - find the t.txt file inside the "/" (root Directory) which means all the system

find . -name t.txt - find the t.txt file inside the "." (Current Directory)

find . -name t.txt -ls - find the t.txt file inside the "." (Current Directory) and list this file as well

find . -name t.txt -exec ls -l {} \; - find the t.txt file inside the "." (Current Directory) and execute command (ls)

find / -iname t.txt - same as -name but with ignore the case

locate t.txt - faster than find to locate t.txt fine inside the whole system

updatedb - to update the data base cache for the locate command
