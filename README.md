# 5.1 🧪 Lab Instructions — Basic Security and Identifying User Types

---

>💬 \*\*Tip:\*\* Paste this study guide into ChatGPT and ask for \*\*more instructions\*\* by specifying:  
>- “Provide step-by-step lab instructions for this objective.”  
>- “Include which Linux distro to use (Debian/Ubuntu or RHEL/Fedora).”  
>- “Show examples of installing, verifying, and managing desktop and server applications.”  
>- “Include minimal command-line practice for package management and development tools.”  
>- “Focus only on what is most important for passing the LPI Linux Essentials exam.”  

>This will prompt ChatGPT to give \*\*practical, exam-focused lab steps\*\* for each section.

---

**Objective:** Practice identifying user types, checking permissions, and exploring system and standard users.

---

### 👑 Root and Standard Users
- 🔄 **Switch to root**: `sudo -i` or `su - root`  
- 👤 **Switch to a standard user**: `su - username`  
- 💻 **Verify current user**: `whoami` and `id`  
- 🏠 **Check home directories**: `ls /root` (root), `ls /home` (standard users)

---

### 🖥️ System Users
- 🔍 **List all users**: `cat /etc/passwd`  
- 🚫 **Identify system users with no login shell**: `grep -E '(/sbin/nologin|/bin/false)' /etc/passwd`  
- 👥 **Check group memberships**: `cat /etc/group` and `id username`

---

### 📜 Login History & Current Users
- 📊 **Check last logins**: `last`  
- 👀 **See currently logged-in users**: `who` and `w`

---

### 🔐 Permissions & Security Practice
- 🔄 **Use sudo for commands as root**: `sudo whoami`, `sudo id`  
- 💡 **Test restricted access**: Try editing `/etc/shadow` as standard user (should fail)

---

### ✅ Lab Exercise Summary
- Switch between root and standard users  
- Identify system users and check login shells  
- Explore `/etc/passwd`, `/etc/shadow`, `/etc/group`  
- List current and last logged-in users  
- Practice using `id`, `whoami`, `last`, `who`, `w`, `sudo`, and `su`
