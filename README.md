#Codename One offline build framework

Using CN1 server has many advantage but there is some disadvantage - build time (specially for Windows port), you need basic account to get sources and professional to build code with stable API version. That is why this project was setup. Here are everything needed for offline build.
Of course this way is more complicate than using CN1 server but in many case it is useful. Especially for windows port which is not complete on CN1. Here I will try to gather some new port which is much more complete and actual.

Note: This project is not supported by CN1 team so do not ask about it on their forum.

##Installation

1. Copy the VM folder to your Netbeans/Eclipse project.
2. If you do not have rsync (cygwin64 folder) or XMLVM copy it.
3. In VM folder you need to create native project or make link to it.
4. Check the ant parameters and correct (VM\cn1offline.properties).
5. Run ant task in VM folder (WP8_3.1/WP8_3.2/WP8_3.3).

##What where done

1. I correct xmlvm2csharp.xsl file: 
	- implement dex:rem-double and dex:rem-double-2addr
	- correct template for try/catch
	- skip some unnecessary variable initialization
2. Update XMLVM port for csharp
3. Create Ant framework to cross compile java code offline


##To do

1. Implement dex:filled-new-array|dex:filled-new-array-range (not very important but maybe someone can fix the last cross compile error)
2. Setup Ant task for other platforms (iOS,Android).
3. Create Ant task to copy/update resources
4. Create native project framework
5. Compile and build native code

##Links to used projects
	CN1 - (https://github.com/codenameone/CodenameOne)
	Cygwin - (https://cygwin.com/)
	XMLVM - (http://xmlvm.org/overview/)

