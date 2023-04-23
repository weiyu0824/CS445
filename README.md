# Editing image using seam-carving
The seam carving code is adapted from https://github.com/andrewdcampbell/seam-carving

## Requirements
- OpenCV
- scipy
- numba
- numpy

## Usage
- `-body`: mode for editing human image
- `-vis`: visualize the seam carving process
- `-im`: edited image path
- `-out`: output image path
- `-bmaks`: body mask (place you wan't to remove or increase) 
- `-mask`: protective mask (place you don't want to remove).
- `-dx`: number of seam going to removed
```
    python seam_carving.py -body -vis -im [image_path] -out [output_path]  -bmask [body_mask_path] -mask [mask_path] -dx [# removed seams]
```

### Example
- Bikini Example:
```
python3 seam_carving.py -body -vis -im images/bikini/bikini.jpg -out bikini_thin.jpg -bmask images/bikini/bikini_mask_2.jpg -mask images/bikini/bikini_mask_1.jpg -dx -30
```

## Methods


