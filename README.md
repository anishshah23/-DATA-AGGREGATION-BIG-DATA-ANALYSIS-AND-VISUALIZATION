# -DATA-AGGREGATION-BIG-DATA-ANALYSIS-AND-VISUALIZATION
Data aggregation from Twitter and NYTimes using the APIs exposed by data sources, applying classical big data analytic method of MapReduce to the unstructured data collected, and building a visualization data product.

    a. Choose a topic of current interest to people in the USA. Something that is in the news.
        Used the topic as the key word or phrase to aggregate tweets and news articles about the topic for the same period.
        For the initial prototype just used 1 day, later you can collected these two sets of data for the same period from Twitter and NYTimes.
    b. Imported the VM appliance for Hadoop infrastructure and Loaded the data aggregated in step (a) into the VM, two directories: TwitterData and NewsData. Each directory can have many files of data.
    c. Coded and executed MapReduce word count on each of the data sets. Map will clean and parse the data sets into words, remove stop words, and reduce will count the useful words.Reviewed and visually compared the output for representative words about the topic.
    d. Visualized each of the outputs using D3.js and stored on a simple web page.
    e. Designed a web page and feed the results by embedding D3.js code (with replaceable worldclouds) in it, finalizing the display of results. Input a search topic, we will return the word cloud associated with that topic!
    f. To drill deeper into our analysis, Using the smallest data sets collected in step a), analyzed each set (Twitter and News) word co-occurrence for only the top ten words.
    g. Assumed context for co-occurrence is the “tweet” in the case of TwitterData, and the paragraph of the news
       article in the NewsData. Your “map” function emits <word, co-occurring word> and your “reduce”
       function should collate the co-occurrences for the top ten words
