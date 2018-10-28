# tarea3
tarea 3 de métodos computacionales
from skimage import io
import matplotlib.pyplot as plt
from skimage.color import rgb2gray
from scipy import fftpack
import numpy as np
from scipy import ndimage



im = plt.imread('Arboles.png').astype(float) # imread lee las imagenes con los pixeles codificados como enteros 
# en el rango 0-255. Por eso la convertimos a flotante y en el rango 0-1
im_fft = fftpack.fft2(im)
plt.plot(im_fft)
plt.show()
