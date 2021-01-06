# numba-convolutional-smoothing
A small demonstration of the power of Numba to speed up mathematical calculations in Python.

## installation of dependecies

Create environment:

```python3 -m venv ./venv```

Activate environment:

```source ./venv/bin/activate```

Install dependencies:

```pip install -r requirements.txt```



https://livebook.manning.com/book/geoprocessing-with-python/chapter-11/77
11.2.2. Focal analyses
Focal analyses use the pixels that surround the target pixel in order to calculate a value. For a given cell in the output, the value is calculated based on the corresponding cell and its neighbors in the input dataset. This is also called a moving window analysis because you can think of it as “window” of cells centered on each pixel in turn. Once the value for the target pixel is calculated, the window moves to the next pixel. Figure 11.3 shows how a 3 x 3 window would “move” across an image. The output values of the dark pixels are calculated using the nine surrounding lightly-shaded input pixels. These types of operations are common for smoothing data and removing random noise. In fact, you’ve probably used similar filters to touch up your own digital photos. Focal analyses can also be used for anything else that requires input from surrounding pixels, such as computing slope and aspect for an elevation dataset.
