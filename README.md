<div align="center">
  <h1>Command Utils</h1>
  <p>Some useful commands if you are <b>not</b> that familiar with linux and just want to setup a new linux server</p>
</div>

> **Warning**  
> All commands are only tested on a Debian 12 machine  
> so they might not work if you are using a different operating system


# Table of contents

- [Basics](#Basics)

# Basics

### Show running prozesses and RAM, CPU ... usage
> Is equivalent to the windows task manager
```
htop
```

### Navigate to a directory
```
cd <path>
```
> You can use `cd ..` to go to the parent diretory you are in

### Create a directory
```
mkdir <name>
```

### Delete a file
```
rm <file-name>
```
> You can use rm -r <directory> to delete a directory recursively

### View a file
```
cat <file-name>
```

### Create a file
```
touch <file-name>
```

### Copy a file/directory
```
cp -r /path/ /new/path/
```
