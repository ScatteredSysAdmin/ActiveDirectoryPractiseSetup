# ActiveDirectoryPractiseSetup
Script to automatically generate a random active directory filled with all the famous people of the netherlands

Currently used in 2012R2 Server. 

1. Get your server up and running and patched to the latest level
2. Run InstallAD_rev1.ps1 -> This will configure your domain controller
3. Run BuildOUsandUsers_rev3.ps1 -> this will create OU's and Cities based on values in the variables and fill the OU's randomly with names of people inside the ScriptSamplenames.csv

And you are done.

Helper scripts:

- ChangeDNSandJoinDomain.ps1 is a script to run on the member servers
- trustForDelegation.ps1 will change the AD properties of a managedServiceAccount to enable trustForDelegation
