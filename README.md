# devops-system
A devops ruby system util to get your system information and performing all the tasks on the clusters and computing storage. A ruby gem that will solve most of the daily devops tasks on the computing storage. Updating it with the complete devops including a yaml creator for the ansible. The ruby gem has been published [devopsutils](https://rubygems.org/gems/devopsutils). Releasing a new version with system profiling tools. 

```
gem install devopsutils
require "devopsutils"
```
```
initialize the class
devops = DevopsSystemUtil.new("/Users/gauravsablok/Desktop/Code/Release/datasets",
                                                          "/usr/bin/desktop","fasta")
devops.geneatepath # generate the bash commands for file movement
devops.memory # check the memory
devops.getsystemInfo # get the system information to kill the running pid process.
devops.user # get the user information
devops.changepermission(directory_path) # will only ask for the password
# will generate all the scp commands for the remote file transfer for file type mentioned
# means look for csv file in this directory and genrate the transfer
devops.generate_push_ssh("/Users/gauravsablok/Desktop/Code/Release/datasets", "csv", "1.1.1.1", "/usr/Desktop") 
devops.filesearch #additional methods
devops.list #additional methods
```
Gaurav Sablok \
University of Potsdam \
Potsdam,Germany 
