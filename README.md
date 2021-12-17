# "Influence network" hidden in Quotebank

###    We are "Pandas & Brown Bears" and we introduce our ADA data story.

The world is small, especially for famous public figures. Do you want to know how two seemingly unrelated people in different fields could be connected to each other? Who talks about others most and who is talked among others most?  The aim of our project is to reveal these unobvious relationships between the most authoritative speakers by creating directed graphs with weighted edges for different years based on how much other people talk about a particular person according to Quotebank, a corpus of quotations attributed to the speakers who uttered them, extracted from news articles of 2015-2020. The graph will represent an “influence network” of Quotebank speakers. 
# ------------------------------------
<div>
<script>
function openCity(evt, cityName) {
  // Declare all variables
  var i, tabcontent, tablinks;

  // Get all elements with class="tabcontent" and hide them
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }

  // Get all elements with class="tablinks" and remove the class "active"
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }

  // Show the current tab, and add an "active" class to the button that opened the tab
  document.getElementById(cityName).style.display = "block";
  evt.currentTarget.className += " active";
}
</script>

<style>
/* Style the tab */
.tab {
  overflow: hidden;
  border: 1px solid #ccc;
  background-color: #f1f1f1;
}

/* Style the buttons that are used to open the tab content */
.tab button {
  background-color: inherit;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  transition: 0.3s;
}

/* Change background color of buttons on hover */
.tab button:hover {
  background-color: #ddd;
}

/* Create an active/current tablink class */
.tab button.active {
  background-color: #ccc;
}

/* Style the tab content */
.tabcontent {
  display: none;
  padding: 6px 12px;
  border: 1px solid #ccc;
  border-top: none;
}
</style>

<!-- Tab links -->
<div class="tab">
  <button class="tablinks" onclick="openCity(event, 'London')">London</button>
  <button class="tablinks" onclick="openCity(event, 'Paris')">Paris</button>
  <button class="tablinks" onclick="openCity(event, 'Tokyo')">Tokyo</button>
</div>

<!-- Tab content -->
<div id="London" class="tabcontent">
  <h3>London</h3>
  <p>London is the capital city of England.</p>
</div>

<div id="Paris" class="tabcontent">
  <h3>Paris</h3>
  <p>Paris is the capital of France.</p>
</div>

<div id="Tokyo" class="tabcontent">
  <h3>Tokyo</h3>
  <p>Tokyo is the capital of Japan.</p>
</div>
</div>
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

## Key Takeaways:

## Who Are We?
<div class="flourish-embed flourish-bar-chart-race" data-src="visualisation/8154330"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

# Katz Centrality (7 persons who appear in top-50 influential people 6 years in a row):
<div class="flourish-embed flourish-chart" data-src="visualisation/8140221"><script src="https://public.flourish.studio/resources/embed.js"></script></div> 
