# JPG_to_UIUC_colors
Recreated input jpg image in UIUC colors

Converts an input .jpg file, quantizes it to UIUC colors, and applies Atkinson dithering. Includes optional downsampling of input image before quantization.

To save time during quantization, instead of finding the nearest UIUC color for a given pixel directly, nearest color values for 24-bit depth rgb have been precomputed.
These precomputed nearest values have been stored in 'color_array_ui.npz. This file should be stored in the same directory as the script itself.
Otherwise, its location can be passed as an arguement when running the script.

For quantization and dithering, the script uses the following official UIUC colors:

U of I Blue (RGB: 19/41/75)
Urbana Orange (RGB: 232/74/39)

Plus an additional white "neutral" color (RGB: 232/233/234)
