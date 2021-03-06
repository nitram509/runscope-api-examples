Runscope Test Backup
============
Sample app that uses the Runscope API to back up your
Runscope tests. The app will create new folders for
each bucket and dump the contents of every test into
a JSON file.

Requirements
------------
- Python
- Python Requests library
- Runscope API key (access token)

Configuration
------------
Copy ```config.json.sample``` to ```config.json``` and then 
make the necessary modifications (add your access token
from Runscope).

Obtaining an Access Token
------------
To create an access token, login to your Runscope account and navigate to [https://www.runscope.com/applications](https://www.runscope.com/applications). Here, click ```Create Application``` -- for name, type in *Test Backup App*. For website and callback URLs, you can just type in ```https://www.runscope.com``` as placeholders (these URLs are never used -- we're just creating an application for the personal access token). After you've created the application, copy the personal access token (i.e. ```5ffffffe-ab99-43ff-7777-3333deee99f9```) and use it in ```config.json```.

Running the App
------------
$ python backup.py

ChangeLog
------------
2015-08-17 - Initial release.
