# 🔐 File Permissions in Linux

## Understanding Permissions

Every file has three permission sets:

```
-rwxr-xr--  1  alice  staff  4096  Jan 1 10:00  script.sh
 ↑↑↑↑↑↑↑↑↑
 │└──┬──┘└──┬──┘└──┬──┘
 │  Owner  Group  Others
 │
 └── File type: - = file, d = directory, l = symlink
```

| Symbol | Meaning |
|--------|---------|
| `r` | Read (4) |
| `w` | Write (2) |
| `x` | Execute (1) |
| `-` | No permission (0) |

## chmod — Change Permissions

### Numeric Method
```bash
chmod 755 script.sh     # rwxr-xr-x
chmod 644 file.txt      # rw-r--r--
chmod 600 secret.txt    # rw------- (private file)
```

### Symbolic Method
```bash
chmod +x script.sh          # Add execute for all
chmod u+w file.txt          # Add write for owner
chmod o-r secret.txt        # Remove read for others
chmod g=rx script.sh        # Set group to r-x
```

## chown — Change Ownership

```bash
chown alice file.txt            # Change owner to alice
chown alice:staff file.txt      # Change owner and group
chown -R alice /home/alice/     # Recursive change
```

## Common Permission Examples

| Permissions | Octal | Use Case |
|-------------|-------|----------|
| `rwxr-xr-x` | 755 | Shell scripts, binaries |
| `rw-r--r--` | 644 | Regular files |
| `rw-------` | 600 | SSH private keys |
| `rwx------` | 700 | Private directories |

---
Next → [Package-Management.md](Package-Management.md)
