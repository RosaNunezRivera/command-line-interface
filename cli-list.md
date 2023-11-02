# Command Line Interface (CLI)

A sheet for bash commands.

## Commands List

### Listing directories and files

```bash
| Command       | Description                                                            |
| ------------- | -----------------------------------------------------------------------|
| ls            | List all files and directories in the currect working directory        |
| ls -a|--all   | List all hidden files and directories in the currect working directory |
|               | hidden files star with a . (dot)                                       |
| ls -l         | List directories and add more information like type, permission, owner,|
|               | name, etc.                                                             |
| ls -R         | List directories until achieve the last directory and files            |
| pwd           | Print the current directory                                            |
| ------------- | -----------------------------------------------------------------------|
```

### Navigating directories

```bash
| Command         | Description                                                          |
| -------------   | ---------------------------------------------------------------------|
| cd <directory > | Change the current directory to the directory specified              |
| cd ..           | Return to the previos directory                                      |
| cd ~            | Go to the home directory                                             |
| cd /            | Go to the root directory                                             |
| -------------   | ---------------------------------------------------------------------|
```

### Creating directories

```bash
| Command             | Description                                                      |
| ------------------- | -----------------------------------------------------------------|
| mkdir <directory >  | Create a new directory                                           |
| mkdir <dir > <dir > | Create multiple directories                                      |
| ------------------  | -----------------------------------------------------------------|
```

### Deleting directories

```bash
| Command             | Description                                                      |
| ------------------- | -----------------------------------------------------------------|
| rmdir <directory >  | Delete non-empty directory                                       |
| rm -r <directory >  | Delete directory including contents                              |
| ------------------  | -----------------------------------------------------------------|
```

### Creating files

```bash
| Command                  | Description                                                 |
| -------------------------| ------------------------------------------------------------|
| touch file.txt           | Create file or update existing files                        |
| touch file1.txt file2.tx | Create multiple files                                       |
| touch file1.txt file2.tx | Create multiple files                                       |
| touch {file1, file2}.txt | Create multiple files                                       |
| touch file{1..3}         | Create test1, test2 and test3 files                         |
| ------------------------ | ------------------------------------------------------------|
```

### Redirect the output to a file

```bash
| Command                  | Description                                                 |
| -------------------------| ------------------------------------------------------------|
| echo "Hi" > file.txt     | Redirect the output to a file, overrite with content        |
| echo "World!" >> file.txt| Redirect the output to a file, append with content          |
```

### File permissions

```bash
|Access class              | Operatos            | Type          |
|--------------------------| --------------------|---------------|
| u (user)                 | +(add access)       | r (read)      |
| g (group)                | -(remove access)    | w (write)     |
| o (others)               | = (set exact access)| x (excecute)  |
| a (all of the above)     |                     |               |
|--------------------------| --------------------|---------------|
```

Permission: What do those letters means? ***drwxr-xr-x***
    ***d:*** directory
    ***rwx*** read write excecute (user)
    ***r-x*** read and execute (group)
    ***r-x*** read and execute (other)

```bash
| Command                  | Description                          |
| -------------------------| -------------------------------------|
| chmod user operator<file>| Give the user execute permission     |
|--------------------------| -------------------------------------|
```
