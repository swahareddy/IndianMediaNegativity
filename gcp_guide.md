I enthusiastically started with GCP since I am comfortable with connecting to it due to my project at work. And also, I am no ML, NLP expert and Google's APIs let any chomu do cool NLP stuff.
 
How are we getting all this? Google cloud gives developers 300$ of credits for one year. I have set this up using that trial. Mine will not get over, but if it does, we can use someone else's account. I don't think that given our small use case, it will even cost anything significant.
 
## Colab 
Its just an easy to get-started with type solution. If you know jupyter notebook, then this is just like jupyter notebook-meets-google doc. Can share in real time and no tension of local setup. It also has special GPU features for model training, but ofc we are NOT using any of that fancy stuff.

If you don’t know jupyter, then it is a way to write code in your browser in the cellular format of text+code that you see here. In traditional jupyter, this code would run on your local file system and processor. Ofc in COlab all that is cloud. There are other competitors to Colab too (from AWS, Azure, DataStudio, Saturn etc)
## BigQuery
For the purpose of this project, just treat it as any other traditional database. We don’t need to bother with hosting it etc.
In reality it's one of Google’s bg adat solutions supposed to be really fast and clean. Can be integrated with many other GCP products 
## Natural Language API
This is one of Google's AI/ML APIs. If we use the out of the box (and not AutoML) solution, we can do the following:
Sentiment analysis
Semantic analysis
Content categorisation
Entity extraction
Entity sentiment analysis
Instead of me explaining these, just try the interactive demo.
DataStudio

It's just a visualisation software for a given database. Not started using this really. Will update further if we integrate with our solution. 
