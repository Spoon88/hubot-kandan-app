Hubot-Kandan App
================
An easily deployed Hubot for Kandan, running in the cloud. A regular Algonquin round table of ribaldry and wit.

Installation
============
You'll need the heroku gem installed with Heroku. Then:

    git clone https://github.com/cloudfuji/hubot-kandan-app.git
    cd hubot-kandan-app

    # Add Hubot scripts to ./scripts if you want.
    # Visit the [Hubot Script Catalog](http://hubot-script-catalog.herokuapp.com/)
    # for some cool tricks you can teach your Hubot.

    # Push and scale
    heroku create --stack cedar
    git push heroku master --force
    heroku ps:scale app=1

    # *************** EDIT TO ADD YOUR VARIABLES *************** #
    # Add any other config variables your extra scripts may need #
    heroku config:add HUBOT_KANDAN_CHANNELS=1 HUBOT_KANDAN_HOST=kandan-host HUBOT_KANDAN_TOKEN=kandan-token 

You can get your `HUBOT_KANDAN_HOST` and `HUBOT_KANDAN_TOKEN` variables on Cloudfuji by clicking on App Settings while in Kandan:

![](http://github.com/cloudfuji/hubot-kandan-app/raw/master/settings.png)    

Or if you're running it elsewhere, use the `rake kandan:hubot_access_key`

Done! Never feel lonely again with your own robotic companion.

Other cloud providers
=====================
Installation instructions for other cloud providers are readily accepted, but be sure keep them as close to copy/paste as possible.

Credits
=======
The staff of News Radio for their inspirational lyrics.

License
=======
MIT - see LICENSE for more details

Get Involved!
=============
That's not a question, it's an order! Or more of a friendly offer, really. Kandan is a fully open-source app, so dive in and start adding features, fixing bugs (what bugs?), and cleaning up the code.

* Talk with us on the [mailing list](https://groups.google.com/forum/?fromgroups#!forum/cloudfuji)
* GitHub [issues tracker](https://github.com/cloudfuji/kandan/issues)
* Twitter [@cloudfuji](https://twitter.com/#!/cloudfuji)
* [New-wave open-source meetup](www.meetup.com/San-Francisco-New-Wave-Open-Source-Apps/) - we meetup once a month to share tips on how developers grow business around super high-quality open source software
* ... trained orca whales are also an acceptable communication medium, iff they arrive on tricycles.
