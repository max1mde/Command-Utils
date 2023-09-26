<div align="center">
  <h1>Command Utils</h1>
  <p>Some useful commands if you are <b>not</b> that familiar with linux and just want to setup a new linux server</p>
</div>

> **Warning**  
> All commands are only tested on a Debian 12 machine  
> so they might not work if you are using a different operating system


# Table of contents

- [Basics](#Basics)
- [Nginx](#Nginx)
- [Certbox](#Certbot-(For-HTTPS))

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
> You can use rm -r <directory> to delete a directory recursively
```
rm <file-name>
```

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

# [Nginx](https://de.wikipedia.org/wiki/Nginx)

### Install
```
sudo apt update
sudo apt install nginx
```

### Start
```
sudo systemctl start nginx
sudo systemctl enable nginx
```

### Status
```
sudo systemctl status nginx
```

### Restart
```
sudo systemctl restart nginx
```

# Certbot (For HTTPS)

###Install
```
sudo apt update
sudo apt install certbot python3-certbot-nginx
```

### Add domain and get a certificate for it
> **Important**
> The domain must point to your root servers IP
```
sudo certbot --nginx -d yourdomain.com
```

