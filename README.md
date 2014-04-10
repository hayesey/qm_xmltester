XML-RPC Tester
==================================

```
Project version: 1.0 
Runtime environment: Java Servlet
Licence: "Public domain"
```
See the [changelog](CHANGELOG.md).

Project description
-------------------

This is a simple Java Servlet for testing XML-RPC with QueueMetrics.

http://www.queuemetrics.com

I use it with Tomcat it should work with any servlet container.

I wrote this several years ago for my own use, it's handy for seeing the exact output from the various XML-RPC requests from Queuemetrics while writing your custom reports.

There is a single Java class in the WEB-INF/classes folder, this does all the work.  

There is a simple compile bash script too.  The WEB-INF/lib folder contains the 3rd party Java packages you'll need to compile against.

For now the URL to the XML-RPC server is hard-coded into the code so this needs editing.  If I get round to it I'll put this into an input box on the web page and/or a settings file.

There's a basic web.xml config file in there which will get it working.  I've used it with Tomcat 5, 5.5, 6 & 7.


Requirements
------------
Java Servlet engine (such as the one you're already using for Queuemetrics)

Installing
----------

Just put the xmlrpc-tester folder into your webapps folder

Compile the servlet, the included compile script should do this for you.

```
cd <tomcat path>/webapps/xmlrpc-tester/WEB-INF/classes
./compile.sh
```

Then restart Tomcat or whichever servlet container you're using.

Usage istructions
-----------------

Web browse to:

<url to tomcat base>/xmlrpc-tester/xmltest

Authors
-------
Author: Paul Hayes <paul AT polog40 DOT co DOT uk>
Date: Sometime in 2009.  Uploaded in 2014.

