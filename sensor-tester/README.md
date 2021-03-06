# Sensors tester

This web application allows to test functionality of the sensors, for example, whether the sensor:

- model copmply with specification
- is implemented or supported by the hardware
- provides expected measurement values

![Alt text](../images/sensor-tester.png?raw=true "Sensor tester")

## Getting Started

Make sure you have following dependencies installed:

 + [Node.js](https://nodejs.org)
 + [Polymer CLI](https://www.npmjs.com/package/polymer-cli) ``` npm install -g polymer-cli ```
 + For deployment to Google App Engine, install [SDK for App Engine](https://cloud.google.com/appengine/downloads).

## Install NPM dependencies

Install polymer components that are required for the project.

```
npm install
```

## Viewing Your Application

```
polymer serve
```

This will serve application locally. By default, port 8080 will be used (http://localhost:8080/).

## Building Your Application

```
polymer build
```

This will create a `build/` folder with `bundled/` and `bundled_appspot/` sub-folders
containing a bundled (Vulcanized) builds, both run through HTML, CSS, and JS optimizers.
The `bundled/` folder contains application that is supposed to be served from
`generic-sensor-demos/sensor-tester/build/bundled/` base path, so it is easy to test the
app from the GitHub pages. The `bundled_appspot/` folder contains app that can be served
from the root base path, for example, when served from the Google App Engine.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
polymer serve build/bundled_appspot
```

## Deploying to App Engine

```
gcloud app deploy app.yaml -v VERSION --project PROJECT_NAME
```

 + VERSION should be the version of your application, if omitted, it will be autogenerated.
 + PROJECT_NAME should be the name of App Engine project.

You could check demo of the web application at https://sensortestapp.appspot.com/ or
pre-built [application here](https://intel.github.io/generic-sensor-demos/sensor-tester/build/bundled/)

## Testing on device

For testing tips'n'tricks, please check
[Development environment](https://intel.github.io/generic-sensor-demos/) section.