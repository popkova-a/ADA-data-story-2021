# "Influence network" hidden in Quotebank

### We are "Pandas & Brown Bears" and we introduce our ADA data story.
The world is small, especially for famous public figures. Do you want to know how two seemingly unrelated people in different fields could be connected to each other? Who talks about others most and who is talked among others most? The aim of our project is to reveal these unobvious relationships between the most authoritative speakers by creating directed graphs with weighted edges for different years based on how much other people talk about a particular person according to Quotebank, a corpus of quotations attributed to the speakers who uttered them, extracted from news articles of 2015-2020. The graph will represent an “influence network” of Quotebank speakers. 

## Introduction

Nowadays we acquire information mostly from social media, but a lot of people still prefer to read news. We know how news can manipulate public opinion. Journalists select topics and the way they cover them. In addition, they choose people they quote. Who are these quoted people? How are they related to each other? Usually, we don’t think about these questions when we read a news article. However, their statements have a huge impact on our society. In our project we present an “influence network” of speakers quoted in news articles between 2015 and 2020 and show what type of communities they form, highlighting some surprising results.

## Data Source

Quotebank, an open corpus of 178 million quotations attributed to the speakers who uttered them, was extracted from 162 million English news articles published between 2008 and 2020. Here, we first use Quotebank to find out the most “conversable” speakers. Since we want to find out the network of the most influential people, we selected 350 speakers whose quotation number ranks the highest. Then, we build a speaker pair, to find out how many times a “speaker” quoted a “character”.

## Analysis of the top-7 most influential people with explanations based on the political events and connections between these speakers

<div class="flourish-embed flourish-chart" data-src="visualisation/8140221"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

In our project we measure the "importance" of each speaker in order to determine the most influential people in the network. For this purpose, we use Katz centrality measure which assigns the number of paths from other nodes to this node, giving less weight to larger distances. Then, we use the obtained results to create a ranking of the most influential people, according to our news dataset.

So, who are the most influential people? To answer this question, let’s look at the interactive plot with 7 people who appeared in top-50 most influential speakers lists 6 years in a row. And 6 of them are American politicians. You can see that their positions are not stable and depend on the year selected for analysis. **We try to explain some of these fluctuations by analyzing personalities of these speakers, their attitudes towards each other and the most important political events of these years they took part in.** 

* To begin with, **Donald Trump** always kept the leading position in our top-7 ranking. We are pretty sure you know Donald Trump, but still, let us remind you of some facts about him. Donald Trump was the Republican nominee for President of the United States in the 2016 election. His presidential campaign was formally launched in June 2015. It was initially not taken seriously by political analysts, but he quickly rose to the top of opinion polls. Donald Trump won the election. At the same time, Hillary Clinton, who lost the election to Donald Trump, was just one position below in our ranking for 2015-2016. Trump made an unprecedented number of false or misleading statements during his campaign and presidency. He lost the 2020 presidential election to Joe Biden (2nd place in our competition for 2020) but refused to concede.

* We already mentioned **Joe Biden**. He is the current president of the United States, but our dataset only contains news published before his election. As a member of the Democratic Party, he served as the vice president from 2009 to 2017 under Barack Obama. Biden was often said to get prepared for a possible bid for the 2016 Democratic presidential nomination, but later, he announced that he decided not to run for president in 2016. Throughout the 2016 election, Joe Biden strongly criticized Hillary Clinton’s opponent, Donald Trump. After leaving the vice presidency, Joe Biden became a professor at the University of Pennsylvania. In 2017 he wrote a memoir and went on a book tour. Joe Biden remained in the public eye, endorsing candidates while continuing to comment on politics, climate change, and the presidency of Donald Trump. Between 2016 and 2019, media outlets often mentioned Joe Biden as a likely candidate for president in 2020. He finally launched his campaign in April 2019, that’s why, there was a sharp increase in his rating in that year. From his campaign announcement up to the start of the elections, he was generally regarded as the Democratic front-runner. National opinion polls conducted in 2020 generally showed Joe Biden leading Donald Trump in favorability. 

* Our third authoritative speaker is **Bernie Sanders**. He was a major candidate for the Democratic presidential nomination in 2016 and 2020. Despite initially low expectations, his 2016 campaign generated significant grassroots enthusiasm and funding from small-dollar donors, carrying Bernie Sanders to victory against eventual nominee Hillary Clinton in 23 primaries and caucuses before he conceded in July. In February 2019, Sanders announced that he would seek the Democratic Party's 2020 nomination for president. However, in April 2020, he conceded the nomination to Joe Biden, who had won a series of decisive victories as the field narrowed. Bernie Sanders supported Hillary Clinton and Joe Biden in their general election campaigns against Donald Trump while continuing his efforts to move the Democratic Party in a more progressive direction. Bernie Sanders’s presidential campaigns led to a resurgence of interest in democratic socialism among millennials.

* **Barack Obama** is an American politician, lawyer, and author who served as the president of the United States from 2009 to 2017. He was top-1 in our ranking before the election of Donald Trump. In May 2018, Barack Obama criticized President Trump's decision to withdraw from the nuclear deal with Iran under the Joint Comprehensive Plan of Action. In April 2020, Barack Obama endorsed his former vice president Joe Biden, the presumptive Democratic nominee, for the 2020 presidential election. In May 2020, Barack Obama criticized President Trump for his handling of the COVID-19 pandemic. Donald Trump retaliated by accusing Barack Obama of having committed "the biggest political crime in American history". In other parts of our analysis, we got results confirming that Barack Obama and Donald Trump talked about each other a lot.

* We have already mentioned **Hillary Clinton**, a member of the Democratic Party. She was the party's nominee for the 2016 presidential election, becoming the first woman to win a presidential nomination by a major U.S. political party. Hillary Clinton helped to organize a diplomatic isolation and a regime of international sanctions against Iran in an effort to force it to curtail its nuclear program; this effort eventually led to the multinational JCPOA nuclear agreement in 2015. Her usage of a private email server when she was Secretary of State was the subject of intense scrutiny; while no charges were filed against Hillary Clinton, the email controversy was the single most covered topic during the 2016 presidential election. Clinton lost the presidential election to Republican opponent Donald Trump in the Electoral College despite winning a plurality of the popular vote. Hillary Clinton was making comments on President Trump, who might be quoted in the news in 2018-2019. Since January 2020, she has been the chancellor of Queen's University Belfast in Belfast, Northern Ireland.

* **Mitchell McConnell** is an American politician and retired attorney. He has served as Senate Minority Leader since 2021, and also as the senior United States senator from Kentucky, a seat he has held since 1985. As a member of the Republican Party, he previously served as Senate Majority Leader from 2015 to 2021. McConnell worked to withhold Republican support for major presidential initiatives during the Obama administration, having made frequent use of the filibuster, and blocked many of President Barack Obama's judicial nominees. During the Trump administration, the Senate Republican majority under his leadership confirmed a record number of federal appeals court judges during a president's first two years. While supporting many of Donald Trump 's policies, McConnell was critical of his attempts to overturn the 2020 presidential election. In 2015 and 2019, Time listed Mitchell McConnell as one of the 100 most influential people in the world.

* The most unexpected (at least for us) person in this list is **Vladimir Putin**, the current president of Russia. His political actions were often widely discussed in the American and European press during the 2015-2020 period. Most members of the international community and organizations have condemned Russia for its actions in post-revolutionary Ukraine, accusing it of breaking international law and of violating Ukrainian sovereignty. In December 2015 Vladimir Putin admitted that Russian military intelligence officers were operating in Ukraine. In September 2015, President Putin authorized Russian military intervention in the Syrian civil war, following a formal request by the Syrian government for military assistance against rebel and jihadist groups. Putin announced in March 2016 that the mission he had set for the Russian military in Syria had been "largely accomplished" and ordered the withdrawal of the "main part" of the Russian forces from Syria. In 2018 Vladimir Putin won the presidential election and started his fourth term that will last until 2024. This event explains his high position in the ranking of 2018.

## Analysis of the number of quotations

<div class="flourish-embed flourish-bar-chart-race" data-src="visualisation/8163376"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

Now we can compare this ranking with another one, which is based on the number of quotations in news, and look for the dependencies between the number of speaker’s quotes in the dataset and his/her influence. We will follow speakers that were already mentioned above and see who else has the largest number of quotations among all people.
Donald Trump always took a leading position: he had a record number of quotations in different news publications. His level of influence was also the highest among all speakers in our dataset.

* Barack Obama moved down from the first position in 2015 and was out of the top-10 ranking since 2018, while he was still authoritative, according to our ranking of influential speakers. Nevertheless, he didn’t speak a lot about other influential people. You can check this in the Chord diagrams below.
Joe Biden appeared in the top in 2018 and quickly took a leading position. His number of quotations and influence level increased significantly when he launched his election campaign.

* Bernie Sanders was present in the top-10 during all years, apart from 2017.

* Hillary Clinton from the 3rd place moved out of the ranking in 2017: she was not quoted a lot, but her influence was still great.

* The interesting fact is that we can’t see Mitchell McConnell in this ranking at all. That means that he was not often quoted in news articles, and, at the same time, he was authoritative, according to the top-7 of the most influential people.

* Vladimir Putin was in the ranking in 2016-2018.

* Narendra Modi and Pope Francis were often quoted in the news. They were always present at the top of our ranking based on the number of quotations. At the same time, we can’t see them among the most influential speakers.

There are also a lot of other people in this ranking. The majority of them are American politicians. However, we can also find politicians from Israel, Canada, the United Kingdom, India and Australia. Moreover, several football managers and even Elon Musk with an enormous number of quotations also appear in our ranking.

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

## Number of quotes in degree out degree

In the year of 2015, 2017 and 2018, communities are weakly connected.
whereas in the year of 2016, 2019 and 2020, communities are not weakly connected, which means that there are separated communities of speakers having connections only between people from the same community.

The degree distribution and the in-degree distribution of the nodes in each year’s graph are skewed, justifying that we work with the real-world network.

People at the center position tend to have high in degree and relatively low out degree while people on the edge are prone to have high out degree and relatively low in degree, corresponding to the true reality.


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

## Profiles of the representative communities

"Human beings form social networks because the benefits of a connected life outweigh the costs."

**"Most influential people"**

    - Although the community is dynamic and evolving over the years, undoubtedly, the hub of the largest community always belongs to the incumbent US President, who is the most mentioned person in this community. American politicians including the secretaries of state, speakers of the United States House of Representatives, governors, and senators occupy the largest proportion in this community. 

    - Moreover, presidents of China, North Korea, Russia, Palestine, France, and the sovereign of the Vatican City State are also in this American-dominated community. Donald Trump stoked up the "America First" slogan in his speech, emphasizing the superiority of the United States, inciting hatred, changing political attitudes towards potentially threatening countries, such as China, North Korea, and Russia. Trump talked about these leaders much more than leaders of other countries, causing the sharp deterioration of bilateral relations.

    - Additionally, people from various domains, especially the business field, also appear in this big community. For instance, Jeff Bezos: founder of “Amazon” and one of the biggest stakeholders of “The Washington Post”, Elon Musk: CEO of “SpaceX” and “Tesla”, and Michael Bloomberg: founder of “Bloomberg L.P.”. Not only do they control the world’s biggest corporate giants, they are also actively involved in political campaigns, which could be explained by the fact that politics and business are usually closely related and inseparable. 

    - Surprisingly, some American celebrities are also in this “big” community. In 2020, Kobe Bryant entered this community due to his unexpected death and the whole world was caught in a whirlpool of grief mourned for this fallen legend over months.

**Indian Politicians**

    - The Indian politician community led by current Indian prime minister Narendra Modi consists of a prominent position in the influential social network. Donald Trump shifted the Obama era rebalance of the Asia-Pacific region with a new “Indo-Pacific” strategy, enhancing the positive partnership with India. Modi and Trump established their own rapport since people with similar characteristics are likely to become friends. In addition, Modi is the most quoted and also the most influential figure in this community over the 6 years. 

**British Celebrities (only appeared in 2020)**

    - The Brexit issue has been one of the most contentious topics in recent years. Since 2016, politicians have repeatedly tried to negotiate and reach a consensus between the UK and EU that would lay out the terms of the UK’s exit, ripping up the old rules of British politics as well as reshaping Europe’s trading landscape.

    - Meanwhile, the British royal family has always been the focus of the public’s attention for its members’ anecdotes: Queen’s era-defining outfits, Prince Wiliam’s new baby, Prince Harry and Meghan Markle’s Royal Drama.

    - It's not surprising that British celebrities could form a community. This community includes Prime Minister Boris Johnson, Prince Charles, Meghan Markle, Keir Starmer, and even our beloved British singer Elton John.

The three former communities we discovered are more or less correlated with politics. The question is, apart from political communities, what other genres of communities do we have? 

**European Football Community**

    - Football is the most popular sport worldwide. Europe, home of the biggest football clubs such as Real Madrid, Bayern Munich, Manchester United, has always been the center of football matches, not to mention European countries such as Germany, Belgium, England, and Italy. They have also consistently ranked top in FIFA. Therefore, European football celebrities form the world's largest sports community.

    - In this community, we could find the most authoritative figures in the football world. Pep Guardiola: the manager of Premier League club Manchester City, José Mourinho: the current head coach of Serie A club Roma, and Jürgen Klopp: the manager of Premier League club Liverpool. 

    - The interesting part is, we always assume that for a football team, the football players should be the stars. However, the majority of the people in this community are football team managers or former football players between the 1980s and 1990s. Exceptions are only for superstars like Cristiano Ronaldo: he is too hot to get away from the public’s attention.

**American Basketball Community**

    - Basketball is among the most popular sports that are watched across the globe, melting the audience's heart as well as presenting true sport spirits. Another biggest sports community is the American Basketball Community. 

    - This community comprises famous players like LeBron James: one of the greatest players in the NBA, Steven Curry: opponent of LeBron James, Kyrie Irving: teammate of Lebron James who helped the Cleveland Cavaliers secure their 2016 NBA championship over the Golden State Warriors, Dwyane Wade: LeBron James’s former teammate. This community also contains professional basketball coaches like Steve Kerr: Steven Curry’s coach, Frank Vogel: LeBron James’s coach and Nick Nurse. 

**American Football and Baseball Communities**
    - American football is the most popular sport in the United States. A survey showed that  33% of Hispanic respondents enjoyed watching American Football. The NLF (National Football League) games are the most watched content on TV, and the NFL broadcast has an average of 16.6 million viewers. This perfectly explains why the American football community, which is centered on Tom Brady (except for 2015), is one of the most stable communities during the analysed 6 years. 

    - Same situation also applies for baseball, which is the third most popular sport in the United States. The main organization, Major League Baseball (MLB), attracted 8 million viewers when the all star game began. American Baseball players, which is always dominated by Davide Price, Joe Maddon, and Terry Collins, also form a stable community.

**Actors and Singers Community(only appeared in 2020)**

    - Maybe you are not a big fan of pop music, but I am sure you know Taylor Swift: the most famous singer in the world according to Google Search. Maybe you don’t listen to rap at all, but I am sure you know Kanye West, who declared he would run for US president in 2020. Maybe you are not an avid fan of television sitcoms, but I am sure you must have heard about “Friends”. 

    - Entertainment industries like the music industry and film industry take a big part of people’s daily life. People enjoy the high quality content that the creators bring to them, whenever Lady Gaga releases a new album or Tom Hanks’ new movie comes out, they could always draw the public's attention. However, there is something the public cares more about: those creators’ personal lives. 


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

### Please note that in order to make the communities distinguishable, we limit the number of colors, the small communities are assigned to the last color.

<div class="flourish-embed flourish-chart" data-src="visualisation/8165619"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
