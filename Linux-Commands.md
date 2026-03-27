# 💻 Essential Linux Commands

## Navigation

```bash
pwd             # Print current directory
ls              # List files
ls -la          # List all files (including hidden) with details
cd /home        # Change to /home directory
cd ..           # Go one level up
cd ~            # Go to your home directory
```

## File Operations

```bash
touch file.txt          # Create empty file
mkdir myfolder          # Create directory
cp file.txt backup.txt  # Copy file
mv file.txt docs/       # Move file
rm file.txt             # Delete file
rm -rf myfolder         # Delete folder (careful!)
cat file.txt            # View file contents
less file.txt           # Scroll through file
nano file.txt           # Edit file (beginner-friendly editor)
```

## Searching

```bash
find / -name "file.txt"         # Find file by name
grep "hello" file.txt           # Search text inside file
grep -r "hello" /home/user/     # Search recursively
```

## System Info

```bash
top                     # Live process viewer
htop                    # Better process viewer (install first)
df -h                   # Disk usage
free -h                 # RAM usage
ps aux                  # Running processes
kill 1234               # Kill process by PID
```

## Networking

```bash
ping google.com         # Test internet
ip a                    # Show IP addresses
curl https://example.com # Fetch URL
wget https://example.com/file.zip  # Download file
```

## Tips

- Use **Tab** to auto-complete commands and paths
- Use **↑ ↓** arrows to scroll command history
- `Ctrl+C` stops a running command
- `man ls` shows the manual for any command

---
Next → [File-Permissions.md](File-Permissions.md)
