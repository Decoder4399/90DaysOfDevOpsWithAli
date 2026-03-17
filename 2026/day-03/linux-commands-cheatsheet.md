# DevOps Important Commands Cheat Sheet

## Linux Basics

    pwd — Show current directory path
    ls — List files and directories
    cd — Change directory
    mkdir — Create a new directory
    rm — Remove files or directories
    cp — Copy files/directories
    mv — Move or rename files
    touch — Create empty file
    cat — View file content
    nano — Edit file in terminal
    chmod — Change file permissions
    chown — Change file ownership

## Process Management

    ps — Display running processes
    top — Real-time process monitoring
    htop — Interactive process viewer
    kill — Terminate process by PID
    killall — Kill processes by name
    nice — Start process with priority
    renice — Change process priority

## Package Management (Ubuntu/Debian)

    apt update — Update package list
    apt upgrade — Upgrade installed packages
    apt install — Install a package
    apt remove — Remove a package

## Networking

    ifconfig — Show network interfaces (legacy)
    ip a — Show IP addresses
    ping — Check network connectivity
    netstat — Show network connections
    ss — Display socket statistics
    curl — Transfer data from/to server
    wget — Download files from internet

## Disk & File System

    df -h — Show disk space usage
    du -sh — Show directory size
    mount — Mount filesystem
    umount — Unmount filesystem
    lsblk — List block devices

## Permissions & Users

    whoami — Show current user
    id — Show user ID and groups
    useradd — Create new user
    passwd — Set/change password
    su — Switch user
    sudo — Run command as admin

## Archive & Compression

    tar -cvf — Create archive
    tar -xvf — Extract archive
    gzip — Compress file
    gunzip — Decompress file

## Git (Version Control)

    git init — Initialize repo
    git clone — Clone repository
    git status — Show repo status
    git add — Stage changes
    git commit — Save changes
    git push — Upload changes
    git pull — Fetch & merge changes
    git branch — List/create branches
    git checkout — Switch branch

## Docker

    docker build — Build image
    docker pull — Download image
    docker run — Run container
    docker ps — List containers
    docker images — List images
    docker stop — Stop container
    docker rm — Remove container

## Kubernetes (kubectl)

    kubectl get pods — List pods
    kubectl get svc — List services
    kubectl apply -f — Apply config file
    kubectl delete -f — Delete resources
    kubectl describe pod — Detailed pod info
    kubectl logs — View pod logs

## CI/CD & System

    systemctl start — Start service
    systemctl stop — Stop service
    systemctl restart — Restart service
    systemctl status — Check service status
    journalctl -u — View service logs

## Monitoring & Logs

    free -m — Show memory usage
    uptime — Show system uptime
    vmstat — System performance stats
    iostat — Disk I/O stats
    tail -f — Live log monitoring
    grep — Search text in files


