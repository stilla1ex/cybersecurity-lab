# HTB Linux Module - Working with Files and Directories

*Essential file and directory operations in Linux*

---

## Objective
- SSH into the server at `the machine ip` (ACADEMY-NIXFUND).
- Check [here](https://github.com/Iam4lex/HTB/blob/main/Modules/001:Getting%20started/001:sshtokali.md) on how to ssh.

---

**Find the Name of the Last Modified File in the `/var/backups` Directory**

**Navigate to the `/var/backups` directory**
- Type or copy the following command to change to the directory:
```bash
cd /var/backups
```

**Check the last modified file**
- Use the `ls` command and `-lt` option (-t: sort by modification time, newest first) to list the files in the directory with timestamps
```bash
ls -lt
```
- The output will show files listed by modification time, with the last modified file at the top.

**Answer**
```bash
apt.extended_states.0
```
![image](https://github.com/user-attachments/assets/1ddddce1-87e0-44bf-9e1d-bb69cba65b06)


---

**Find the Inode Number of the `shadow.bak` File**

**Locate the `shadow.bak` file**
- Ensure that you're still in the `/var/backups` directory. If not, navigate back:
```bash
cd /var/backups
```

**Find the inode number**
- Use the `ls` command with the `-i` option to display inode numbers for all files:
```bash
ls -i shadow.bak
```

**Answer**
```bash
265293
```
![image](https://github.com/user-attachments/assets/b8e75030-c1ff-4838-a672-6aa95c3462ff)

---

*For questions or feedback about this module, please refer to the main repository documentation.*
