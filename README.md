# Wing Image Standardization

Resources and tools for standardizing images of insect wings (cropping and persepctive correction). Under development. Contact ostwald.madeleine@gmail.com with any questions.

# Repository Directory
### Imaging Cards
Contains files for printable templates used as backdrops for wing imaging ("imaging cards"). These cards include ArUco markers, which are unique identifying shapes that are compatible with computer vision applications (fully supported in OpenCV). Framing wings in these markers allows us to automate the cropping and perspective correction process. These markers can also be used as a size reference for measurement, eliminating the need to include a ruler in these images.
We have included three image card sizes, for imaging bees (or any insects) of various sizes. For most bees, the "3mm_imaging_card" size should be appropriate, i.e., the entire wing should fit within the bounding rectangle. For the largest bees (e.g., queen *Bombus*, many *Xylocopa*), the "3mm_imaging_card_wide" version may be necessary to fit the entire wing into the bounding rectangle. For the smallest bees, the "1mm_imaging_card" may be desirable so that images can be taken at a higher zoom magnification.

![overview figure](readme_figures/overview_figure.jpg)

#### How to print, prepare, use, and modify the imaging cards
The imaging card templates are provided as PDFs that can be printed on 8.5x11" paper, and the ArUco markers should be printed at the length indicated on the card (either 3mm or 1mm). Confirm with a ruler that the length is preserved after printing. We have also provided photoshop files (.PSD) if you would like to modify the cards in any way or change the printing size. You can also assemble new cards by generating ArUco markers using this free resource: https://chev.me/arucogen/

Each print-out contains multiple stacked imaging cards that need to be individually cut out according to the directions below. Cut out a region that includes all four markers, with the measurement and "Wing" on the bottom. This serves as a reminder of which side to place the wing for imaging. The card can be cut out in a rectangle of any size, as long as all four markers are included, and the right-hand "wing" side is cut as close to the marker boundary as possible (without actuling cutting into the markers). This will allow you to place the bee flush with the edge of the card so that as much of the wing is imaged as possible.

![printout instructions](readme_figures/printout_instructions.jpg)

When imaging, align the bee with the right hand side of the marker, such that right wings will be imaged with the bee's head oriented toward the bottom of the card, and left wings will be oriented with the head facing up (see image below). Be sure to position the wing so that it fits entirely within the cropping region indicated in orange below. This is the region that will be cropped with the cropping script.

![imaging instructions](readme_figures/imaging_instructions.jpg)

### Image Cropping
Contains materials for cropping wing images, including an annotated JupyterNotebook file with the cropping script, the rendered HTML file, the rendered .MD file, and the outputted cropped test image. 

### Perspective Correction
Contains a JupyterNotebook file for correcting perspective in wing images.
