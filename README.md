## Introduction

Stub project for [Dropwizard](http://dropwizard.codahale.com/) example integrated with [Atmosphere](https://github.com/Atmosphere/atmosphere) rest-chat example.

NOTE: The base for this is [dropwizard-atmosphere] (https://github.com/mgutz/dropwizard-atmosphere).

CHANGES: Differences with the above:
* Upgraded atmosphere and atmosphere-js to 2.0.x line
* Removed unnecessary junk (db, auth, and other modules)
* Removed non-essential thing from config file
* Forced non-blocking connector type in the service irrespective of what is set in the config

How to use this: As the name suggests, use it as a stub.

## Overview

Dropwizard is a high performance JVM REST framework built upon proven production JVM technologies.

Atmosphere provides server side push technology using websockets when it can and
gracefully degrades to long polling for browsers that suck.

# Running The Application

To test the example application run the following commands.

*   To package the example run.

        mvn package

*   To run the server run.

        java -jar target/dropwizard-example-0.6.2.jar server example.yml

To test chat, which purposely resides in its own directory to excercise CORS

*   Browse the file

        app/chat.html

