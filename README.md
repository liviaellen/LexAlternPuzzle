

A vectorizing algorithm fits splines along the piece borders to generate a cuttable SVG.

You can grow the jigsaw manually until you're satisfied and download the result for lasercutting or whatever.

Use with caution!

PS. Nothing is uploaded anywhere, your SVG border stays in your computer!

# How to use

1. Adjust the desired generation parameters:

   * Columns and rows: in rectangular (default) jigsaw mode, these define the number of rows and columns for the piece grid
   * Grid size: regular square grid size for seeding. Seeds are planted in regular intervals every grid size cells, with some added randomness.
   * Initial grid possition noise: how much noise will be added to each seed position. Setting this parameter to 0 will place the seeds in a regular square grid.
   * Growth radius: cells will only expand up to this radius away from the seed cell. It should be set to at least 2x grid size.
   * Curve fitting threshold: higher value = the vectorizer uses more straight line segments. Lower value: less straight line segments, more jittery curves.
   * Magic number: just leave this at 6.2 ok?
   * Growth probability: each cell will grow with this probability each cycle.
   * Cell size: how a cell translates to the physical world. Each cell represents an area of size x size mm. Set to at least 2mm, better if 3 or more, so that choke points don't create too weak pieces.
   * Preview viewing scale: size of each cell in pixels for the colored preview thing.
   * Custom border scale factor: when using a custom border, this scale will be applied to the border SVG. The puzzle size will be border size x scale.
2. Want to use a custom SVG border? Use the file picker and then press Load SVG customborder.
3. Press Generate Jigsaw and wait
4. Press Grow as many times as you want until you're satisfied
5. Download SVG, check and cut.
