# Introduction
## Abstract:
Influence has long been studied in the fields of sociology, communication, and political science. Traditional communication theory states that a minority, called influentials, excels in persuading others. Generally, more quotations of a person indicate more impact of this speaker or at least his/her higher exposure to the public. 

In this project, our intention is to reveal the unobvious relationships between the most authoritative speakers by creating a directed graph with weighted edges based on how much other people talk about a particular person according to Quotebank, a corpus of quotations attributed to the speakers who uttered them, extracted from news articles of 2015-2020. The graph will represent an “influence network” of Quotebank speakers. The world is small (recall “six degrees of separation”), especially for famous public figures, so we are also interested in how two seemingly unrelated people in different fields could be connected to each other.

## Research Questions:
* **Who are the most authoritative people that other speakers talk about?** 
    - Introducing the new measure of “influence” defined as the number of mentions of the person by other speakers, we are interested in the fact who occupies the highest positions in the ranking based on this impact rate. 
* **Does the number of speaker’s quotes in the dataset correlate with his/her influence?**
    - Since the quotation rate of a person can be also considered as a measure of his/her exposure to the public (the more news sources quote the speaker, the more impact he/she has), we are going to analyze which people satisfy both of the criteria.
* **What potential/hidden communities do the speakers form? And how do they link together?**
    - In general, we tend to classify people by their occupations, genders, races, etc. But are there potential communities that aren’t that obvious? We are looking forward to discovering hidden communities with a clustering algorithm, and trying to investigate how these latent communities form.
* **How does the “influence network” evolve over 2015-2020?**
    - After the construction of the “influence network”, we would like to study further its evolution in these 6 years and answer questions: Whose influence increases over time and whose decreases? Who joined and who left the ‘most influential people’ community? etc.
 
## Methods:
In order to determine the most influential people in the network, we will use the Katz centrality measure for directed graphs.

Further, we will apply a community detection algorithm named Girvan-Newman to decompose the most influential speakers’ neighborhoods into different heavily interlinked groups, which results in hierarchical clustering. Since the Girvan-Newman method encounters some problems when applied to some directed graphs with a special structure, then our approach is to treat a directed graph as undirected when using this method for community detection. We will use modularity to evaluate the quality of a community clustering.

In order to track the evolution and structure of communities over time, we will use Jaccard similarity, which is a statistic used for gauging the similarity and diversity of sets.

Other characteristics of the graph that we plan to get are the connectivity of the directed graph and its in-degree distribution. As the “influence network” representation, we draw a graph using the NetworkX Python library, also we plan to show the relationships between the most authoritative persons by plotting a heatmap.
