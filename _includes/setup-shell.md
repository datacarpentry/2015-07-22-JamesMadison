Most bioinformatics is done on a computer running a Linux/UNIX operating system. In this workshop we will be doing data analysis on a remote linux server rather than on our own laptops. To do that we need: (1) a remote computer set up with all the software we'll need, (2) a way to connect to that computer, and (3) a way to transfer files to and from that computer.

Since most of us don't have our own Linux server running somewhere, we'll *rent* a server from Amazon for the duration of this course.

<!--

**Create AWS account**

First, create an Amazon Web Services account: <http://aws.amazon.com/>. Make sure to register for a Basic (Free) account. You will be required to enter a credit card and billing information -- don't worry, I have free use vouchers for you so you will not be charged. You will need to verify a phone number before you can start using AWS. Note that your Amazon.com account is not connected to your Amazon Web Services account. They are two separate entities with different login and billing information.

Once you have your AWS account set up and can successfully log in to [console.aws.amazon.com](https://console.aws.amazon.com/), email Stephen Turner (<a href="http://www.google.com/recaptcha/mailhide/d?k=01uXi4zl-bIdygzSeXF4649A==&amp;c=_81hv-sTQvJ9rjELjZNDJeAXTvLvkpfD9KEuItpEHTE=" onclick="window.open('http://www.google.com/recaptcha/mailhide/d?k\07501uXi4zl-bIdygzSeXF4649A\75\75\46c\75_81hv-sTQvJ9rjELjZNDJeAXTvLvkpfD9KEuItpEHTE\075', '', 'toolbar=0,scrollbars=0,location=0,statusbar=0,menubar=0,resizable=0,width=500,height=300'); return false;" title="Reveal this e-mail address">sd...</a>@virginia.edu) to obtain a voucher to be able to use AWS for free during and after our course. Use the subject line "RNA-SEQ COURSE AWS VOUCHER" in your email to me. Once you have your voucher, return to the AWS console, click your name at the top right, click "Billing & Cost Management", then on the left, click "Credits". Redeem the promo code I sent you -- this credit will buy enough compute time to complete this workshop and for several future RNA-seq analyses.

If you're interested in trying out EC2 prior to the workshop, watch [this short video](http://youtu.be/SKM0BB0F02Q) to learn how to launch your first instance (and make sure to stop the instance after you're done). Whether you do this or not, *be sure to stop or terminate any running EC2 instances when you are done with them*. After the course, you may deactivate your AWS account if you wish under the "My Account" settings in the AWS console.

-->

- **(_All participants_) Download a file transfer program.** Download and install Cyberduck (free): <https://cyberduck.io>. We will use this transfer files back and forth between our local laptops and our remote linux server running on Amazon. Note: If using a Mac, download from the website above (free), *not* from the Mac App Store (paid). 
- **(_All participants_) Download a text editor.** We may wish to view and/or edit plain text files. To do this, let's use a better alternative to the built-in Notepad (Windows) or TextEdit (Mac). Download and install Sublime Text (works for Windows and Mac): <http://www.sublimetext.com/>. 
- **_For Windows users only_**:
    - **Install git-bash**. Download and run [the installer here](http://msysgit.github.io/). This will install a "real" command line on a Windows machine.
    - **Install the Software Carpentry Installer**. _After_ installing git-bash, [download and install the software carpentry installer here](http://files.software-carpentry.org/SWCarpentryInstaller.exe).
    - **Download a terminal emulator.** 
        - [Download the latest version of PuTTY here](http://the.earth.li/~sgtatham/putty/latest/x86/putty.exe). Ensure that you can run this .exe file (no installation necessary). This is your terminal emulator.
        - [Download puttygen here](http://the.earth.li/~sgtatham/putty/latest/x86/puttygen.exe). This will allow you to generate a key used to log in to your cloud computing instance.
- **Bookmark these links**: These resources will be useful for logging in and transferring data to your instance.
    - [Transferring data between your computer and your EC2 instance](http://angus.readthedocs.org/en/2014/amazon/transfer-files-between-instance.html)
    - [Logging on to your instance for windows](http://angus.readthedocs.org/en/2014/amazon/log-in-with-ssh-win.html)
    - [Logging on to your instance for Mac](http://angus.readthedocs.org/en/2014/amazon/log-in-with-ssh-mac.html)

