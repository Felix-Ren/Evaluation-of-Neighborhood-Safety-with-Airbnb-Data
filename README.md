# Evaluation-of-Neighborhood-Safety-with-Airbnb-Data

## Contributors: Winnie Gao, Fei Ren, Somsakul Somboon, Jidapa Thanabhusest, Jing Wang

The accessibility of commercial data has now exceeded that of federal data in certain
cities and categories. For example, there are now Airbnb reviews datasets available in cities
where no official crime dataset or a crime events map available to the public. Our team saw an
opportunity from this observation and decided to create a machine learning model that enables
us to generate a crime level map based on Airbnb dataset. Ultimately, we would like to offer the
public a crime map indicating safety levels in cities where there isn’t one.

Our final output is the interactive heat density map which allows users to locate areas by
inputting zipcodes in the search bar and view safety levels predicted by our best trained model.
The map is created with folium package and it is layered on openstreetmap which also provides
detailed information of the area such as street names and landmarks. To create the model, we
generated crime level measurements and used features related to neighborhood safety. We
learned from research papers and created a 1-100 spectrum of crime score normalized by
population density. For text review data, we utilized NLP techniques including bag of words and
sentimental analysis to select top important key phrases as prediction features. Also, we applied
word embedding and google’s word2vec model to measure the distance between reviews text
and self-selected words suggesting neighborhood safety. Comparing to baseline model, we saw
our best tuned random forest model has a near 20% increase in the cross validation accuracy
for LA data and near 50% increase for Austin data. Overall we think our current results can help
residents and travellers to make more informed decisions regarding safety when living or
exploring cities without public crime data.We hope that our project will be useful or inspiring
anyone interested in analyzing the area safety data to make a difference for our community.
