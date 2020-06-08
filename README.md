# WordCloud
Word cloud of some Machado de Assis books

<p align="center">
  <img src="https://user-images.githubusercontent.com/56649205/84075676-ecc3a280-a9aa-11ea-8750-836fcdcd9d9d.jpg">
</p>

## Requirements
* [OpenCV](https://pypi.org/project/opencv-python/)
* [Numpy](https://numpy.org/)
* [Matplotlib](https://matplotlib.org/)
* [Nltk](https://pypi.org/project/nltk/)
* [Wordcloud](https://amueller.github.io/word_cloud/)
* [PIL](https://pypi.org/project/Pillow/)

## Steps
1) Get the image that will be the contour of the words
2) Delete the image's background
3) Run *Criando a máscara* script (in [Python Code](https://github.com/luiseduardobr1/WordCloud/blob/master/MachadoPython.ipynb)) changing the filename:
```Python
# Open image
img = cv2.imread('machado_burned.jpg')
...
```
4) Now we have a photo similar to [machado mask](https://github.com/luiseduardobr1/WordCloud/blob/master/machado_mask.jpg)
5) Delete stopwords, punctuations and more with [nltk stopwords](https://www.nltk.org/book/ch02.html) and *Analisando a frequência das palavras* script. 
