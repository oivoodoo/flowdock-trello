flowdock-trello
===============

Usage locally:
==============

TRELLO_BOARDS=(board id here),(board id here)

TRELLO_KEY=(trello key here)

TRELLO_TOKEN=(trello token here)

FLOWDOCK_TOKEN=(flowdock token here)

FLOWDOCK_EMAIL=(email here)

bundle exec ruby trello.rb

Or you can use rc file:

  cp rc.example rc

Set all needed keys in the rc file and before run bundle exec ruby trello.rb,
use:

  source rc

Heroku Deployment:
==================

  heroku create

  heroko config:set TRELLO_BOARDS=(board id here),(board id here)
  heroku config:set TRELLO_KEY=(trello key here)
  heroku config:set TRELLO_TOKEN=(trello token here)
  heroku config:set FLOWDOCK_TOKEN=(flowdock token here)
  heroku config:set FLOWDOCK_EMAIL=(email here)
  heroku ps:scale worker=1

