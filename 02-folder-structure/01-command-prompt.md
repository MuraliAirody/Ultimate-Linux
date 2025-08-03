```bash
root@ubuntu-dev:/#
```

### Is simply the command prompt inside your Ubuntu container

**Breaking it down**
- `root` → You are logged in as the root user (full admin privileges inside the container).
- `@ubuntu-dev` → The container’s hostname. You set it with --hostname ubuntu-dev when starting the container.
- `:/` → Your current working directory is / (the root of the filesystem inside the container).
- `#` → In Linux shells, # at the end of the prompt means you are root (a normal user gets $ instead).