# Nuclear_Energy_Sentiment_Analysis

We scrape data from Google News and Twitter to compare the sentiment towards nuclear energy in Germany over the last two years.
Context: In Germany the nuclear phase-out was basically political consens until the war in Ukraine started in late February 2022. Since then an energy shortage discussion started because of the country's dependence of Russian gas. Hence the topic of nuclear energy came back to life last year, with some major political parties bringing even building new power plants back on the agenda.
We try to analyze how that discussion is represented in news headlines and on Twitter and evaluate the sentiment towards the topic of nuclear energy.
1. About 1600 german news article headlines are evaluated with a pretrained BERT model ("german-news-sentiment-bert") from Huggingface which was trained on German news articles. The data is scraped from Google News from Jan 2021 until the end of Jan of 2023
2. For our Twitter analysis we fine tune a BERT text classifier model ("german-sentiment-bert") from Huggingface on a rated Twitter dataset from the Technical University of Berlin.
3.We analyse the sentiment of roughly 45 000 Twitter posts from Jan 2021 until Jan 2023
4. Interpretation of the results.
Hypotheseis 1: The topic of nuclear energy should be trending more often on Twitter since Feb 2022, and also the amount of news articles related to that matter should be have increased.
Hypotheseis 2: There should not only be an absoute increase of articles and Twitter posts concering nuclear energy but also an relative increase of favourable content.
