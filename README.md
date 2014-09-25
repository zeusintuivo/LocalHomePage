### A Local Home Page for OSX Web Development
### Modified for the [AscendProject](http://ascendproject.org) Class
This is a small and simple local home page that automatically lists, and provide links to, your local sites.
Taken from the sample post [blog post](http://mallinson.ca/post/osx-web-development)
That was written about setting up your Mac for web development.

![Sample Screen Shot](img/screenshot.png)

### Install

I recommend to install in the base Sites inside an index.html folder.
*Notice I said index.html folder not an index.html file.

It should look something like this.

~~~
+--- ~/Sites/
  +----index.html/
      .
      ├── README.md
      ├── config.sample.php
      ├── css
      │   └── main.css
      ├── img
      │   ├── icon-gear.png
      │   ├── icon-wp.png
      │   └── screenshot.png
      ├── index.php
      └── info.php

~~~

That way it does not leave a bunch of files in the base directory.


Once you Dump the files, or move the files, or copy the files,
Make sure to copy the config.sample.php into a file called config.php

~~~
cp config.sample.php config.php
~~~


So now we should have a new file in there like this:
~~~
+--- ~/Sites/
  +----index.html/
      .
      ├── README.md
      ├── config.php
      ├── config.sample.php
      ├── css
      │   └── main.css
      ├── img
      │   ├── icon-gear.png
      │   ├── icon-wp.png
      │   └── screenshot.png
      ├── index.php
      └── info.php

~~~

Make sure you open that file with 'subl' aka Sublime. and edit the necessary changes.

Inside line 16:

~~~
/** directory name(s) */
$dir = array("/Users/username/Sites/*");
~~~

Make that match your user name

Read the rest of the config file to and change it to match your needs.

* Notice at the botton of the config.php file there is a '$hiddensites' list
that you might like to edit as well.


* img/icon-gear.png from [Icons DB](http://www.iconsdb.com/black-icons/gear-2-icon.html)