# iGaming Studio Tech Radar

[![Build Technology Radar](https://github.com/lnw-studios/tech-radar/actions/workflows/build.yml/badge.svg)](https://github.com/lnw-studios/tech-radar/actions/workflows/build.yml)

**Contents**
<!-- TOC -->
* [iGaming Studio Tech Radar](#igaming-studio-tech-radar)
  * [Tech Radar](#tech-radar)
    * [Structure](#structure)
    * [Versions](#versions)
  * [Technology Blips](#technology-blips)
  * [Project Structure](#project-structure)
  * [Development](#development)
    * [How to run the radar locally](#how-to-run-the-radar-locally)
    * [Regenerate the json file based on your changes on md files](#regenerate-the-json-file-based-on-your-changes-on-md-files)
  * [Adding a new version](#adding-a-new-version)
  * [Tech Radar Themes](#tech-radar-themes)
<!-- TOC -->

This is the source code for the iGaming Studio Tech Radar which is published under: https://igaming-studio.techradar.io/

The radar was build using the [AOE Tech Radar](https://github.com/AOEpeople/aoe_technology_radar]) and was adapted to fit the needs of the iGaming Studio org. The AOE Tech Radar is inspired by the famous [ThoughtWorks Tech Radar](https://www.thoughtworks.com/en-gb/radar) but provides a more flexible and customizable approach as well as a more modern look and feel.

## Tech Radar
### Structure
A Tech Radar is a visual representation used by organizations to assess their technology landscape. It helps in decision-making about technology choices for different purposes, such as developing new software or updating existing systems. The radar is divided into quadrants representing different areas of technology (like languages, tools, platforms, etc.). Each quadrant contains rings that indicate the level of adoption of a particular technology (like adopt, trial, assess, hold).

### Versions
The Tech Radar is versioned. Each version is a snapshot of the technology landscape at a specific point in time. The radar is updated regularly (approx. every 6 months) to reflect the current state of the technology landscape. The radar is also used to track the evolution of the technology landscape over time.

## Technology Blips
Every technology (language, framework, tool, platform, etc.) is represented by a blip on the radar. Each blip is a short description of the technology and its current status (like adopt, trial, assess, hold). The blips are organized in quadrants and rings on the radar.

Every blip should be tagged with one or more of the following tags:

**Capabilities**
* client
* server
* engine
* qa
* art

**Areas**
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

Clicking on a blip will show a detailed description of the technology and its current status.

## Project Structure
The project is a Node application and includes the `package.json` with all the available actions. 

**/radar**
The radar data are stored in the `/radar` folder and every version of the radar is stored in a separate folder with the filename format 
being as "yyyy-MM". 

The radar data is stored in markdown files which are then converted into a JSON file that is used by the radar application.
The markdown file for a blip is:

```
---
title:      "Java"
ring:       adopt
quadrant:   languages-and-frameworks
tags:       [server,qa,coding]
featured:   true
---

Java is a high-level, class-based, object-oriented programming language that is designed to have as few implementation dependencies as possible. It is a general-purpose programming language intended to let application developers write once, run anywhere (WORA), meaning that compiled Java code can run on all platforms that support Java without the need for recompilation. Java applications are typically compiled to bytecode that can run on any Java virtual machine (JVM) regardless of the underlying computer architecture. The syntax of Java is similar to C and C++, but it has fewer low-level facilities than either of them.

### Usages
* GDM Platform
* Engine Development
* GDM Tools
* Automated Testing
```

**/public**
The public folder is used for overriding the default behaviour provided by the AOE Tech Radar. For more infomration 
about the various possibilities, please refer to the AOE Tech Radar.

## Development

### How to run the radar locally
To do this, you need to have Node.js installed on your machine. You can download it from [here](https://nodejs.org/en/download/).
Then you must run the **start:static** script to build the radar and serve it as a static website. After the build, the 
radar is available at http://localhost:8080/.

The script will also generate the **build** folder which contains all the generated static files.

If you have defined a specific sub-path for your URL (see the build.yml) then add that when you navigate from the browser.
For example, this is a valid path for the deployed radar.

```
env:
  REACT_APP_RADAR_NAME: "Studios Tech Radar"
  PUBLIC_URL: "/tech-radar/"
```

### Regenerate the json file based on your changes on md files
```
npm run generateJson
```

You can do this while the server is running.
You can find the newly created rd.json in "/build/rd.json". 

## Adding a new version
To add a new version, a new folder must be added to the `/radar` folder with the filename format being as "yyyy-MM".

If a new technology was introduced, then a new markdown file must be added to the new version folder. The markdown file must contain the following structure:

```
---
title:      ""
ring:       adopt/trial/assess/hold
quadrant:   languages-and-frameworks
tags:       []
---

Description of the technology

### Usages
Usages of the technology
```

If a technology was changed, then a markdown file must be added to the new version folder.

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
