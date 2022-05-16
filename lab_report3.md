## Lab Report 3

### Part 1
Here we show how to modify ssh config file. First we simply use command `cd .ssh` to go to the ssh directory.  
![](LR3/ssh_setup.png)  
![](LR3/sshprt.png)  
Now we can modify this file via many ways, and I'm going to use `vim filename` here to modify this file.  
![](LR3/config.png)  
Now we can simply use `ieng6` to login to remote instead of the full name.  
![](LR3/ssh_res.png)
Similarly for `scp` command.  
![](LR3/ssh_scp.png)  
  
### Part 2
We are going to set up git streamline on remote terminal. Go to profile-setting-developer setting to generate key.  
![](LR3/gitkey.png)   
We save the generated key to somewhere for easy access.  
![](LR3/gitkeystore.png)  
Now we use git commands, first we go to a existing repo and make change to a file.  
We make change directly on terminal using vim to the demo two sum java code
![](LR3/gitvim.png)  
![](LR3/gitvimm.png)  
We now we commit and push.  
![](LR3/gitvim_cap.png)
  
### Part 3
We can use `scp -r` command to upload whole directory!  
![](LR3/scpr.png)  
And we check our remote repo, also if our program runs. Since we already create the makefile we can just use `make test` to run desired tests while compling java file.
![](LR3/sshrun.png)  
Now we make everything in to single line.  
![](LR3/onelinecmd.png)  
Check if runs:   
![](LR3/onelineres1.png)  
![](LR3/onelineres2.png)
