# Foraging example

This is the foraging example used in the RoboCert paper.
It is laid out as follows:

- `*.rct` files are RoboChart input.
- `*.rcert` files are RoboCert input; one file per specification group
  (ie. one per target).
- `representations.aird` is the Sirius representations file for the RoboChart
  input, used for graphical viewing and editing of that input.

To use this project (assuming you have both RoboChart and RoboCert tools
installed):

1. Open this directory as a project in Eclipse.
2. Edit and save the `*.rcert` files you want to generate (there is currently
   no action for manually regenerating the CSP output).
3. In `csp-gen/timed/robocert/pkg`, corresponding `.csp` files will appear.
   Open these in FDR4 or `refines` to check assertions.
4. If there are any mentions of missing CSP files, try pressing the
   cog icon next to 'CSP' in the toolbar to generate CSP for the RoboChart
   models.
