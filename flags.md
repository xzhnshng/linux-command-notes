## Flag Session
### -c
`-c` flag means execute the following command
```shell
sudo sh -c 'echo "foo" > /home/bar'
```
- `sh` calls the program sh as interpreter and the `-c` flag means execute the following command as interpreted by this program.
- the above command will write the file bar containing the text foo to /home/
- It's important to use 'single quotes' around the command string, otherwise the current shell will try to expand it before it's passed to the interpreter you called.
- refer[1]: https://askubuntu.com/questions/831847/what-is-the-sh-c-command



## References
- refer[1]: https://askubuntu.com/questions/831847/what-is-the-sh-c-command
