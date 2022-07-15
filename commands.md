### history
```shell
history

history | grep "docker run"
```

### grep
*refer[2]*
```shell
grep searchStringPattern file1

grep searchStringPattern file1 file2 file3

grep searchStringPattern *

# options: -w, -i, -x, -r, ...
```

use `grep` with other command
```shell
# read content of test.sh and use pipe input test.sh content to grep command
cat test.sh | grep -n 'echo'

# get history commands that contains "docker run"
history | grep "docker run"
```


### mkdir
*refers[3]*
```shell
# syntax: mkdir [option] dir_name

# Creates a directory in the current location
mkdir directory_name

# Creates multiple directories in the current location. Do not use spaces inside {}
mkdir {dir1,dir2,dir3,dir4}

# Creates a directory structure with the missing parent directories (if any)
mkdir –p directory/path/newdir
# example:
mkdir -p db/migration


# Creates a directory and sets full read, write, execute permissions for all users
mkdir –m777 directory_name

# To see the details of the mkdir process, use -v to get verification info
mkdir –v directory_name(s)
```


## References
[2] grep: https://phoenixnap.com/kb/grep-command-linux-unix-examples <br/>
[3] mkdir: https://phoenixnap.com/kb/create-directory-linux-mkdir-command <br/>
