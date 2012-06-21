# 1962 Instructions

## Architecture and files

The project contains:

- README
- INSTRUCTIONS.md
- CONTRIBUTORS
- PIECE
- /media
- /extra

### README.md

Summary of the project used for the GitHub project homepage and the project website. This file follows the [Markdown](http://en.wikipedia.org/wiki/Markdown) syntax.

### INSTRUCTIONS.md

The file you are reading now. It explains the project and how to participate. This file follows the [Markdown](http://daringfireball.net/projects/markdown/syntax) syntax.

### CONTRIBUTORS

List of the contributors to the project. To write / edit this file, see *Syntax*.

### PIECE

Source code of the physical sculpture 1962. In this file are depicted and documented all the objects which constitute a sculpture version and all the informations about the sculpture version itself.

### /media

Folder containing images of the current state of the piece and archives of past versions. This folder must be updated at least with photographs of the sculpture for each versions.

In /media, documents must be named using the tag of the last commit. For example: 0.jpg will be a photograph of the version 0 of 1962 ; 2_5.ogg can be a video capture of the version 2.5 of 1962…

A /media/HD (optional) subfolder can contain high-definition documents. This folder will be used to make media loading easier on a project web page. In this folder, documents must be named using the tag of the last commit + "HD". For example: 0_3HD.jpg.

### /extra

Folder (optional). It can be used as an addenda, an annexe or the archive of complementary documents such as process pictures, drawings films…

## Syntax

1962's files CONTRIBUTORS and PIECE follow a couple of simple syntaxic rules:

### Basics

- Use the format "Key: value"
- Parentchip relationship are symbolised using indentation (hit [tab](http://en.wikipedia.org/wiki/Tab_character) key at the begining of a line). Demonstration:

        Name: Floral foam brick
        Size
            Width: 22,5cm
            Height: 10,6cm
            Depth: 8cm

- A line can't stay empty
- A line must begin with a capital letter
- A line can contain a title or a couple "key: value"

### Main informations

Details to understand the PIECE file:

    *     = Required informations
    //    = Comments
    Text: = Needs a value
    Text  = Is a title

The PIECE file template:

    Title: 1962
        Project curator: * // Name of the owner of the project
        Repository URL: * // Ex.: https://github.com/raphaelbastide/1962
        Physical location
            Latitude: *
            Longitude: *
            Altitude:
            City:
            Country: *
        Sculpture surface // in centimeters (cm)
            Width: *
            Height: *
            Depth:
        Position of the origin: * // Free description of a point. Each object's position will be relative to this point
        Capture hardware
            Type: // Can be photographic, video, video stream, drawing, 3D capture…
            Model: // free description
            X position: // Relative to the given origin
            Y position:
            Z position:
            Dirrection: // Can be a free description or more precise
        Lighting hardware
            Natural // or, if artificial:
            X position: // Relative to the given origin
            Y position:
            Z position:
            Dirrection: // Can be a free description or more precise
        Objects *
            ID: * // Define the identifier for the object - First one must be 1, then 2, 3…
                Name: * // A name of the object
                Size
                    Width: *
                    Height: *
                    Depth: *
                Position
                    X position: * // Relative to the given origin
                    Y position: *
                    Z position: *
                    Position description: // Free description of the position
                Color / texture:
            ID: 2 // Here can begin a second object description
                Name: 
                ...
                
### Evolutions of this INSTRUCTIONS file

This INSTRUCTIONS file can and must envolve. I should be modified in order to accompany the PIECE file. For example if a new kind of object needs the creation of a new kind of key (property), it needs to be archived below:

#### Mode

Electric or mechanical hardware can have one or multiple status, in this case a key "Mode" will be specified with values such as "On", "Off", "Blink"…

    Mode: On

#### Nutrients

Plant or animals needs water or food to live, a key "Additional water" or "Additional food" can be created, with scalable values such as units "|". Exemple for four water additions:

    Additional water: ||||