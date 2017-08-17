## WEBDRIVERIO sample

This sample test cover the following Objectives:
- Create two simple tests for the feature Login into BrowserStack web page
- Run the two test in parallel
- Link and configured the report generation across WebDriverIO

## Getting Started

* Clone the repo from https://github.com/fsejasm/WebdriverIO.git in the folder of prerequisites detailed(WebDriverIO)
* Install dependencies `npm install`

## Prerequisites

Node JS installed
WebdriverIO
   - Create folder WebDriverIO
   - CD to WebDriverIO
   - npm init -y
   - npm install --save-dev webdriverio
   - npm install -g selenium-standalone
   - selenium-standalone install

## Run tests

Currently was created in ./test/testspecs the following features login test:
* login.failure.spec.js
* login.success.spec.js

Easily can be changed to another system to login. I've used the Browserstack because it's interesting site to work with WEBDRIVERIO :).

Use the following command starting in the path to allow run in parallel the Login tests: 
c:\WebdriverIO\node_modules\.bin>wdio wdio.conf.js --suite login

## Reports

The Reports currently are in xml and json format in the ".bin\reports" Folder, from here it's possible to integrate with Jenkins with some more time :).


## Notes
* Firstly I had Troubles with my Node.js version it's important to update
* Setup and configure WebdriverIO selecting all options it's having issue, was fixed selecting just appropriated options as you can see in the file configuration(Wdio.conf.js)
* Test Runner troubles at the moment to run WEBDRIVERIO tests, Translated test to Mocha and everything go well :).
    
## Additional Resources
* Configured and run test  in https://www.browserstack.com/ to familiarize with the cross browser testing and integration with WebDriver.IO

##Author

Frank Alain Sejas Maranon






