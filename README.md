# WordCloud
Word cloud with Machado de Assis books

<p align="center">
  <img src="https://user-images.githubusercontent.com/56649205/84083088-59449e80-a9b7-11ea-9ed2-621a560713c3.jpg">
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
5) Delete stopwords, punctuations and more with [nltk stopwords](https://www.nltk.org/book/ch02.html) and *Analisando a frequência das palavras* script (see my version of [portuguese stopwords](https://github.com/luiseduardobr1/WordCloud/blob/master/portuguese_stopwords))
6) After filter the words just run *Word Cloud* script (for [more examples](https://amueller.github.io/word_cloud/auto_examples/index.html)

## Machado de Assis - Sources
**Books:** Dom Casmurro, Esaú e Jacob, Histórias sem data, Mão e a luva, Memorial de Ayres, Memórias Póstumas de Brás Cubas, Papeis Avulsos, Poesias Completas e Quincas Borba. 

[Machado de Assis - Gutemberg Project](http://www.gutenberg.org/ebooks/author/9685)
