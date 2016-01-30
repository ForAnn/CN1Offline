#Codename One offline build framework

Using CN1 server has many advantage but there is some disadvantage - build time (specially for Windows port), you need basic account to get sources and proffessional to build code with stable API version. That is why I try to prepare project where is everythink you need for offline build.
Of course this way is more complicate than using CN1 server but in many case it is usefull. Especially for windows port which is not complete on CN1. Here I will try to gother some new port which is much more complete and actual.

Note: This project is not supported by CN1 team so do not ask about it on their forum.

##Installation

1. Copy the VM folder to your Netbeans/Eclipse project.
2. If you do not have rsync (cygwin64 folder) or XMLVM copy it.
3. In VM folder you need to create native project or make link to it.
4. Check the ant parameters (VM\cn1offline.properties).
5. Run ant task in VM folder (WP8_3.1/WP8_3.2/WP8_3.3).

Note:  In some versions of Codename One, you will need to perform an explicit "Build" before it will work in the simulator.  I.e. Right click on your project in the project explorer, and select "Build".  After that you should be able to run it normally in the simulator.

##What where done

1. I correct xmlvm2csharp.xsl file to implement 
	- dex:rem-double and dex:rem-double-2addr
	- correct template for try/catch and variable initialization
2. Change XMLVM port for csharp
2. Create Ant framework to build java cfode offline


##To do

1. Implement dex:filled-new-array|dex:filled-new-array-range
2. Setup Ant task for other platforms (iOS,Android).

##Links to used projects
	CN1 - https://github.com/codenameone/CodenameOne
	Cygwin - https://cygwin.com/
	XMLVM - http://xmlvm.org/overview/

