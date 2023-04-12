# ansible_tutorial

This is my Ansible Repository

## Commands
### Tutorial 1
```
    1  ssh 192.168.56.121
    2  ssh 192.168.56.122
    3  ssh 192.168.56.123
    4  ls -la .ssh
    5  ls -la ~/.ssh
    6  cd ~/.ssh
    7  ls
    8  cat known_hosts 
    9  cd ..
   10  ls
   11  cd study/
   12  ssh-copy-id -i ~/.ssh/id_ed25519 192.168.56.121
   13  ssh-copy-id -i ~/.ssh/id_ed25519 192.168.56.122
   14  ssh-copy-id -i ~/.ssh/id_ed25519 192.168.56.123
   15  ls -la ~/.ssh
   16  ssh 192.168.56.123
   17   which git
   18  git clone git@github.com:praveen21b/ansible_tutorial.git
   19  cd ansible_tutorial/
   20  ls
   21  which nano
   22  dnf install nano
   23  which nano
   24  la
   25  ls
   26  nano README.md 
   27  cat README.md 
   28  git status
   29  git diff README.md 
   30  git add .
   31  git status
   32  git commit -m "Updated Readme file, initial commit"
   33  git push origin master
   34  git push origin main
   35  history
   ```

### Tutorial 2 (Initial Ansible Commands)
```
   36  dnf install ansible
   37  nano inventory
   38  ls
   39  cat inventory 
   40  git status
   41  git add .
   42  git status
   43  git commit -m "first version of inventory file is added"
   44  git push origin main
   45  which ansible
   46  ansible all ~/.ssh/id_ed25519 -i inventory -m ping
   47  ansible all ~/.ssh -i inventory -m ping
   48  ssh-keygen -t ed25519 -C "Ansible"
   49  ssh-copy-id -i ~/.ssh/ansible.pub 192.168.56.121
   50  ssh-copy-id -i ~/.ssh/ansible.pub 192.168.56.122
   51  ssh-copy-id -i ~/.ssh/ansible.pub 192.168.56.123
   52  ansible all ~/.ssh/ansible -i inventory -m ping
   53  ansible all --key-file ~/.ssh -i inventory -m ping
   54  ansible all --key-file ~/.ssh/ansible -i inventory -m ping
   ```

    To shorten ansible all --key-file ~/.ssh/ansible -i inventory -m ping
    -   create ansible.cfg on the local folder the original copy lies in /etc/ansible.cfg,
        but this file overridden by the local config file.
