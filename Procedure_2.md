# Git


**STEP 1: Generate SSH key**

     command : ssh-keygen -t ed25519 -C "your_email@gmail.com"

     Creates a secure key pair:
     private key → stays on your laptop
     public key → goes to GitHub
     (set passphrase if asked.)


**STEP 2: Start SSH agent & add key**

     command : eval "$(ssh-agent -s)"
               ssh-add ~/.ssh/id_ed25519

     Loads your key into memory so Git can use it


**STEP 3: Copy public key**

     command : cat ~/.ssh/id_ed25519.pub

     Prints your public key (copy the full line).


**STEP 4: Add key to GitHub**
      
     Settings → SSH and GPG keys
     New SSH key
     Paste → Save


**STEP 5: Test SSH connection**

     command : ssh -T git@github.com

     Hi username! You've successfully authenticated...




