# HERA-MI

To carry out your exercise I start by creating two virtual machines to be able to dock on them and then have containers in two separate networks.

To be able to synchronize the files from one container to the other 
I link the two by an ssh connection with a key authentication which allows the two containers to be linked constantly.

A directory is created on each container to accommodate the different files.

I clone the files on your Git Repository using the git clone command:

git clone https://github.com/hera-mi/test_material.git

I then create a cron task that will be able to automate the transfer of files from the directory of the containers C1 to C2 when a difference in content is present.

/1 * * * * scp -r -p home/files_hera_mi/ root@192.168.1.87:home/new_files_hera_mi

Then I create a dockerfile to be able to deploy the C3 container containing the Mongo DB database.

I also create a docker files to deploy the VPN on the C4 container.
