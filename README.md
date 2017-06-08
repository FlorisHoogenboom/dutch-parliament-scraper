# dutch-parliament-scraper
Some time ago I came up with the idea to build a voting compass (i.e. an app
  that helps users decide which party to vote on) using data on motions
  submitted by the different parties. This notebook is the very first step in
  this project and is used to scrape all data, publicly available, from
  tweedekamer.nl. If you are worried about any legal concerns: the Dutch
  government allow scraping of their websites!

## Using this notebook
Simple open the notebook using Jupyter. To store the results you are required to
have a Neo4J instance running somewhere. To run using Docker, simply execute
something like
```
  ddocker run --publish=7474:7474 --publish=7687:7687 --volume="$(pwd)/data:/data" --volume="$(pwd)/logs:/logs" -e NEO4J_AUTH=neo4j/{YOUR PASSWORD} neo4j:3.0
```
