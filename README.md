## For ssh key setup in windows/mac/ubuntu

### ssh-keygen -t rsa -b 4096 -C "YOUR Email Id here"

#### if this command does not run or is not supported on your laptop, please run the command below and for the remainder of this setup,please use the string ed25519 in place of rsa.. If the command above runs successfully , please skip to step b.

### ssh-keygen -t ed25519 -C "ENTER YOUR Mail here"

#### Hit Enter for the following prompts and do not set a passphrase for your key
#### If the key was created successfully, you should see a random art image generated.

## Key configuration

### a.Run the command open ~/.ssh/config
### b.If the terminal responds saying that the file does not exist, run touch ~/.ssh/config to create a new file.
### c.Pastes these contents in the file: Host * AddkeysToAgent yes UseKeyChain yes IdentityFile ~/.ssh/id_rsa

## Add the key to your Github account

### a. Open the key file using the command cat ~/.ssh/id_rsa.pub
### b. Copy the contents printed out on the screen, from the "ssh-rsa" down to your email address.
### c. Navigate to github.com in your web browser
### d. In the top right corner, click on your profile and open settings > SSH and GPG keys > New SSH key
### e. Paste the key here, ensuring that there are no white spaces at the end of the key. Hit save.



