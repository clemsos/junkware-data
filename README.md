# Junkware Data Sets

Datasets use to NLG for the [Junkware](http://junkware.io) installation.

## Patent Data

Patent data comes from the [Fung Institute](https://github.com/funginstitute/downloads) at UC Berkeley

    mkdir data && cd data
    # wget https://s3.amazonaws.com/fungpat_olddata/patdesc.sqlite3
    wget https://s3.amazonaws.com/fungpat_olddata/patent.sqlite3
    # wget https://s3.amazonaws.com/fungpat_olddata/class.sqlite3

    # build data
    python parse_data.py

## Wikipedia Data

Wikipedia data use the [Wiki Crawl](https://github.com/guokr/wikicrawl) project to extract articles by categories. 

* It is a clojure project, so you should use ``leiningen``. 
* Change the [app.clj](https://github.com/guokr/wikicrawl/blob/master/src/wikicrawl/app.clj) according to your settings
* ``lein run`` in your terminal

## Twitter Feelings data

Extracted tweets containing "I feel" or "I am feeling" from Twitter - following [We Feel Fine](http://wefeelfine.org/methodology.html) recommandations
