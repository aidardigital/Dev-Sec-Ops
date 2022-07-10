Shell Aliases Theory

# Login Shell
A Login shell is created after a successful login of user. For example, when you login t a Linux system via terminal, SSH or switch to user with “su -” command.

When a login shell start, it runs a set of predefined script to configure shell environment. To identify the login shell, run the below command on terminal.

# A Login Shell executes following scripts:
- Login shell executes /etc/profile
- /etc/profile executes all scripts in /etc/profile.d/
- Then executes users ~/.bash_profile
- ~/.bash_profile executes users ~/.bashrc
- ~/.bashrc executes /etc/bashrc

# Non Login Shell
Non Login Shell is the shell, which is started by the login shell. For example, A shell which you started from another shell or started by a program etc.

A non login shell executes the following script to set the shell environment.

- Non login shell first executes ~/.bashrc
- Then ~/.bashrc executes /etc/bashrc
- /etc/bashrc calls the scripts in /etc/profile.d

# Check Login vs Non Login Shell
To find the current shell is login shell or non login shell simply run the below command. See the results and find the different between them.
- echo $0
Login shell output will be -bash or -su.

Non logins shell output will be bash or su
