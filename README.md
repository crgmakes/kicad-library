# CRG Makes KiCad Library

This repo contains all the customized KiCad symbols, footprints, models, and other files supporting development within KiCad.

## Installation

To install this library, start by [cloning](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) the CRG Makes libary repo to a convienent local directory.

In this example, we will use: /Users/tom/Development/KiCad/CRGM/

## Basics

Within KiCad Project viewer, perform the following actions:

1. Preferences->Configure Paths
1. Click "+" near the bottom
1. Type "KICAD_USER_LIBRARY" in the first cell
1. Paste the local location repo's root directory (i.e., /Users/tom/Development/KiCad/CRGM/)
1. Click "+" near the bottom
1. In the first cell, type "KICAD_USER_MODEL_DIR"
1. In the second cell, paste "${KICAD_USER_LIBRARY}/models"
1. Click "+" near the bottom
1. In the first cell, type "KICAD_USER_TEMPLATE_DIR"
1. In the second cell, paste "${KICAD_USER_LIBRARY}/templates"
1. Ensure your KiCad 3rd Party library is set to KICARD_USER_LIBRAY as well, as shown below.

   > KICAD9_3RD_PARTY	${KICAD_USER_LIBRARY}

<div class="alert alert-info">
  <i class="fas fa-info-circle"></i> <strong>Note:</strong> Ensure your KiCad version is correct in the 3rd party library variable.
</div>

## Schematic

Within KiCad Schematic Editor, click Preferences->Manage Symbol Libraries, and add:

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

## PCB

Within KiCad PCB Editor, click Preferences->Manage Footprint Libraries, and add:

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