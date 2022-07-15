### history
```shell
history

history | grep "docker run"
```

### grep
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
refer[1]: https://phoenixnap.com/kb/grep-command-linux-unix-examples

## References
[1] grep: https://phoenixnap.com/kb/grep-command-linux-unix-examples
