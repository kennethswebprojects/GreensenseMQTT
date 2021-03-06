# GreensenseMQTT
This is a fork of 'thegardenapp', where the aim is to use a NodeJS based MQTT broker. The thinking behind this is to make 
a move towards the MQTT frontend being browser based as opposed to the use of Linear MQTT so as to make the interface 
more generic {moving away from solely Android/IOS focused}. This can later be integrated into the main Greensense project 
so that the initial setup scripts pull down npm the package manager / the latest version of node / mosca / bunyan, with the 
user arriving at a browser based interface.


This is the most basic Express v4.0 based set up as a template, generated by the Jetbrains Webstorm IDE.
'express-generator' is a package that goes about setting the basic infrastructure of the NodeJS web server, the main app.js 
file, the file infrastructure required, then lays the foundation of the coding practices of a NodeJS app, i.e. it creates 
folders for the location of the app.js to locate it's routes, as is convention amongst NodeJS developers.

Install latest versions of NPM & Node respectively.

******************************************************************
14th August 2019-

Porting the content from :
https://github.com/GreenSense/website

HTML of former index.html from above ^ page has been converted to /views/index.pug via the tool:
https://html-to-pug.com/

Most of the content of former index.html has been added as layout to /views/layout.pug

Many pathing changes have been made to take the pre-existing website and to copy it's content into the NodeJS, Express Generator file structure / convention.

******************************************************************

https://www.npmjs.com/package/express-generator
- NPM module for creating the basic framework of the app

https://www.npmjs.com/package/mosca
- NPM module that acts as an MQTT broker {this is what we'd ideally phase in to replace Linear MQTT in the chain of events}

https://www.npmjs.com/package/bunyan
- NPM module that aids in the parsing of incoming JSON messages, then 'pretties them up' before outputting them to the terminal.

Run 'mosca -v | bunyan' to start mosca and have bunyan display the received JSON cleanly at the terminal.

It matters most to prove the concept and have the correct protocols implemented properly, the fact that it's 
just outputting to the terminal will suffice in the preliminary phases, we can build upon this later within the frontend if it 
proves to be fruitful.

At this point, the template of the application has been created, the required modules have been installed, then at that early 
point the unchanged 'starting point' is up on the repositiory. {This is worth spending some time on as overall it reduces the 
'obstacle of entry' during the on-boarding process for newcomers to the Greensense project, at each phase of the supply chain,
be they particpants of the project or end service users}.
