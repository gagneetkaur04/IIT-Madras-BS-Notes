## GrPA 1

**QUESTION:**

We created some directories and change our current working directory using the cd command as given by the sequence of commands below. Write a bash command to make the directory "level2" as your current working directory. i.e. after executing your solution, if we execute the command "pwd" it should return the path of the directory "level2".
Write your solution as a single line bash command.

```
cd /
mkdir level1
cd level1
mkdir level2
cd level2
mkdir level3
cd ..
cd ..
```

**SOLUTION:**

`cd level1/level2`


## GrPA 2

**QUESTION:**

We have a file named "systemcommands.txt" in the present working directory. Write a Bash command to change its permissions to

user: read, write, execute
group: execute
others: write

**SOLUTION:**

`chmod 712 systemcommands.txt`


## GrPA 3

**QUESTION:**

We want to change the file permissions of "someFile.txt" file as follows.

user: execute
group: execute, read
others: write

We will use the command `chmod XXX someFile.txt` where `XXX` represents a 3 digit number used to set the above permissions. Write a bash command to create a file named `XXX.digits` in the current working directory such `XXX` is the same three digit number used to set the permissions as mentioned above. The file your command creates can be empty.
For e.g. If your think the command `chmod 111 someFile.txt` will change the permission of file `someFile.txt` as mentioned above, then your solution should create a file named `111.digits` in the current working directory.

**SOLUTION:**

`touch 152.digits`


## GrPA 4

**QUESTION:**

Create two folders named dir1 and dir2 in the current working directory.
Try to write a single line bash command to perform the above task.

**SOLUTION:**

`mkdir dir1 dir2`

## GrPA 5

**QUESTION:**

Move only the file `file_1` present in `dir_1` to the empty directory `dir_2`.
Delete the directory `dir_1`.
`dir_1` and `dir_2` are directories in the current working directory. The operation should not change your current working directory.

**SOLUTION:**

`mv dir_1/file_1 dir_2; rm -r dir_1`
