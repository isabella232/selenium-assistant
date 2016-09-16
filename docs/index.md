---
layout: index
title: "Home"
navigation_weight: 1
---
This library is designed to make using selenium a little easier in terms
of finding different releases of a particular browser and
generating a web driver instance.

If you have feedback or find bugs, please feel free to file issues on the
github repo.

# Drivers

To use this package, you'll need to include / download the drivers
for each browser yourself, this is to reduce dependencies for this project.
For example:

To use Google Chrome:

    npm install --save chromedriver

To use Opera:

    npm install --save operadriver

To use Firefox there isn't a helpful wrapper that works 100%, but you
can use the {@link SeleniumAssistant#downloadFirefoxDriver} to make
the appropriate driver available:

    const seleniumAssistant = require('selenium-assistant');
    seleniumAssistant.downloadFirefoxDriver()
    .then(() => {
      console.log('Finished downloading Firefox\'s Driver');
    });