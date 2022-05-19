# LearnOpenVas
This is a writeup of me learning how to use OpenVas.

## Setup
I am using an m1 macbook air, kali linux with parallels.
I made sure my kali distro is fully updated.
Then I started the installation process.
### Installation 
I ran **_sudo apt install openvas_**

After that is done I run **_gvm-setup_** (Note this takes a few minutes)

Finally I check my setup by running **_gvm-check-setup_**
## Starting OpenVas
Run **_sudo gvm-start_**. Then on a browser go to https://127.0.0.1:9392
 
## Troubleshooting
If you dont know the credential after installing do the following to reset password

1.**_sudo -u _gvm gvmd --get-users**_

2.And, reset password for 'admin' username using this command **sudo runuser -u _gvm -- gvmd --user=admin --new-password=StrongPassword**

After installing OpenVas, I get an error when trying to scan **Failed to find config ‘daba56c8-73ec-11df-a475-002264764cea’**. To fix this I did
  
