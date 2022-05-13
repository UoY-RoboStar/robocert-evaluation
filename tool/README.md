# Tool snapshots for RoboCert v0.1.0

Integration of RoboCert with the RoboTool update sites is forthcoming.
Until then, you can install snapshots of the RoboCert tooling using the
subdirectories of this directory.

## Prerequisites

- Java 17;
- Eclipse (2021-12 preferred, 2022-03 may work but is not well-supported,
  recent older versions may also work);
- RoboTool version 3 (tested with CSP generator v3.0.0.202202010017; we
  recommend installing all plugins);
- RoboTool's prerequisites (for instance, Epsilon - you will likely need to
  install Epsilon _before_ RoboTool, and uncheck the 'contact all software
  sites' setting, to avoid issues with installing the Epsilon dependencies).

## Method

- Install RoboChart and its dependencies first.
- Clone this repository somewhere locally.
- Select `Help > Install New Software...`, then `Add...`, then `Local...`.
- Select the `metamodel` directory.
- Select the `RoboCert` category for installation, then `Next >`, and
  proceed as with normal Eclipse software installs.  Make sure to accept
  unsigned software (we do not sign RoboCert yet).
- On restarting the IDE, repeat the process, but for the `textual` directory.
- To test the installation, open a `.rcert` file; you should see syntax
  highlighting, and modifying the `.rcert` file should cause the generation
  of CSP-M files under the `csp-gen/timed/robocert/pkg` directory.  Make
  sure you use RoboTool to generate CSP-M for the RoboChart files before
  trying to open the RoboCert-generated CSP.
