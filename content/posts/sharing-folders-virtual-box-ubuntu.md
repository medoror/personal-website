---
title: "Sharing Folders Virtual Box Ubuntu"
date: 2019-01-20T19:02:18-05:00
draft: false
---
This was entirely more complicated than I thought. Sharing these notes to maybe help someone in the future

This will probably work a few versions of windows and ubuntu but these steps were defined with a Windows 7 host machine and an Ubuntu 17.04 Virtual Machine on Virtual Box 5.1.26. Before sharing folders, you must install Guest Additions. For instructions on how to do this, see <a href="https://help.ubuntu.com/community/VirtualBox/GuestAdditions">Guest Additions</a>.

1) Create a folder on the host windows machine. This example shows that a "VM_Share" folder was created locally.
2) On the Virtual Box VM, navigate to Devices &gt; Share Folder &gt; Shared Folder Settings
3) Create a folder under the “Machine Folders” heading
4) Choose the folder created in step 1. Check off the auto-mountable and make permanent
checkboxes

<a href="http://michaeledoror.com/wp-content/uploads/2017/09/VirtualBoxShareFolders.png"><img class="alignnone size-full wp-image-249" src="http://michaeledoror.com/wp-content/uploads/2017/09/VirtualBoxShareFolders.png" alt="" width="681" height="500" /></a>

5) Click ok
6) Open a terminal on the guest OS and navigate to <code>/media/sf_&lt;created folder&gt;</code>
7) This file by default will not have permissions so run the following command to add yourself to
the group : <code>sudo gpasswd -a &lt;username&gt; vboxsf</code>
8) Run <code>sudo reboot</code> to reboot the VM
9) You should now have access to here: <code>/media/sf_&lt;created folder&gt;</code>. Adding files to this folder
should add files to the same location on the host OS
