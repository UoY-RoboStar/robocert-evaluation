# Evaluation artefacts for RoboCert

This repository contains snapshots of the various RoboCert artefacts, for use in evaluating:

- the tool (in the form of RoboCert plugins for Eclipse);
- a case study (the foraging robot of Buchanan et al.).

The reference manual is [elsewhere](http://robostar.cs.york.ac.uk/publications/reports/robocert.pdf).

## NOTE

As of writing (2022-05-08), the contents of this repository are provisional; the
plugins have not yet been tested outside of the environment in which their zip
was created, and the case study may need some tidying up to reflect the latest
paper draft.  These will happen as soon as possible.  Apologies for the
inconvenience caused.

## Contents

- `robocert.zip`: zip of Eclipse plugin JARs
- `foraging/`: foraging case study (see enclosed README).

## Prerequisites

To install the tool, you will need:

- Eclipse (tested with 2022-03);
- RoboTool version 3 (tested with CSP generator v3.0.0.202202010017; we recommend installing all plugins);
- RoboTool's prerequisites (for instance, Epsilon);
- (**TODO: check**) the Eclipse Plugin Development Environment.

You do not need Sirius and the RoboTool graphical editors to get RoboCert working
(and, indeed, at time of writing, there have been a few issues in getting things
to line up with these).  However, if these are installed, it will be easier to
validate that the RoboChart models in `foraging` match their descriptions in the
paper.

### Installing the RoboCert plugins

**NOTE:** This workflow has not been tested yet.

1. Acquire an Eclipse installation with the prerequisites installed.
2. Extract `robocert.zip` somewhere readable by Eclipse.
3. In Eclipse, right click the package explorer, and pick _Import_.
4. In the _Import_ dialog, select _Plug-in Development > Plug-ins and Fragments_.
5. In _Import From_, select _Directory_ and then the directory containing the extracted contents of `robocert.zip`.
6. Select _Import As Binary projects_.
7. Select _Add All ->_, and _Finish_.
