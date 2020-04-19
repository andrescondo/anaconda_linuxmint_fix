# anaconda_linuxmint_fix
This is to address anaconda's current oversight of the Linux Mint OS, a distro based off of Ubuntu.  
As a result of this oversight, running anaconda-navigator from the command line will fail because the search
conducted in vscode.py fails to find Linux Mint as a distro.

This file is found in the following directory: 
./anaconda3/lib/python3.7/site-packages/anaconda_navigator/api/external_apps/vscode.py

The file posted has as sole modifications the 'linuxmint' keywords where only 'debian' and 'ubuntu' were listed for 
that branch of Linux distros using the deb package managers.

Following these addition, anaconda works fine in Mint.
Enjoy.
