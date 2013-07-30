twitter-rss
===========

This is a python3 fork of Astalaseven's twitter-rss, https://github.com/Astalaseven/twitter-rss. 

This is currently not stable while I make changes to update it to python3 and clean up some bits. The old documentation should still apply.

Rss-generator for Twitter

* Doesn't make use of Twitter API (no registration needed, no 180 requests limitation, ...)
* Support account and hashtag following
* Option to append pic.twitter.com images in feed
* Generate a valid RSS-feed

## Installation

Requirements : `python3`

    git clone git://github.com/Astalaseven/twitter-rss.git

    sudo apt-get install python-pip
    sudo pip install -r requirements.txt
    
## Launch

You can edit `config.py` file to change the time between two updates (TIMER = 600),the server name 
(SERVER = 'localhost:5000'), where the files should be stocked (DIR = '/var/www/') and if you want 
to fetch the tweet pic (PICS = False).

    cd twitter-rss/
    python3 run.py
  
`run.py` will launch a webserver that can be used to create new feeds. You can also create them by opening 
`your_server/user/choosen-user-or-hashtag.xml` or by directly write them down in `user/user.txt` and `htag/htag.txt`.
