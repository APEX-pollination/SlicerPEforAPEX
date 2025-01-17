
![Slic3rPE logo](/resources/icons/Slic3r.png?raw=true)

# Slic3r Prusa Edition (modified for use in APEX pollination's 3D-printing factory)

### This repository contains a slight modification of PRUSA SlicerPE. These modifications include printing profiles for CREALITY CR10 max printers, and a modified Honeycomb fill pattern to print foundation sheets for honeybees.

Prebuilt Windows, OSX and Linux binaries are available through the [git releases page](https://github.com/prusa3d/Slic3r/releases).

Slic3r takes 3D models (STL, OBJ, AMF) and converts them into G-code
instructions for FFF printers or PNG layers for mSLA 3D printers. It's
compatible with any modern printer based on the RepRap toolchain, including all
those based on the Marlin, Prusa, Sprinter and Repetier firmware. It also works
with Mach3, LinuxCNC and Machinekit controllers.

See the [project homepage](https://www.prusa3d.com/slic3r-prusa-edition/) and
the [documentation directory](doc/) for more information.

### What language is it written in?

All user facing code is written in C++, and some legacy code as well as unit
tests are written in Perl. Perl is not required for either development or use
of Slic3r.

The slicing core is the `libslic3r` library, which can be built and used in a standalone way.
The command line interface is a thin wrapper over `libslic3r`.

### What are Slic3r's main features?

Key features are:

* **multi-platform** (Linux/Mac/Win) and packaged as standalone-app with no dependencies required
* complete **command-line interface** to use it with no GUI
* multi-material **(multiple extruders)** object printing
* multiple G-code flavors supported (RepRap, Makerbot, Mach3, Machinekit etc.)
* ability to plate **multiple objects having distinct print settings**
* **multithread** processing
* **STL auto-repair** (tolerance for broken models)
* wide automated unit testing

Other major features are:

* combine infill every 'n' perimeters layer to speed up printing
* **3D preview** (including multi-material files)
* **multiple layer heights** in a single print
* **spiral vase** mode for bumpless vases
* fine-grained configuration of speed, acceleration, extrusion width
* several infill patterns including honeycomb, spirals, Hilbert curves
* support material, raft, brim, skirt
* **standby temperature** and automatic wiping for multi-extruder printing
* [customizable **G-code macros**](https://github.com/prusa3d/Slic3r/wiki/Slic3r-Prusa-Edition-Macro-Language) and output filename with variable placeholders
* support for **post-processing scripts**
* **cooling logic** controlling fan speed and dynamic print speed

### Development

If you want to compile the source yourself, follow the instructions on one of
these documentation pages:
* [Linux](doc/How%20to%20build%20-%20Linux%20et%20al.md)
* [macOS](doc/How%20to%20build%20-%20Mac%20OS.md)
* [Windows](doc/How%20to%20build%20-%20Windows.md)

### Can I help?

Sure! You can do the following to find things that are available to help with:
* Add an [issue](https://github.com/prusa3d/Slic3r/issues) to the github tracker if it isn't already present.
* Look at [issues labeled "volunteer needed"](https://github.com/prusa3d/Slic3r/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue+label%3A%22volunteer+needed%22)

### What's Slic3r license?

Slic3r PE is licensed under the _GNU Affero General Public License, version 3_.
The Prusa Edition is originally based on Slic3r by Alessandro Ranellucci.

The [Silk icon set](http://www.famfamfam.com/lab/icons/silk/) used in Slic3r is
licensed under the _Creative Commons Attribution 3.0 License_.
The author of the Silk icon set is Mark James.

### How can I use Slic3r PE from the command line?

Please refer to the [Command Line Interface](https://github.com/prusa3d/Slic3r/wiki/Command-Line-Interface) wiki page.
