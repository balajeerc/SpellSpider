=============
SpellSpider
=============

A simple web crawler that can be used to check grammar and spelling on a site

Do checkout the:
 - Source repository: https://github.com/balajeerc/SpellSpider

Building and running
--------------------
The source distribution comes with an Eclipse project that should work as is. You will need to set the commandline arguments as shown below.
You can export to a jar file and run the application with:

$ java -jar SpellSpider.jar <targetUrl> <targetOutputDirectory>

eg.
$ java -jar SpellSpider.jar http://www.balajeerc.info /Users/balajeerc/Temp/crawl

NOTE: The url must contain "http://www." preceeding the domain name. For some reason, crawler4j that this application relies on doesn't like urls without it.

Output
-------
When the application is run, the output directory gets populated with two files
a) consolidated.txt which simply contains a dump of all the text from the site
b) errors.csv which is a comma separated file listing all the errors found

Should you have any problems with this application, please drop me an email and I'll get back to you ASAP: mail at balajeerc dot info


License
---------
This application's code is licensed under GNU GPL v3 (included with source)