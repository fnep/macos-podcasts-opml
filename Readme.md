# MacOS Podcasts OPML export

This helper script tries to export the Apple MacOS Podcast subscription list as OPML in case you want to switch to another podcatcher. It looks like Apple "forgot" to add this feature to their new Catalyst app. The subscriptions are placed in a sqlite3 file. This script simply selects the data and prints them as OPML.

### Warning
- **No batteries included** ... this is just the code i use. It's not really maintained. It's just here in case it's useful for somebody. 

### Dump as OPML:

``` commandline
$ ./macos-podcasts-opml.py
<?xml version="1.0" ?>
<opml version="1.0">
  <head>
    <title>MacOS Podcasts</title>
  </head>
  <body>
    <outline htmlUrl="https://feed.url" text="Show Name" type="rss" xmlUrl="https://show.website"/>
    <outline htmlUrl="https://feed.url" text="Show Name" type="rss" xmlUrl="https://show.website"/>
    <outline htmlUrl="https://feed.url" text="Show Name" type="rss" xmlUrl="https://show.website"/>
  </body>
</opml>
```          

### Dump into a file
 ``` commandline
$ ./macos-podcasts-opml.py > podcasts.opml
```          
