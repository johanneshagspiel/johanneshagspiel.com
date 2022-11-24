---
layout: software-project
title: G-Code Viewer
description: "🖥️ A desktop application to visualize G-Code"
published: True
---

<img src= "/assets/software-project/gcode-viewer/gcode_viewer_logo.JPG" alt="G-Code Viewer Logo" width="20%">

## G-Code Viewer ([repository](https://github.com/johanneshagspiel/gcode-viewer))

| Summary  |
| -------------------------------------------------- |
| 🖥️ A desktop application created in order to support the manipulation of G-Code, for example by the [G-Code Modifier](https://github.com/johanneshagspiel/gcode-modifier), by visualizing the actions taken by a 3D-printer when executing a G-Code file.  |

## Features

With the "G-Code Viewer", the user can:
- move around freely in a generated 3D model representing the bed of a 3D printer and the results of a G-Code file
- analyze the actions taken by a 3D printer when executing a G-Code file in both a static and dynamic 2D layer-by-layer view

## Tools

| Purpose                | Name                                                         |
|------------------------|--------------------------------------------------------------|
| Programming language   | [Python](https://www.python.org/)                            |
| Dependency manager     | [Anaconda](https://www.anaconda.com/products/distribution)   |
| Version control system | [Git](https://git-scm.com/)                                  |
| GUI Framework 		 | [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)   |
| 3D-Model Viewer 		 | [PyQtGraph](https://www.pyqtgraph.org/)   |


## Installation Process

If you want to import this project and resolve all the dependencies associated with it, it is assumed that you have already installed [Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html), [Python](https://www.python.org/downloads/windows/), an IDE like [PyCharm](https://www.jetbrains.com/pycharm/download/#section=windows) and that your operating system is Windows.
Re-create the original `GCode-Viewer` environment from the `environment.yml` file with this command:

	conda env create -f environment.yml

Activate the new environment:
 
	conda activate GCode-Viewer

Lastly, check that the new environment was installed correctly:
	
	conda env list

## Licence

The "G-Code Viewer" is published under the MIT licence, which can be found in the [LICENSE](LICENSE) file.