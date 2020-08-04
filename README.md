[![Screen-Shot-2020-08-03-at-21-54-55.png](https://i.postimg.cc/vZ8k9N0K/Screen-Shot-2020-08-03-at-21-54-55.png)](https://postimg.cc/SJ5gbDFL)
# Game of Thrones - Sentences Analysis
This project is related to a series of data analysis about to the worldwide famous tv show 'Game of Thrones', more specifically about all sentences said during the 8 seasons.

## Technologies you'll see here
- Python
- Spark (PySpark)
- Docker
- Jupyter Notebook
- Sentiment Analysis Python packages
- SQL strategies

## The Notebook
The 'star' of this repository is [here](https://github.com/lmassaoy/got-sentence-analysis/blob/master/jupyter_pyspark/volume/notebooks/GoT_Sentences_Analysis.ipynb) to be checked.
I made a series of data analysis very compatible to a professional case and, as a bonus, I applied an enhancement to create the sentiment analysis of each sentence of the dataset, allowing us to understand how the python libs 'vaderSentiment' and 'textblob' can be easily used in data engineering or as service.
Please have fun :)

## Setup - How to build and explore by yourself
### Docker Image
Q: "lyamada, why not use the jupyter official image"
A: Because we'll need to have the sentiment analysis libs installed in our container
```
$ docker build -t jupy_sentiment:latest .
```
### Docker-Compose (Start)
```
$ cd jupyter_pyspark
$ docker-compose up -d
```
### Opening the Jupyter
```
$ docker ps
$ docker logs <container_id>
```
Copy the URL with the token and change the port '8888' to '10000'.
Paste in your favorite browser
### Spark History
Access in your browser the address localhost:4040
### Docker-Compose (Stop)
```
$ cd jupyter_pyspark
$ docker-compose down
```
