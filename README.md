# Meteo Webcam Analysis

The goal of this project is to analyze webcam capture images from [meteo.physic.ut.ee](https://meteo.physic.ut.ee/) and practice applying different analysis methods on the data. 
All images used here are downloaded from the [archive](https://meteo.physic.ut.ee/webcam/uus/archive/). Thank you to the Laboratory of Environmental Physics in University of Tartu (Institute of Physics) for keeping this archive open and free to use.

## Ideas
- Skies only (top 310 pixels).
- Cars in the parking lot.
- Weather, duration of days, light.
- People.
- Lights in the buildings.

Video clips of the archived footage can be found in the same location as the images, or in the form of a timelapse: [2019](https://youtu.be/q_ZRND_3uQY) and [2020](https://youtu.be/9cNdEs1fOOQ).

## Files

Raw image files (in .jpg) are accessible at the archive, linked above. I would suggest to use the `--wait` option (if using wget) with at least 2-3 seconds in order to keep the server stress-free.

For the skies only dataset, I have uploaded a 5x downscaled version for the years 2019 and 2020 [here](https://owncloud.ut.ee/owncloud/index.php/s/baF67777B4FTrMC), for a total of 17537 images in 256x62.

All of the code is contained in the Jupyter notebook file `meteo_webcam_analysis.ipynb`.

## Requirements

Language: `Python 3.8+`

Libraries used:
- numpy
- matplotlib
- opencv-python (cv2)
- pillow (PIL)
- _tensorflow_
- _sklearn_