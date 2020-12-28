## Oracle Virtual Box

This project is about configuring and running Hercules on Linux. If you already have a Linux box set up, you can skip this step and resume at the <a href="https://github.com/davidjwalling/drinker/blob/master/docs/System-Prep.md">Preparing your Linux Environment</a> page.

On this site I document how to configure and run Hercules continuously in the cloud because I want to access my development environment at any time from practically anywhere over the Internet. These instructions can also be used to set up a virtualized Linux instance on your local computer. That is why I have included this page. Having a local Linux environment running virtually lets me test changes to my configuration before migrating them to the cloud.

You have choices if you want to run Linux virtually. I use Oracle VirtualBox. But, choices include other type-1 hypervisors like VMWare or OS-level virtualization like Docker or Windows Subsystem for Linux (WSL). I prefer VirtualBox for this project because it doesn't require Hyper-V and its control panel conveniently stays open when stopping and starting different virtual machines.

<table><tr><td>
As of this writing, Oracle VirtualBox 6.16 is the current version.<br>
Download the installer <a href="https://download.virtualbox.org/virtualbox/6.1.16/VirtualBox-6.1.16-140961-Win.exe">here</a>.<br>
Run the installer.<br>
For the most part, we'll accept default values in the wizard.<br>
Click Next.</td><td width=40%><img src="../images/virtualbox-1.png"></td></tr>
<tr><td>
Accept the defaults to install all options.<br>
Click Next.</td><td><img src="../images/virtualbox-2.png"></td></tr>
<tr><td>
Accept the defaults to create default links.<br>
Click Next.</td><td><img src="../images/virtualbox-3.png"></td></tr>
<tr><td>
Oracle VirtuaBox installs networking drivers.<br>
Click Yes to accept the update of network.</td><td><img src="../images/virtualbox-4.png"></td></tr>
<tr><td>
The wizard is ready to install now.<br>
Click Install.<br>
If Windows' User Account Control (UAC) asks for permission, click Yes.</td><td><img src="../images/virtualbox-5.png"></td></tr>
<tr><td>
The installation has completed.<br>
Leave the "Start Oracle VM VirtualBox" checkbox checked.<br>
Click Finish.</td><td><img src="../images/virtualbox-6.png"></td></tr>
<tr><td>
The VirtualBox Manager window is launched.<br>
That completes this stage.<br>
If you're going to install Osboxes Ubuntu now, leave this window open.<br>
We'll return to it to add a Virtual Machine definition.</td><td><img src="../images/virtualbox-7.png"></td></tr>
</table><hr>

Continue to [Osboxes Ubuntu](Osboxes-Ubuntu.md)  
Return to [README](../README.md)
