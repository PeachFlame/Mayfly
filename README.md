# Mayfly
A small server for serving up files that have a fleeting lifecycle.


# Goals
Essentially: A python-based web server with command line interface. It's used to send files for one time downloading.

- place files in a directory and running Mayfly will see those files
- Mayfly will move them to a proper hosting directory
- Mayfly will also generate URLs based on a SHA1 hash of the file name
- spit out the URL on the command line so they can be pasted in an email, message, etc...
- once the URL was accessed, it would no longer function
- once the file was downloaded, it would be destroyed
- might be good to use [Bottle](http://bottlepy.org/docs/dev/index.html) as framework