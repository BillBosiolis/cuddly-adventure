# iGaming Studio Tech Radar

[![Build Technology Radar](https://github.com/lnw-studios/tech-radar/actions/workflows/build.yml/badge.svg)](https://github.com/lnw-studios/tech-radar/actions/workflows/build.yml)

**Contents**
<!-- TOC -->
* [iGaming Studio Tech Radar](#igaming-studio-tech-radar)
  * [Content Guidelines](#content-guidelines)
    * [Capabilities](#capabilities)
    * [Topics](#topics)
  * [Development](#development)
    * [Host the application under a sub path](#host-the-application-under-a-sub-path)
    * [Build the radar](#build-the-radar)
    * [Build the radar with static files](#build-the-radar-with-static-files)
    * [Regenerate the json file based on your changes on md files](#regenerate-the-json-file-based-on-your-changes-on-md-files)
  * [Tech Radar Themes](#tech-radar-themes)
<!-- TOC -->

This is the source code for the iGaming Studio Tech Radar which is published under: https://igaming-studio.techradar.io/

If you want to build your own techradar you may want to have a look at https://github.com/AOEpeople/aoe_technology_radar instead.

This is based on https://github.com/AOEpeople/techradar which turn is based on the famous [ThoughtWorks Tech Radar](https://www.thoughtworks.com/en-gb/radar).

## Tech Radar Structure
TBC

## Content Guidelines

New blips should be tagged. The following tags are currently established:

### Capabilities
* client
* server
* engine
* qa
* art

### Topics
* architecture
* security
* devops
* agile
* coding
* ci/cd
* documentation
* testing
* monitoring
* deployment
* database

e.g. use like this:

```md
tags: [devops, security]
```

## Development

### Host the application under a sub path
To host the application under a sub path, set the environment variable `PUBLIC_URL`, e.g. "/techradar".
The default is `/`.

> For local development I recommend using `/build` and use this for the following steps.

### Build the radar
```
npm i
PUBLIC_URL=/build npm run start
```

Then open here: http://localhost:8080/build

### Build the radar with static files
```
npm i
PUBLIC_URL=/build npm run start:static
```

Then open here: http://localhost:8080/build

### Regenerate the json file based on your changes on md files
```
npm run generateJson
```

You can do this while the server is running.
You can find the newly created rd.json in "/build/rd.json". 

## Tech Radar Themes
The default implementation comes with a predefined theme. 

If you want to change the theme and use different colors for the site background as well as the quadrants, you can do so by:



To change the background and text color of the four quadrants, you have to edit the `src/config.json` file.
```
"quadrantsMap": {
  "languages-and-frameworks": {
    "colour": "#84BFA4",
    "txtColour": "#444444",
    "position": 1,
  },
  "methods-and-patterns": {
    "colour": "#248EA6",
    "txtColour": "white",
    "position": 2,
  },
  "platforms-and-aoe-services": {
    "colour": "#F25244",
    "txtColour": "#444444",
    "position": 3,
  },
  "tools": {
    "colour": "#F2A25C",
    "txtColour": "white",
    "position": 4,
  }
},
```
