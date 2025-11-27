# `rm -rf /* linux` 自毀指令

rm -rf （刪除 ）/*（路徑）

## Care and Caution with `rm -rf /*` Command

The command `rm -rf /*` is known in the Linux world as a **self-destruct code** because of its potential to delete every file in your system starting from the root directory `/`. The components of this command are:

- `rm`**:** This command is used to remove files or directories in Unix/Linux.
    
- `-r`**:** This option stands for "recursive," meaning everything inside directories will be removed recursively.
    
- `-f`**:** This option forces the removal of all files without prompting for confirmation.
    
- `/*`**:** Specifies the root directory, meaning begin deletion here and include all files and directories within.
    

## Consequences

- **Data Loss:** You could lose all your non-backed up data.
    
- **System Failure:** The system may become unbootable if system files are deleted.
    
- **Recovery Complexity:** Recovering from such command execution can be extremely complex and might not be entirely successful.
    

## Recommendations

- **Do Not Execute Lightly:** Avoid running this command unless you fully understand the consequences and have a strict need to delete the entire file system.
    
- **Backup Important Data:** Always ensure critical data is backed up regularly.
    
- **Use Restrictions:** Run as a non-root user or ensure file permissions restrict such destructive commands.
    
- **Testing Environment:** Test commands in a safe environment (e.g., virtual machines) before executing them in production.
    

## Alternatives

If your goal is to clear space or manage files, consider alternatives such as:

- `rm -rf /path/to/directory/*`**:** Operate within a specific directory.
    
- `find /directory -type f -delete`**:** More controlled removal of files.
    

**Always proceed with caution and ensure you have reliable backups and recovery plans.**

# `sudo su root`

The command `sudo su root` allows a user to switch to the root user, the system's administrative user with full access to all commands and files. Here's a breakdown of the command:

- `sudo`: Stands for "superuser do" and it's used to execute commands with superuser privileges.
    
- `su`: Stands for "substitute user" or "switch user". When followed by a username (like `root`), it switches the current user to the mentioned user.
    
- `root`: The username for the superuser account.
    

### Precautions

- **Administrative Access**: This provides full administrative access, and if misused, can lead to unintended or harmful changes to the system.
    
- **Security Risks**: Using `sudo su root` can expose your system to security risks if not used properly, therefore, make sure you know the implications of running commands as the root user.
    

Recommendations

- **Use Sparingly**: Use root privileges only when absolutely necessary.
    
- **Exit Promptly**: After completing tasks requiring root access, type `exit` or `logout` to return to a normal user prompt.
    

`df 查配置`