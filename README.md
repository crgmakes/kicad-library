# CRG Makes KiCad Library

This repo contains all the KiCad symbols, footprints, models, and other files supporting [CRG Makes](https://crgmakes.com) development within KiCad.

## Installation

To install this library, start by [cloning](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) the [CRG Makes libary](https://github.com/crgmakes/kicad-library) repo to a convienent local directory.

In this example, our local directory will be: `/Users/tom/Development/KiCad/CRGM/`. 

<div class="alert alert-info">
  <i class="fas fa-exclamation-triangle"></i> <strong>Note:</strong> Replace this value with absolute path of where you place <b><i>your</i></b> library.
</div>

Start by setting the base parameters, the schematic parameters, and finally PCB parameters.

### Set Base Parameters

Within KiCad Project viewer:

![KiCad Project Viewer](resources/images/install-1.png)

Click on Preferences->Configure Paths...

![Configure Paths](resources/images/install-2.png)

Perform the following actions:

1. Click "+" near the bottom
1. Type "KICAD_USER_LIBRARY" in the first cell
1. Paste the local location repo's root directory (i.e., `/Users/tom/Development/KiCad/CRGM/`)
1. Click "+" near the bottom
1. In the first cell, type "KICAD_USER_MODEL_DIR"
1. In the second cell, paste "${KICAD_USER_LIBRARY}/models"
1. Click "+" near the bottom
1. In the first cell, type "KICAD_USER_TEMPLATE_DIR"
1. In the second cell, paste "${KICAD_USER_LIBRARY}/templates"

Your screen should look something like this:

![Configured Paths](resources/images/install-3.png)

Click OK to save.

### Schematic

Within KiCad Schematic Editor, click Preferences->Manage Symbol Libraries...

![Configure Symbol Libraries](resources/images/install-4.png)

Add the following parameters by clicking +:

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Name</th>
      <th>Value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>CRG Makes</td>
      <td>${KICAD_USER_LIBRARY}/symbols/CRG Makes.kicad_sym</td>
    </tr>
    <tr>
      <td>CRGM Connector</td>
      <td>${KICAD_USER_LIBRARY}/symbols/CRGM Connector.kicad_sym</td>
    </tr>
    <tr>
      <td>CRGM Logos</td>
      <td>${KICAD_USER_LIBRARY}/symbols/CRG Makes.kicad_sym</td>
    </tr>
    <tr>
      <td>CRGM Labels</td>
      <td>${KICAD_USER_LIBRARY}/symbols/CRGM Labels.kicad_sym</td>
    </tr>
    <tr>
      <td>CRGM Power</td>
      <td>${KICAD_USER_LIBRARY}/symbols/CRGM Power.kicad_sym</td>
    </tr>
    <tr>
      <td>CRGM Passive</td>
      <td>${KICAD_USER_LIBRARY}/symbols/CRGM Passive.kicad_sym</td>
    </tr>
    <tr>
      <td>CRGM Symbols</td>
      <td>${KICAD_USER_LIBRARY}/symbols/CRGM Symbols.kicad_sym</td>
    </tr>
    <tr>
      <td>CRGM Switches</td>
      <td>${KICAD_USER_LIBRARY}/symbols/CRGM Switches.kicad_sym</td>
    </tr>
  </tbody>
</table>

Your parameters should look like this:

![Configured Symbol Libraries](resources/images/install-5.png)

### PCB

Within KiCad PCB Editor, click Preferences->Manage Footprint Libraries...

![Configure Footprint Libraries](resources/images/install-6.png)

Add the following parameters by clicking +:

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Name</th>
      <th>Value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>CRG Makes</td>
      <td>${KICAD_USER_LIBRARY}/footprints/CRG Makes.pretty</td>
    </tr>
    <tr>
      <td>CRGM Connector</td>
      <td>${KICAD_USER_LIBRARY}/footprints/CRGM Connector.pretty</td>
    </tr>
    <tr>
      <td>CRGM Logos</td>
      <td>${KICAD_USER_LIBRARY}/footprints/CRG Makes.pretty</td>
    </tr>
    <tr>
      <td>CRGM Labels</td>
      <td>${KICAD_USER_LIBRARY}/footprints/CRGM Labels.pretty</td>
    </tr>
    <tr>
      <td>CRGM Mechanical</td>
      <td>${KICAD_USER_LIBRARY}/footprints/CRGM Mechanical.pretty</td>
    </tr>
    <tr>
      <td>CRGM Power</td>
      <td>${KICAD_USER_LIBRARY}/footprints/CRGM Power.pretty</td>
    </tr>
    <tr>
      <td>CRGM Passive</td>
      <td>${KICAD_USER_LIBRARY}/footprints/CRGM Passive.pretty</td>
    </tr>
    <tr>
      <td>CRGM Switches</td>
      <td>${KICAD_USER_LIBRARY}/footprints/CRGM Switches.pretty</td>
    </tr>
    <tr>
      <td>CRGM Symbols</td>
      <td>${KICAD_USER_LIBRARY}/footprints/CRGM Symbols.pretty</td>
    </tr>
  </tbody>
</table>

<div class="alert alert-info">
  <i class="fas fa-info-circle"></i> <strong>Note:</strong> PCB has a mechanical footprint library without a corresponding symbol library.
</div>

Your parameters should look like this:

![Configured Footprint Libraries](resources/images/install-7.png)

### Models

You may need to manually set the model path for some footprints. You do so by opening the footprint's properties by couple clicking on the footprint in the PCB editor. 

Select 3D Models from the title bar:

![Configured Footprint Libraries](resources/images/install-8.png)

Set the value to: `${KICAD_USER_MODEL_DIR}/{your model}`

Don't for get to select "Show" or your model will not display in 3d mode.

![Configured Footprint Libraries](resources/images/install-9.png)

Happy making!
