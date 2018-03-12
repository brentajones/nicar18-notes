# How to find reporting leads and publishable facts in text data you already have

[Slides](http://www.bit.ly/nlp-car18) | [Examples](http://bit.ly/nlp-car18-examples)

* Jeff Ernsthausen
* Jeremy Merrill
* Youyou Zhou

##### Description

Let's discuss some published projects that have extracted useful, newsy information from big piles of text data — so you can use similar techniques. We'll walk you through real-world examples of every step of the process: gathering text data, dividing it into chunks the computer can understand, analyzing it with fancy or simple techniques and the challenges you'll face in analyzing, bulletproofing and presenting what you find. This session isn't quite a hands-on, but the panelists will discuss the tools, practical techniques and tricks they used to transform giant piles of text into publishable insights and reporting leads. These techniques are often called "natural language processing," but we're going to keep it practical: no obscure mathematical formulas, guaranteed!

## Notes

What kinds of insights can you get? What sorts of text do you have (or can get)?

### Example insights

* Patterns across documents — which documents are most similar to documents you already know are interesting.
* Outliers — What's distinctive about some documents compared to others
* Extract meaning — topic/sentiment

Example: Extract motivation and mentions of killer's race from 141 hours of TV coverage

Example: Database of more than 100,000 disciplinary documents of doctor misconduct, model to tag them and statistically estimate liklihood.

Example: Press releases of government representatives — similar to other legislators, distinctive topics, policy priorities.

### Pipeline (How)

1. Getting the data
2. Dividing it up
3. Analyzing
4. Bulletproofing
5. Presentation

### 1. Getting data is harder than it sounds

Some sources:

* Readily available (Speeches, academics, libraries)
* APIs
* Scraping
* Speech to text
* FOIA

### 2. Dividing it up

* Cleaning
	* OCR
	* Filtering stuff out like documents in other languages
	* Lowercasing, punctuation, stripping HTML, bylines, etc.
* Tokenization (words -> columns)
	* "this is not comprehensible to the computer" -> ["this", "is", "not", "comprehensible", "to", "the", "computer"]
* Stemming/lemmatization & part-of-speech tagging
* Remove stopwords and meaningless words

DocumentCloud

### 3. Analysis

Counting words
TFIDF (Term Frequency Inverse Document Frequency)
Keyword
Clustering
Sentiment
Vectorization

Cleaning data and removing stop words = senator's most common words were his last name and "previous_article"

Vectorization = give it lots of documents, it'll figure out which words appear in similar contexts

Can ask analogies like "what is the Republican version of what the Democrats call an estate tax".

### 4. Bulletproofing

Bulletproofing doctor's harassment reports: Periodically check whether predictions were useful. Randomly select documents with low scores and read those. Be aware of whether you've unintentionally biased your algorithm. False negatives are ok, false positives are unacceptable.

Beware of external factors: One stylebook requires "spokesperson", one requires "spokesman/spokeswoman".

### 5. Presenting and visulization

Bar charts, bubbles, heat maps. Small multiples. 

No word clouds. (exception: Street name visualization)

## Questions

Story planning process: Incremental process.

People start coming to you with every pile of text. Use the easiest tool that will get the job done (DocumentCloud).

Initial loading step: figure out what you actually need from the data. When dealing with large amounts of data, just moving it around can take a long time. Paring it down can be helpful.

What do you want to do with this next: JM - Integrate it into search engine (e.g. search for estate tax, also get stuff related to death tax). 

##### Speakers

Jeff Ernsthausen is a data reporter at the Atlanta Journal-Constitution. He previously interned at The Nation and Harper's Magazine.

Jeremy is a news apps developer at ProPublica. He likes scraping data that's hard to get, maps and public records. He lives in Atlanta, Georgia. He works on a variety of open-source newsroom tools like Tabula, Stevedore and FOIA Lawya. 

Youyou Zhou is a visual journalist at Quartz. She digs into data, writing stories, designing visuals and building interactives out of it. Youyou has a keen interest in the global transfer of knowledge and text data. She is a Mizzou alum and has previously built interactives and election apps for The Associated Press. [@zhoyoyo](https://twitter.com/zhoyoyo)

*Description and speakers from [official schedule](https://www.ire.org/events-and-training/event/3189/3545/)*