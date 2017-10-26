# GitHub Repositories



## Create account on [github](https://github.com)

##Create Repositories on [github](https://github.com) 

## Using SSH to clone GitHub Repositories to local HD - Ubuntu 16.04



### Git Installation [link](https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-14-04)

```sh
sudo apt-get update
sudo apt-get install git
```

### SSH key setup

- Generating a new SSH key

  1. Paste the text below, substituting in your GitHub email address.

     ```sh
     ssh-keygen -t rsa -b 4096 -C 'email address'
     ```

     The entire key generation process looks like this:

     ```
     ssh-keygen -t rsa
     Generating public/private rsa key pair.
     Enter file in which to save the key (/home/demo/.ssh/id_rsa): 
     Enter passphrase (empty for no passphrase): 
     Enter same passphrase again: 
     Your identification has been saved in /home/demo/.ssh/id_rsa.
     Your public key has been saved in /home/demo/.ssh/id_rsa.pub.
     The key fingerprint is:
     4a:dd:0a:c6:35:4e:3f:ed:27:38:8c:74:44:4d:93:67 demo@a
     The key's randomart image is:
     +--[ RSA 2048]----+
     |          .oo.   |
     |         .  o.E  |
     |        + .  o   |
     |     . = = .     |
     |      = S = .    |
     |     o + = +     |
     |      . o + o .  |
     |           . o   |
     |                 |
     +-----------------+
     ```

     The public key is now located in /home/demo/.ssh/id_rsa.pub The private key (identification) is now located in /home/demo/.ssh/id_rsa

  2.  copy the ssh public key from local HD

     ```sh
     cat ~/.ssh/id_rsa.pub
     ```

- Copy the ssh public key to GitHub

  go to GitHub --> Setting --> SSH Keys

- Clone GitHub Repository to local HD

  1. copy SSH link

  ​        go to 'Clone and Download' and copy the SSH link

  ​

  2. copy it to Ubuntu 

      ```sh
     git clone 'SSH link from GitHub'
      ```

  git add .

  git status

  git commit -m 'your message'

  git push 

  ​
