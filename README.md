🎬 Create an Animated GIF with Python 🐍

## 🌟 Overview

Combine multiple images into a smooth, looping GIF animation using Python and the `imageio` library.

## 🛠️ Setup

Install the required library by running:
pip3 install imageio

## 💻 Code Example

import imageio.v3 as iio

### List your image filenames here

filenames = ['pic1.jpeg', 'pic2.jpeg']

### Load images into a list

images = []
for filename in filenames:
images.append(iio.imread(filename))

### Create and save GIF

### duration=500ms per frame, loop=0 means infinite loop

iio.imwrite('pic.gif', images, duration=500, loop=0)

## 🚀 Instructions

1. Edit the `filenames` list with your own images 🖼️
2. Make sure all images have the same dimensions 📏
3. Save the code as `create_gif.py`
4. Run the script with:
   python3 create_gif.py
5. Your animated GIF `pic.gif` will be created in your folder 🎉

## 💡 Tips & Tricks

- Add more images for longer animations ➕
- Adjust `duration` to speed up or slow down frame delay ⏱️
- GIF loops infinitely by default 🔁

🎊 Congratulations! You've created a GIF using Python and `imageio`!
