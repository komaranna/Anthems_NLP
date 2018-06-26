# Anthems_NLP

NLP analysis of anthems around the world, based on English translations from
http://lyricstranslate.com/en/national-anthems-lyrics.html

I use a bag-of-words model to extract features from the corpus of all anthems, then create the feature vector for each anthem. Then, I use a t-SNE visualization to look for clusters.

I didn't find more than 1 clear cluster, however, there is evidence of 3 outliers:

1. Turkish National Anthem: http://lyricstranslate.com/en/istiklal-marsi-liberation-march.html

2. National Anthem of Grenada: http://lyricstranslate.com/en/national-anthems-hail-grenada-lyrics.html

3. Pledge of Allegiance (not an anthem, nevertheless was included in dataset): http://lyricstranslate.com/en/national-anthems-patriotic-songs-american-pledge-allegiance-lyrics.html

Places of improvement:

I tried stemming but it yielded no improvement.

Weighting the features before the t-SNE should improve analysis about clustering. Tried tf-idf but the remaining features became way too specific to the anthems (e.g. the name of the nations)

I didn't account for the different lengths of anthems, which could throw this analysis off somewhat.
