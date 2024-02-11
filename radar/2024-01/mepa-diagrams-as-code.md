---
title:      "Diagrams as Code"
ring:       trial
quadrant:   methods-and-patterns
tags:       [server, engine, architecture, documentation]
---

Documenting concepts and software architecture as diagrams using code offers significant benefits over heavier solutions. Treating documentation and diagrams as code and checking them into version control increases transparency, collaboration, and productivity. The textual representation of diagrams is easy to write and read, and generating graphical representations as SVG or PNG images is also straightforward with the associated tools.

### Options
- [PlantUML](https://plantuml.com/): PlantUML is an open-source tool that allows users to create UML diagrams from a plain text language. It uses simple and intuitive syntax to define diagrams, which makes it easy to version control and keep track of changes. PlantUML supports various types of diagrams such as sequence diagram, use case diagram, class diagram, activity diagram, component diagram, state diagram, object diagram, and others.
- [Mermaid](https://mermaid.js.org/), a JavaScript-based diagramming tool natively supported by many common tools (e.g., GitHub, GitLab, Gitea, Notion, etc.).
- [Drawio](https://app.diagrams.net/): Draw.io (also known as diagrams.net) is a free online diagram software for making flowcharts, process diagrams, org charts, UML, ER and network diagrams. It's an open-source, fully featured diagram editor that allows you to create and edit diagrams directly in your web browser or as a desktop application. Draw.io supports a wide range of diagram types and has strong support for creating software architecture diagrams.

**NOTE:** Drawio is not a pure code-based solution, but it is included here for its popularity and ease of use. A Drawio diagram is described as an XML document and it can be saved in a repository and versioned like any other file. 

### Usages
PlantUML is extensively used in combination with Asciidoc to include and inline PlantUML diagrams in our documentation. 

Draw.io diagrams are mostly used in Confluence documentation but there are cases where diagrams were saved in repositories as XML files and added in the documentation as exported images. 