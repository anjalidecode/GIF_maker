# Create a GIF with Python

**Python:** 3.10 | **Imageio:** 2.16.2

---

## Overview

Learn how to create animated GIFs in Python using just a few lines of code! This project combines multiple images into a GIF using the `imageio` library.

---

## Setup

Install `imageio`:

```bash
pip3 install imageio

Code
import imageio.v3 as iio

filenames = ['pic1.png', 'pic2.png']
images = [iio.imread(f) for f in filenames]
iio.imwrite('pic.gif', images, duration=500, loop=0)

How it works:
filenames: list of images
images: stores image data
iio.imwrite: creates GIF (duration in ms, loop=0 = infinite)

Run
python3 create_gif.py

The pic.gif will appear in the project folder.

Make it Yours
Use your own images
Try 3+ images
Ensure images have the same dimensions

🎉 Congrats! You now have a GIF made entirely in Python.
```
