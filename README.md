# LADUMA sky models

Deep sky model for LADUMA calibration and continuum subtraction

Construction (L-band):

- Ten blocks were processed up to 2GC stage with oxkat.
- The self-calibrated data were jointly imaged with wsclean (16 sub-bands, robust -0.5)
- A locally-thresholded (MakeMask / breizorro) cleaning mask was created.
- Data were jointly imaged with mask in place.
- Second mask was created from thresholded residual image to roll-in more faint sources.
- Masks were merged, artefacts were manually excised and some missed faint sources (mainly around the problem source) were manually added.
- Data were jointly imaged with final mask down to a threshold of 1 uJy.
