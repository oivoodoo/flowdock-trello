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

Heroku Deployment:
==================

  heroku create

  heroko config:set TRELLO_BOARDS=(board id here),(board id here)
  heroku config:set TRELLO_KEY=(trello key here)
  heroku config:set TRELLO_TOKEN=(trello token here)
  heroku config:set FLOWDOCK_TOKEN=(flowdock token here)
  heroku config:set FLOWDOCK_EMAIL=(email here)

