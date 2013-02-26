flowdock-trello
===============

Usage locally:
==============

```bash
  TRELLO_BOARDS=(board id here),(board id here)\
  TRELLO_KEY=(trello key here)\
  TRELLO_TOKEN=(trello token here)\
  FLOWDOCK_TOKEN=(flowdock token here)\
  FLOWDOCK_EMAIL=(email here\
  bundle exec ruby trello.rb
```

Or you can use rc file with ```source``` command for loading settings:

```
  cp rc.example rc
```

Set keys and load to the current environment:

```
  source rc
```

Heroku Deployment:
==================

```bash
  heroku create

  heroko config:set TRELLO_BOARDS=(board id here),(board id here)
  heroku config:set TRELLO_KEY=(trello key here)
  heroku config:set TRELLO_TOKEN=(trello token here)
  heroku config:set FLOWDOCK_TOKEN=(flowdock token here)
  heroku config:set FLOWDOCK_EMAIL=(email here)
  heroku ps:scale worker=1
```

