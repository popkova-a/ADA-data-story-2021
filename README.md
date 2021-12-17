# "Influence network" hidden in Quotebank

###    We are "Pandas & Brown Bears" and we introduce our ADA data story.

The world is small, especially for famous public figures. Do you want to know how two seemingly unrelated people in different fields could be connected to each other? Who talks about others most and who is talked among others most?  The aim of our project is to reveal these unobvious relationships between the most authoritative speakers by creating directed graphs with weighted edges for different years based on how much other people talk about a particular person according to Quotebank, a corpus of quotations attributed to the speakers who uttered them, extracted from news articles of 2015-2020. The graph will represent an “influence network” of Quotebank speakers. 
# ------------------------------------
<div>
  <script>
  function openGraph(evt, yearName) {
    var i, tabcontent, tablinks;

    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
      tabcontent[i].style.display = "none";
    }

    tablinks = document.getElementsByClassName("tablinks");
    for (i = 0; i < tablinks.length; i++) {
      tablinks[i].className = tablinks[i].className.replace(" active", "");
    }

    document.getElementById(yearName).style.display = "block";
    evt.currentTarget.className += " active";
  }
  </script>

  <style>
  /* Style the tab */
  .tab {
    overflow: hidden;
    border: 1px solid #ccc;
    background-color: #f1f1f1;
    width: 800px;
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
    width: 800px;
    height: 800px;
  }
  </style>

  <!-- Tab links -->
  <div class="tab">
    <button class="tablinks" onclick="openGraph(event, '2015')" id="defaultOpen">2015</button>
    <button class="tablinks" onclick="openGraph(event, '2016')">2016</button>
    <button class="tablinks" onclick="openGraph(event, '2017')">2017</button>
    <button class="tablinks" onclick="openGraph(event, '2018')">2018</button>
    <button class="tablinks" onclick="openGraph(event, '2019')">2019</button>
    <button class="tablinks" onclick="openGraph(event, '2020')">2020</button>
  </div>

  <!-- Tab content -->
  <div id="2015" class="tabcontent">
    <embed type="text/html" src="plots/plot2015_750.html" width="800" height="800">
  </div>

  <div id="2016" class="tabcontent">
    <embed type="text/html" src="plots/plot2016_750.html" width="800" height="800">
  </div>

  <div id="2017" class="tabcontent">
    <embed type="text/html" src="plots/plot2017_750.html" width="800" height="800">
  </div>

  <div id="2018" class="tabcontent">
    <embed type="text/html" src="plots/plot2018_750.html" width="800" height="800">
  </div>

  <div id="2019" class="tabcontent">
    <embed type="text/html" src="plots/plot2019_750.html" width="800" height="800">
  </div>

  <div id="2020" class="tabcontent">
    <embed type="text/html" src="plots/plot2020_750.html" width="800" height="800">
  </div>
</div>

<div>
  <script>
  document.getElementById("defaultOpen").click();
  </script>
</div>

<div>
  <script>
  function openGraph_comm(evt, yearName) {
    var i, tabcontent, tablinks;

    tabcontent = document.getElementsByClassName("tabcontent_comm");
    for (i = 0; i < tabcontent.length; i++) {
      tabcontent[i].style.display = "none";
    }

    tablinks = document.getElementsByClassName("tablinks_comm");
    for (i = 0; i < tablinks.length; i++) {
      tablinks[i].className = tablinks[i].className.replace(" active", "");
    }

    document.getElementById(yearName).style.display = "block";
    evt.currentTarget.className += " active";
  }
  </script>

  <style>
  /* Style the tab */
  .tab_comm {
    overflow: hidden;
    border: 1px solid #ccc;
    background-color: #f1f1f1;
    width: 800px;
  }

  /* Style the buttons that are used to open the tab content */
  .tab_comm button {
    background-color: inherit;
    float: left;
    border: none;
    outline: none;
    cursor: pointer;
    padding: 14px 16px;
    transition: 0.3s;
  }

  /* Change background color of buttons on hover */
  .tab_comm button:hover {
    background-color: #ddd;
  }

  /* Create an active/current tablink class */
  .tab_comm button.active {
    background-color: #ccc;
  }

  /* Style the tab content */
  .tabcontent_comm {
    display: none;
    padding: 6px 12px;
    border: 1px solid #ccc;
    border-top: none;
    width: 800px;
  }
  </style>

  <!-- Tab links -->
  <div class="tab_comm">
    <button class="tablinks_comm" onclick="openGraph_comm(event, '2015_comm')" id="defaultOpen_comm">2015</button>
    <button class="tablinks_comm" onclick="openGraph_comm(event, '2016_comm')">2016</button>
    <button class="tablinks_comm" onclick="openGraph_comm(event, '2017_comm')">2017</button>
    <button class="tablinks_comm" onclick="openGraph_comm(event, '2018_comm')">2018</button>
    <button class="tablinks_comm" onclick="openGraph_comm(event, '2019_comm')">2019</button>
    <button class="tablinks_comm" onclick="openGraph_comm(event, '2020_comm')">2020</button>
  </div>

  <!-- Tab content -->
  <div id="2015_comm" class="tabcontent_comm">
    <div class="flourish-embed flourish-network" data-src="visualisation/8150019"><script src="https://public.flourish.studio/resources/embed.js"></script></div> 
  </div>

  <div id="2016_comm" class="tabcontent_comm">
    <div class="flourish-embed flourish-network" data-src="visualisation/8149786"><script src="https://public.flourish.studio/resources/embed.js"></script></div> 
  </div>

  <div id="2017_comm" class="tabcontent_comm">
    <div class="flourish-embed flourish-network" data-src="visualisation/8143275"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
  </div>

  <div id="2018_comm" class="tabcontent_comm">
    <div class="flourish-embed flourish-network" data-src="visualisation/8144602"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
  </div>

  <div id="2019_comm" class="tabcontent_comm">
    <div class="flourish-embed flourish-network" data-src="visualisation/8144488"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
  </div>

  <div id="2020_comm" class="tabcontent_comm">
    <div class="flourish-embed flourish-network" data-src="visualisation/8143518"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
  </div>
</div>

<div>
  <script>
  document.getElementById("defaultOpen_comm").click();
  </script>
</div>

<div>
  <script>
  function openGraph_circ(evt, yearName) {
    var i, tabcontent, tablinks;

    tabcontent = document.getElementsByClassName("tabcontent_circ");
    for (i = 0; i < tabcontent.length; i++) {
      tabcontent[i].style.display = "none";
    }

    tablinks = document.getElementsByClassName("tablinks_circ");
    for (i = 0; i < tablinks.length; i++) {
      tablinks[i].className = tablinks[i].className.replace(" active", "");
    }

    document.getElementById(yearName).style.display = "block";
    evt.currentTarget.className += " active";
  }
  </script>

  <style>
  /* Style the tab */
  .tab_circ {
    overflow: hidden;
    border: 1px solid #ccc;
    background-color: #f1f1f1;
    width: 800px;
  }

  /* Style the buttons that are used to open the tab content */
  .tab_circ button {
    background-color: inherit;
    float: left;
    border: none;
    outline: none;
    cursor: pointer;
    padding: 14px 16px;
    transition: 0.3s;
  }

  /* Change background color of buttons on hover */
  .tab_circ button:hover {
    background-color: #ddd;
  }

  /* Create an active/current tablink class */
  .tab_circ button.active {
    background-color: #ccc;
  }

  /* Style the tab content */
  .tabcontent_circ {
    display: none;
    padding: 6px 12px;
    border: 1px solid #ccc;
    border-top: none;
    width: 800px;
    height: 800px;
  }
  </style>

  <!-- Tab links -->
  <div class="tab_circ">
    <button class="tablinks_circ" onclick="openGraph_circ(event, '2015_circ')" id="defaultOpen_circ">2015</button>
    <button class="tablinks_circ" onclick="openGraph_circ(event, '2016_circ')">2016</button>
    <button class="tablinks_circ" onclick="openGraph_circ(event, '2017_circ')">2017</button>
    <button class="tablinks_circ" onclick="openGraph_circ(event, '2018_circ')">2018</button>
    <button class="tablinks_circ" onclick="openGraph_circ(event, '2019_circ')">2019</button>
    <button class="tablinks_circ" onclick="openGraph_circ(event, '2020_circ')">2020</button>
  </div>

  <!-- Tab content -->
  <div id="2015_circ" class="tabcontent_circ">
    <div class="flourish-embed flourish-chord" data-src="visualisation/8164531"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
  </div>

  <div id="2016_circ" class="tabcontent_circ">
    <div class="flourish-embed flourish-chord" data-src="visualisation/8164398"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
  </div>

  <div id="2017_circ" class="tabcontent_circ">
    <div class="flourish-embed flourish-chord" data-src="visualisation/8164312"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
  </div>

  <div id="2018_circ" class="tabcontent_circ">
    <div class="flourish-embed flourish-chord" data-src="visualisation/8164202"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
  </div>

  <div id="2019_circ" class="tabcontent_circ">
    <div class="flourish-embed flourish-chord" data-src="visualisation/8164102"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
  </div>

  <div id="2020_circ" class="tabcontent_circ">
    <div class="flourish-embed flourish-chord" data-src="visualisation/8163809"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
  </div>
</div>

<div>
  <script>
  document.getElementById("defaultOpen_circ").click();
  </script>
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
<div class="flourish-embed flourish-bar-chart-race" data-src="visualisation/8163376"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

# Katz Centrality (7 persons who appear in top-50 influential people 6 years in a row):
<div class="flourish-embed flourish-chart" data-src="visualisation/8140221"><script src="https://public.flourish.studio/resources/embed.js"></script></div> 
