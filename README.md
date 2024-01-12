# SummaryDo 

![summarydos](https://user-images.githubusercontent.com/71225087/93237337-a390a500-f788-11ea-954f-a8b8f5b7b729.jpg)

## Contents
* [The Vision](#the-vision)
* [Summary](#summary)
* [Algorithms](#algorithms)
* [Code](#code)
* [Chrome Extension](#chrome-extension)
* [Design](#design)
* [API](#api)
* [Future Look](#future-look)
* [How to Run the Extension](#how-to-run-the-extension)
* [Demo Video](#demo-video)

## The Vision

A program that can summarize any product page into a small, simple, and informative design with a few sentences. This summary can be read or listened to, aiding various people during browsing in different ways.

## Summary 

![summary logo](https://user-images.githubusercontent.com/71225087/93217463-c6fc2580-f771-11ea-9a33-df3a6548c8e6.png)

The model will summarize a web page text after shading it. Post-summarization, a voice will read the new text to the browsers, enabling customers to save time and effort. It also helps elders or people with disabilities to have a great experience.

* Until now, it can only speak English.
* The model can deal with any webpage, such as Wikipedia articles, and item descriptions on Amazon, all in one click.

## Algorithms

### TextRanking Algorithm (NLP)
This algorithm links all the text in the articles, then splits the whole text into individual sentences. Every sentence finds a vector representation. Similarities between sentence vectors are calculated and stored in a matrix. The similarity matrix is converted into a graph, with sentences as vertices and similarity scores as edges, for sentence rank calculation, leading to the final summary.

## Code

Written in Python.

#### Importing the Required Libraries (Lines 1-5)

* `stop_words`: A set of default stop words for the English language model in Spacy, an open-source library for NLP in Python.
* `string module`: Contains functions related to strings.
* `punctuation`: A string of ASCII characters considered punctuation characters.
* `flask`: Used for web development issues.
* `heapq.nlargest`: Returns a list with the n largest elements from the dataset.

![background](https://user-images.githubusercontent.com/71225087/93233936-56123900-f784-11ea-9b56-937eb796e593.png)

#### Step-by-Step Explanation (Lines 8-58)

* Using stop words.
* Defining a function for summarization (NLP).
* Vector representation of sentences (extraction).
* Creating vectors for the sentences.
* Fetching vectors.
* Summary extraction.

#### API Fitting (Lines 61-84)

## Chrome Extension 

The Chrome extension was written in JavaScript and HTML. The design is simple to satisfy the user experience, placing a superb impact. After opening the extension, the user will shade the specific text, and then the new summarized text will be ready for the reader.

## Design

The main goal:
* Catching attention with preservation to eye relaxation.
* Simplicity.
* Clear typography.

![summ](https://user-images.githubusercontent.com/71225087/93319473-91f6de00-f818-11ea-87f5-25347656a967.jpg)

Color: Black & Orange, Wording: Killer Brief, Logo: Matchless, representing the idea.

## API 

It is a computing interface defining interactions between multiple software, in our case, a web page and the Python program. Using Flask and JSON, we had the potential to connect them together.

## Future Look 

Looking ahead, new trends continue to emerge and merge. Project development (AI & deep learning) will lead to expansion through every website, e-commerce websites, allowing customers to enjoy browsing.

A new algorithm that can summarize in a smart way, recognizing the subject or category of the text, resulting in better summarization. It would be able to summarize a text giving more weight to the sentences related to its subject, such as speed, LAN ports, technology generation, range for a router.

Likewise, on other products (sports, clothing, gaming, furniture, etc.), it can also be a scientific article.

![SummaryDo](https://user-images.githubusercontent.com/71225087/93099323-8ee0de00-f6b0-11ea-9a38-010bbf37aca2.jpg)

## How to Run the Extension

- Download the files from the repository.
- Upload the "chrome extension" folder as an unpacked chrome extension to Chrome.
- Highlight the text that you want to summarize on any webpage.
- Click the icon of the extension to see and listen to the summary.
- You don't have to run the main.py file because we already deployed the Flask API to pythonanywhere.com.

## Demo Video

Watch the demo video [here](https://drive.google.com/file/d/1DPDNV0x_qsAKNBlwz24GVHVq7EJYC5M/view?usp=sharing).
