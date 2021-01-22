> 本文由 [简悦 SimpRead](http://ksria.com/simpread/) 转码， 原文地址 [www.phon.ucl.ac.uk](https://www.phon.ucl.ac.uk/courses/spsci/webprog/editor.php)

Web Editing and Debugging
-------------------------

_This page provide some practical information about how web pages can be edited, debugged and uploaded to a public web server._

### Local Editing of Web Pages

Web pages are stored in a simple readable text format, so you can use any text editor to create them and edit them. Word Processing software like Microsoft Word is **not** recommended, because such software uses proprietary formats for documents, and while these can be often exported to web format, you get very little control over the exact contents.

Currently we are recommending use of the [Brackets](http://brackets.io/) editor for Windows. This editor has been designed from the ground up as an editor for web programming with specific facilities to help you write in HTML, CSS & JavaScript.

Quick start with Brackets:

1.  Use Windows File Explorer to create a folder for your work. This could be on the local computer, or if you are using a lab computer it is best to create the folder on a memory stick.
2.  Start Brackets and use File|Open Folder to navigate to the folder.
3.  Use File|New to create a new file.
4.  Use File|SaveAs to give the file a name, for example "index.html".
5.  Type in the HTML, CSS or JavaScript code.
6.  Use File|Save to save your edits.
7.  Use File|Live Preview to see your page in the Chrome browser.

You can learn more about using Brackets with this [Getting Started](https://github.com/adobe/brackets/wiki/How-to-Use-Brackets) page.

### Local Display of Web Pages

Once you have typed in your web page you can use a web browser to display its contents from the file on the local machine.

One way to do this is to use Windows File Explorer to navigate to your project folder, then to double-click on the edited file. As long as the file has a ".htm" or ".html" extension to its name, Windows will then start the default browser to view the page.

An as an alternative you can type the name and location of the file into the address bar of the browser. Since the page is not coming from a web server, you cannot use the "http:" protocol in the URL, instead you need to use the "file:" protocol. An example might be:

file:///C:/myfolder/myfile.htm

Fortunately, Brackets provides an easier method than either of these. Brackets supports "Live Preview" using the Chrome browser. If you select menu option File|Live Preview, Brackets will start the Chrome browser and serve the page to the browser itself. You will see a copy of your document displayed in the browser. Live Preview can also be started by clicking on the lightning symbol at the top right of the editor Window.

A particular strength of this way of displaying web pages from within Brackets, is that Brackets will try and keep the displayed version of your file up to date even as you edit the web content. You can even modify the style sheet(s) for a page and see the consequences immediately.

### Chrome debugging tools

Once your page is displayed in the Chrome browser, you can use the Chrome development tools to help you find the cause of faults with the content or functioning of the page. To start the Development tools, press F12 when Chrome is running.

The development tools are particularly useful for tracking down problems with CSS styles and with JavaScript programming errors. With the _Elements_ tab open you are able to see exactly which style sheet rules are being applied to individual elements. This helps you identify why the object is not displaying in the style you had planned. The _Console_ tab is also very useful. Here you can see reports of syntactic errors in your code, probably the most common problem for new programmers. You can also add your own running commentary to your code through the use of the console.log() method which reports messages from your code in the console window. Finally, you can add the command debugger in your JavaScript code to cause your program to halt ("breakpoint") at that statement. You can then inspect the contents of variables in your code at that point in the execution of your script simply by typing their name in the console window.

Much more information on the Chrome tools is available at the [Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools/) web site.

### File transfer to PALS Server

For the purposes of the course (only) you will be allocated an area on the divisional web server. You can use this web space to upload all the web exercises and homeworks. It will also be the best place for you to implement and run your web experiment and to publish the web site that forms your course assessment.

To access the area, go to [https://www.phon.ucl.ac.uk/courses/spsci/webprog/extplorer](http://www.phon.ucl.ac.uk/courses/spsci/webprog/extplorer).

You will be allocated your own username and password, as well as your own folder within which you can create and upload files and folders. Your personal web space can then be accessed at the URL:  
http://www.phon.ucl.ac.uk/courses/spsci/webprog/users/_username_/

The extplorer interface allows you to upload, download, create and edit files. You can choose to perform all your web page editing using extplorer, but you may prefer to write and test your pages locally using the Brackets editor and upload them only after they are working.

You will need to use the web-space when you are running an experiment to allow external users to access your experiment and to allow experimental data to be collected on the server.

### File transfer to UCL Server

UCL provides a [personal web space](https://www.ucl.ac.uk/isd/services/websites-apps/personal-webpages) for every student. This is a convenient - and free - place to test out your web programming skills. It is the best place for you to create web pages unrelated to the course.

Your web address (URL) will be http://www.homepages.ucl.ac.uk/~xxxxxxx (your UCL UserID)

The UCL personal web space does not support server-side scripting, so it is not very useful for running experiments (for that use the PALS server).

Brief instructions on how to upload pages from a local machine to your personal web area:

1.  You need to know your UCL account ID and password.
2.  You must set up access to the UCL Desktop from your computer. Look at [Accessing desktop@UCL remotely (desktop@UCL Anywhere)](http://www.ucl.ac.uk/isd/how-to/desktop/accessing-desktop-browser). This may involve installing a service called "Citrix Receiver" on your computer.
3.  Once installed, you can connect to the UCL desktop by opening [https://my.desktop.ucl.ac.uk/](https://my.desktop.ucl.ac.uk/) in your browser.
4.  If requested, allow the remote computer ("virtual desktop") to read files from your local computer. This will allow you to copy files between computers.
5.  At the UCL Desktop you must then request access to the storage area for your personal web space. This is currently called the "T: drive". If the T: drive is not listed under the "Computer" icon, select Start | All Programs | Utilities | Mount Unix Filestore (T-drive). You will then be able to access the T: drive in the same way as you access other drives available on UCL Desktop.
6.  Use the Windows file explorer to open the T: drive and make sure there is a folder there called html.pub. This is the name of the folder where your personal web space files must be placed. If it doesn't exist, right-click and select New Folder and create it.
7.  You can now copy files from your local computer into html.pub. Find the files on the local computer in Windows file explorer, select and copy their names, then navigate to the html.pub folder and paste them.
8.  Finally you sometimes need to change the access permissions of the files in the html.pub folder since Windows can leave them readable by you but not by anyone else (which would not be good for a web page!). You can make the html.pub folder and all its contents available to anyone by using option Start | All Programs | Utilities | Publish Web Pages
9.  You can test out a page called "test.html" using a web browser at
    http://www.homepages.ucl.ac.uk/~uclyxxx/test.htmlwhere “uclyxxx” should be your UCL ID

Once you have set up your personal web space on the UCL system, you can gain access to it directly from Brackets using an extension that supports "FTP" (File Transfer Protocol). This turns out to be much more convenient, because you can edit and test your web pages on your local machine, then with a few clicks upload all the files to the remote server without having to go through UCL Desktop. For security reasons, this will not work with the PALS server.

Word count: 1507. Last modified: 13:50 14-Oct-2016.