# Nibo - nodejs irc bot
_nibo_ is useful IRC bot, that can be extended by creating additional __plugins__.

**License**: MIT

Full dependecies list is included in **package.json** or **requirments.txt** (with description)

# Before launching
First you have to patch **node-irc** module with *irc.js* patch, that fixes decoding problems.
Simply execute:
```
patch node_modules/irc/lib/irc.js irc.js.patch
```
Nibo uses **node-icu-charset-detector** module, that need **libicu**.
You can install **ICU** from your package manager, ie. for **apt**:
``` 
apt-get install libicu-dev
```
or build from sources http://site.icu-project.org/download

# Creating your own plugins
Plugins are files written in NodeJS, which extends the bot's functionality. They are able to access bot's IRC event, such as joining to the channel, saying something, and so on. Check the wiki for simple how to!

__WIP__, but almost done.. check the TODO file!