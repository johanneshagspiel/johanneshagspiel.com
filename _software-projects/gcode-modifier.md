---
layout: software-project
title: G-Code Modifier
description: "🛠️ A desktop application created in order to support the 3D printing of sustainable materials such as chalk via extrusion through a syringe"
published: True
---

<img src= "/assets/software-projects/gcode-modifier/gcode_modifier_logo.JPG" alt="G-Code Modifier Logo" width="20%">

## G-Code Modifier ([repository](https://github.com/johanneshagspiel/gcode-modifier))

| Summary  |
| -------------------------------------------------- |
| 🛠️ A desktop application created in order to support the 3D printing of sustainable materials such as chalk via extrusion through a syringe. Such a 3D printing process posses unique problems that either can not be addressed at all with popular 3D printer slicing applications like [Cura](https://ultimaker.com/software/ultimaker-cura) or only in a very cumbersome manner. The "G-Code Modifier" itself, however, can not slice a model into G-Code as it instead modifies existing G-Code. |

## Features

The possible modifications of G-Code include:
- changing the flow rate between the first and every other layer
- changing the flow rate between the outer walls and the infill
- changing the bed temperature
- changing the print speed
- turning on the fan while printing
- pausing the print after each layer for a certain amount of time
  - and possibly retracting the syringe slightly during the pause
- cleaning the nozzle during the print (by moving to the bottom right corner, where a sponge is assumed to be installed, and moving the syringe up and down repeatedly)
- retracting the syringe at the end of the print
- supporting a larger syringe with a higher flow-rate

## Tools

| Purpose                | Name                                                         |
|------------------------|--------------------------------------------------------------|
| Programming language   | [Python](https://www.python.org/)                            |
| Dependency manager     | [Anaconda](https://www.anaconda.com/products/distribution)   |
| Version control system | [Git](https://git-scm.com/)                                  |
| Testing framework      | [unittest](https://docs.python.org/3/library/unittest.html/) |
| Application Bundler    | [PyInstaller](https://pyinstaller.org/en/stable/index.html/) |
| GUI Framework 		 | [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)   |

## Installation Process

A precompiled executable can be found with the [latest release]((https://github.com/johanneshagspiel/gcode-modifier/releases/)). 

If you want to build the application yourself, it is assumed that you have installed [Python](https://www.python.org/downloads/windows/) and that your operating system is Windows.

Open this repository in the terminal of your choice. In case `pip` has not been installed, do so via:

    py -m ensurepip --upgrade

Install `pyinstaller` with this command:

    pip install -U pyinstaller

Now, create the executable via:

    cd src | pyinstaller paste_printer/main.py --distpath "pyinstaller/dist" --workpath "pyinstaller/build"  --noconsole --add-data "paste_printer/resources/icons/*;paste_printer/resources/icons" --add-data "paste_printer/resources/gcode/0.6/*;paste_printer/resources/gcode/0.6" --add-data "paste_printer/resources/gcode/0.8/*;paste_printer/resources/gcode/0.8" --add-data "paste_printer/resources/gcode/1.5/*;paste_printer/resources/gcode/1.5" --add-data "paste_printer/resources/fonts/*;paste_printer/resources/fonts" --add-data "paste_printer/resources/settings/*;paste_printer/resources/settings"

This should have created a new folder in `src` called `pyinstaller`. The executable can be then be found at `src/pyinstaller/dist/main.exe`

If you want to import this project and resolve all the dependencies associated with it, it is assumed that you have already installed [Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html). Re-create the original `GCode-Modifier` environment from the `environment.yml` file with this command:

	conda env create -f environment.yml

Activate the new environment:
 
	conda activate GCode-Modifier

Lastly, check that the new environment was installed correctly:
	
	conda env list

## Licence

The G-Code Modifier is published under the MIT licence, which can be found in the [LICENSE](LICENSE) file.