
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>PixarSoul twitter analysis</title>

    <style>
      body, html {
        height: 100%;
        margin: 0;
      }

      .container {
          max-width: 800px;
          margin: 0 auto;
          font-family: Helvetica;
          line-height: 1.6;
          text-align: justify;
      }

      H1, H2 {

          color: #003399;
      }

      .column {
            float: left;
            width: 50%;
            margin:0 auto;
            padding: 0px;
                  /* Should be removed. Only for demonstration */
          }
          /* Clear floats after the columns */
      .row::after {
            content: "";
            display: table;
            clear: both;
          }

      a:link {color: #DCB2FE;}


      .bg {
          /* The image used */
          background-image: url("http://qqpublic.qpic.cn/qq_public/0/0-2642333471-B74FFD7650781AA744B7B353556CDB77/0?fmt=jpg&size=75&h=382&w=900&ppv=1/0");

          position: relative;

          /* Full height */
          height: 60%;

          /* Center and scale the image nicely */
          background-position: center;
          background-repeat: no-repeat;
          background-size: cover;
        }

        .caption {
          position: absolute;
          left: 0;
          top: 45%;
          width: 100%;
          text-align: center;
          color: #000;
        }

      .caption span.border1 {
          background-color: #003399;
          color: #fff;
          padding: 18px;
          font-size: 30px;
          letter-spacing: 6px;
        }

      .caption span.border2 {
            background-color: #DCB2FE;
            color: #fff;
            padding: 12px;
            font-size: 10px;
            letter-spacing: 2px;
          }

    </style>

    <script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>

  </head>
  <body>



    <div class="bg">

      <div class="caption">

        <span class="border1">Analyse the Success of PixarSoul from Twitter data</span><br><br><br>
        <span class="border2">Hongshan Fan  11/01/2021</span>

      </div>

    </div><br><br>




    <div class="container">


    <div>

        <h2>Why choose soul as the theme</h2>

    </div>



    <div>
      <p>On Christmas Day, December 25, 2020, Pixar’s original animated film Soul was released in North America and areas without streaming media services. Unlike the past, most European and American countries are severely affected by the Covid-19 and offline theaters cannot operate normally, the work is exclusively shown on Disney+. The film was originally scheduled to premiere in the United States in June, but was affected by the epidemic and was finally set on December 5. </p>

      <p>"Soul" doesn't require any extra fees to watch. The movie is included as part of a standard Disney Plus subscription. Disney previously charged $30 for "<a href="https://www.businessinsider.com/disney-plus-premiere-access">Premier Access</a>" to "<a href="https://www.businessinsider.com/how-to-watch-mulan-movie" >Mulan</a>" when it skipped theaters for Disney Plus in September. </p>

      <p>At Christmas and New Year, people affected by the epidemic will naturally be more inclined to engage in entertainment projects that can be experienced online at home. The free viewing service that Disney+ launched during this period (excluding the subscription fee of $6.99 per month or $69.99 per year) must have been strategically considered. So, it is very meaningful to analyze users' opinions on this movie and Disney+ service. </p>
    </div><br><br>



    <div>

        <h2>User Twitter analysis</h2>

    </div>



    <div>
      <p>In this part, I used TAGS to collect tweets with hashtag #PixarSoul from December 31, 2020 to January 9, 2020. I hope to analyze the effects of Disney+’s commercial strategy from the audience’s evaluation and views on the film. </p>

      <h3>Top tweeters and bots</h3>

      <p>Top tweeters sent and forwarded the most relevant information during the sampling period. This statistic can help us filter out the "core followers" of the topic, whose voices are very precious. But at the same time, we cannot ignore the impact of robots on this statistic. My survey hopes to see the changing trend of the discussion content and discussion heat for the movie and Disney+ during the period, and the robot will continue to automatically forward the content of specific tags and official accounts. This will undoubtedly cause great interference to the research. The following table is a comparison of top tweeters before and after noise removal. </p>

      <div id="chart_div1"></div>
      <div id="chart_div2"></div>

      <p>After data noise reduction, we can see that some robots that have tweeted more are removed. Although we still see some users maintaining a high number of tweets, the overall number of tweets is more reasonable. Users who send Twitter frequently in a short period of time play an important role in some research on user behavior, but I won’t go into details this time.</p>

      <p>After using the <a href="https://botometer.osome.iu.edu/">botometer tool </a> to evaluate, we can see that among the top ten tweets, 7 have a robot index exceeding 2.5 (indicating that they have more Robot behavior). Because the main purpose of this article is to listen to the user's voice and analyze the user's focus on the film, so I excluded users with a robot score of more than 2.5 and their tweets from the top 50 Twitters. In the end, I deleted 487 tweets of 20 Twitter users and continued the analysis using the noise reduction data (from the remaining 10,194 tweets). </p>
    </div><br>




    <div>
      <h3>The ratio of tweeters from top 10 tweeters</h3>
      <p>After the data noise reduction process, I want to know how many tweets and retweets are from the top ten tweets. These statistics can help us analyze whether this event is a widely discussed event or an event led by a minority group.</p>
      <div id="piechart1" style="width: 800px; height: 444px;"></div>
      <p>We can see that the actual volume of the top 10 tweeters is not large, accounting for only 2.9% of the total tweets. This also means that the discussion surrounding the movie Soul is more from a broad audience than a small number of active users. This reflects that the Twitter data collected this time can well illustrate the user's discussion and views on the movie and watching mode of Disneyplus.</p>
    </div><br>



    <div>
      <h3>The distribution of the number of tweets</h3>
      <div align="center"><img width="700px" src="chart.svg"></img></div>
      <p>Statistics show that the vast majority of viewers only post/repost a small number of tweets. On the one hand, it shows that the data noise reduction is relatively successful. On the other hand, it shows that although the topic has caused a relatively wide range of discussions, the continuous discussion and attention of users on the topic is not high.
      </p>
    </div><br>




    <div>
      <h3>Demographic</h3>
      <p>After analyzing the top 10 Top twitters, we can find that 6 of them have more than 1k followers (fans). It can be seen that users with more fans will actively participate in this discussion. Among them, 2 users have tweeted more than 1M (Top 1 and 2 respectively), and most of their Twitter content is reposted. Although we have performed data noise reduction, the behavior of these two users is still suspicious.
      </p>
      <p>I also found that there is an official account @DisneyStudios in it, which shows that Disney officials put a lot of energy into the promotion of this film and that the film is relatively important.
      </p>

    </div><br>




    <div>
      <h3>The top retweet and proportion of retweets to tweets</h3>
      <p>"RT @PixarSoul: 🎊"Good luck finding that spark"🎊 #PixarSoul". This short tweet was retweeted the most, up to 350 times. His original author is @PixarSoul, indicating that the official account has a certain guiding role in this discussion on Twitter.</p>
      <div id="piechart2" style="width: 800px; height: 444px;"></div>
      <p>In addition, retweets accounted for 50.67% of total tweets. We can see that at least half of the tweets are original by viewers, which shows that users have enough spontaneous love for the topic.
      </p>
    </div><br>




    <div>
      <h3>High-frequency vocabulary and sentiment analysis</h3>
      <p>As we predicted, Disneyplus is frequently mentioned in both Twitter texts and co-hashtags. It can be seen intuitively in the emotional analysis that people’s evaluations of this movie and Disneyplus are mostly positive and pleasant.
      </p><br>
      <div align="center"><img src="Hashtag.png" width="650"></div>
      <div align="center"><img width="800px" src="wordcloud.svg"></img></div>

      <p>In addition, I also used a <a href="https://www.lexalytics.com/demo#">text sentiment analysis tool</a> to analyze the text of the top 50 reposted tweets, and found that the overall emotional tendency of the text is positive. Since the proportion of reposted tweets accounts for half of the total tweets, this sentiment analysis result can also reflect that users' emotions when discussing the movie are generally positive.
      </p>


    </div><br>




    <div>
      <h3>Geographic analysis</h3>
      <p>Regional analysis is a very complicated task. I need to merge the information of the location of Twitter (USA, United States, America, etc.) and deal with the data noise caused by the virtual geographic location.
      </p>
      <div class='row' alignment='center'>
              <div class='column'>
                <div id="piechart3" style="width: 500px; height: 278px; "></div>
              </div>
              <div class='column'>
                <div id="piechart4"style="width: 500px; height: 278px; "></div>
              </div>
      </div>

      <p>According to statistics, among the 10,194 tweets collected this time, about 28% of the geographic information is unlabeled.
      Among them, there are actually only 4 people located by geocode. It shows that the vast majority of users have not disclosed their true geographic location.
      </p><br>
      <div id="regions_div" style="width: 800px; height: 444px;"></div><br>
      <p>From the figure, we can clearly see that among the collected Twitter, American users account for the vast majority. This is because the movie's recent launches are mainly in North America, and Twitter users are more concentrated in the United States. Although the number of the second-ranked UK is very different from that of the United States, considering that the film was premiered at the London Film Festival in October 2020, the second place can also reflect the excellent quality of the work as a film that was released for the "second time".</p>
    </div><br>




    <div>
      <h3>Changes in the number of tweets over time</h3>
      <p>So, when did this movie have the highest degree of discussion? Through the daily summary, we can see that during the New Year’s holiday, more people are discussing this movie on Twitter. As time goes by, the popularity gradually decreases. This is in line with our general view of the popularity of a movie-it is widely discussed in people's leisure time, and the popularity diminishes with time.
      </p>
      <div id="curve_chart1" style="width: 800px; height: 444px"></div>
      <p>But on January 1, 2021, I found a strange phenomenon after counting in hours. From 19 to 20, the number of tweets increased dramatically. The reason for the rapid growth is speculated to be the concentrated discussion of the film by the audience during the afternoon of the holiday.
      </p>
      <div id="curve_chart2" style="width: 800px; height: 444px"></div>

    </div><br>



    <div>
      <h3>Conclusion</h3>
      <p>After data collection, noise reduction and analysis, we can draw the following conclusions:
      </p>

      <p>a. Soul, as an excellent film, aroused widespread and spontaneous discussion among the audience;
      </p>
      <p>b. The audience is positive about the film and the way of watching the movie;
      </p>
      <p>c. During the holidays, the discussion about the film is lively, and the degree of discussion decreases with time.
      </p>
    </div><br>



    <div>
      <h2>Disney+ strategy</h2>
      <p>In the last part, I analyzed and summarized the collected Twitter data from multiple angles, and from being a true original movie of Disney, its significance is not only that it is a moving and excellent work, it also brought a touch of warmth to the New Year when movement was restricted due to the impact of the epidemic in this cold winter. The movie is undoubtedly a success, but I actually want to explore what role Disneyplus played in this discussion. It can be seen from the high-frequency vocabulary part of the Twitter analysis that the audience mentioned Disneyplus many times while discussing their experience of watching movies. Although Disneyplus is the only movie-watching channel now, the positive text emotions can still reflect from the side that Disney+ users have a better experience.
      </p>

      <p>It is the first time that Disney provides exclusive streaming media services to subscribers for free. All this is not without preconditions. On December 10, 2020, before the film’s release, Disney+ stated that their subscribers exceeded 86 million and provided Star Wars and Marvel content.
      </p>
      <p>Prior to this, the Covid-19 led to the closure of theme parks and the delay of film releases, all of which caused Disney to suffer huge losses.
      </p>
      <p>Statistics from statista show that in 2020, Disney+ subscriptions have achieved greater growth in Q4. Whether Soul, which can be watched without additional payment, can become a turning point for Disney+ and even Disney's turnaround, it still needs time to verify.
      </p>
      <a href="https://www.statista.com/statistics/1095372/disney-plus-number-of-subscribers-us/" rel="nofollow"><img src="https://www.statista.com/graphic/1/1095372/disney-plus-number-of-subscribers-us.jpg" alt="Statistic: Disney+'s number of subscribers worldwide from 1st quarter 2020 to 4th quarter 2020 | Statista" style="width: 100%; height: auto !important; max-width:1000px;-ms-interpolation-mode: bicubic;"/></a><br />Find more statistics at  <a href="https://www.statista.com" rel="nofollow">Statista</a><br><br>
      <a href="https://www.statista.com/statistics/1040284/quarterly-income-loss-walt-disney-company-by-segment/" rel="nofollow"><img src="https://www.statista.com/graphic/1/1040284/quarterly-income-loss-walt-disney-company-by-segment.jpg" alt="Statistic: Operating income/loss of the Walt Disney Company from 4th quarter 2017 to 4th quarter 2020, by segment (in million U.S. dollars) | Statista" style="width: 100%; height: auto !important; max-width:1000px;-ms-interpolation-mode: bicubic;"/></a><br />Find more statistics at  <a href="https://www.statista.com" rel="nofollow">Statista</a>
    </div><br>









  </div><br><br><br><br>



    <script type="text/javascript">
      var myMapsApiKey = 'AIzaSyAJnpteIPHLgrxrSH32i8R763yjjKOp6Jw';
      google.charts.load('current', {
        'packages':['geochart'],
        // Note: you will need to get a mapsApiKey for your project.
        // See: https://developers.google.com/chart/interactive/docs/basic_load_libs#load-settings
        'mapsApiKey': myMapsApiKey
      });
      google.charts.setOnLoadCallback(drawRegionsMap);

      function drawRegionsMap() {
        var data = google.visualization.arrayToDataTable([
          ['Country', 'Popularity'],
          ['Mexico', 105],
          ['United States', 2654],
          ['United Kingdom', 414],
          ['Canada', 160],
          ['India', 142],
          ['Venezuela', 122],
          ['France', 100],
          ['Brazil', 97],
          ['Spain', 69],
          ['Australia', 47],
          ['Chile', 33],
          ['Colombia', 30],
          ['Indonesia', 27],
          ['Russia', 26],
          ['Nigeria', 25],
          ['Germany', 25],
          ['Japan', 20],
          ['China', 10],
          ['Thailand', 18],
          ['Panama', 17],
          ['Cameroon', 33],
          ['Netherlands', 17],
          ['Cuba', 13],
          ['Italy', 16],
          ['República Dominicana', 14],
          ['Singapore', 13],
          ['United Arab Emirates', 35],
          ['Korea', 12],
          ['Utah', 11],
          ['South Africa', 11],
          ['Kenya', 10],
          ['Argentina', 9],
          ['Portugal', 8],
          ['Egypt', 8],
          ['Argentina', 9],
          ['Isreal', 5],
          ['Bali', 6],
        ]);

        var options = {colorAxis: {colors: ['#F4E9FF', '#2649AA', '#003399']}, title: 'The volume of tweets around the world' };

        var chart = new google.visualization.GeoChart(document.getElementById('regions_div'));

        chart.draw(data, options);
      }
    </script>



    <script type="text/javascript">
      google.charts.load('current', {'packages':['corechart']});
      google.charts.setOnLoadCallback(drawChart);

      function drawChart() {

        var data = google.visualization.arrayToDataTable([
          ['tweet Type', 'Volume'],
          ['geocoded',     4],
          ['ungeocoded',      10190]
        ]);

        var options = {

          legend: { position: 'right'},
          colors:['#DCB2FE', '#003399'],
          sliceVisibilityThreshold: .0001
        };

        var chart = new google.visualization.PieChart(document.getElementById('piechart4'));

        chart.draw(data, options);
      }
    </script>
    <script type="text/javascript">
      google.charts.load('current', {'packages':['corechart']});
      google.charts.setOnLoadCallback(drawChart);

      function drawChart() {

        var data = google.visualization.arrayToDataTable([
          ['tweet Type', 'Volume'],
          ['located',     7327],
          ['unlocated',      2867]
        ]);

        var options = {

          legend: { position: 'right'},
          colors:['#DCB2FE', '#003399'],
          sliceVisibilityThreshold: .0001

        };

        var chart = new google.visualization.PieChart(document.getElementById('piechart3'));

        chart.draw(data, options);
      }
    </script>
    <!--piechart-->

    <script type="text/javascript">
      google.charts.load('current', {'packages':['corechart']});
      google.charts.setOnLoadCallback(drawChart);

      function drawChart() {

        var data = google.visualization.arrayToDataTable([
          ['tweet Type', 'Volume'],
          ['Retweets',     5166],
          ['tweets',      5028]
        ]);

        var options = {
          title: 'what was the ratio of tweets and retweets?',
          legend: { position: 'top', alignment: 'center'},
          colors:['#DCB2FE', '#003399']
        };

        var chart = new google.visualization.PieChart(document.getElementById('piechart2'));

        chart.draw(data, options);
      }
    </script>
    <script type="text/javascript">
      google.charts.load('current', {'packages':['corechart']});
      google.charts.setOnLoadCallback(drawChart);

      function drawChart() {

        var data = google.visualization.arrayToDataTable([
          ['Task', 'Hours per Day'],
          ['Top tweeters',     304],
          ['Others',      10195]
        ]);

        var options = {
          title: 'How many tweets are from top 10 tweeters?',

          slices: {  1: {offset: 0.2},
          },
          legend: { position: 'top', alignment: 'center'},
          colors:['#DCB2FE', '#003399']
        };

        var chart = new google.visualization.PieChart(document.getElementById('piechart1'));

        chart.draw(data, options);
      }
    </script>
    <!--piechart-->

    <script type="text/javascript"
      src="http://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script>
      <script type="text/javascript" src="https://www.google.com/jsapi"></script>
      <script type="text/javascript">
      google.load("visualization", "1", {packages:["corechart"]});
      google.setOnLoadCallback(drawChart);
      var jsonDataObj1 = {
      "rows":[
      {"c":[{"v":"Shunsuke_K_D"},{"v":69},{"v":0}]},
      {"c":[{"v":"DiChristine"},{"v":66},{"v":1}]},
      {"c":[{"v":"MatthewTwihard"},{"v":60},{"v":0}]},
      {"c":[{"v":"Jemorr1"},{"v":52},{"v":0}]},
      {"c":[{"v":"BruceJ95"},{"v":51},{"v":0}]},
      {"c":[{"v":"MohitHaram2049"},{"v":47},{"v":0}]},
      {"c":[{"v":"animationmovief"},{"v":31},{"v":0}]},
      {"c":[{"v":"rirapido1"},{"v":12},{"v":18}]},
      {"c":[{"v":"JasonYoong"},{"v":0},{"v":27}]},
      {"c":[{"v":"Rea_Alanna20"},{"v":25},{"v":0}]},
      ],
      "cols":[
      {"id":"1","label":"tweeter","type":"string"},
      {"id":"1","label":"retweets","type":"number"},
      {"id":"1","label":"tweets","type":"number"}
      ]
      };


      function drawChart() {
      var jsonData = jsonDataObj1;
      var data = new google.visualization.DataTable(jsonData);
      var options = {
      width: 800,
      height: 480,
      isStacked: true,
      title: 'Top tweeters before cleaning',
      colors: ['#003399', '#DCB2FE']
      };
      var chart = new google.visualization.BarChart(document.getElementById('chart_div1'));
      chart.draw(data, options);
      }
    </script>
    <script type="text/javascript">
      google.load("visualization", "1", {packages:["corechart"]});
      google.setOnLoadCallback(drawChart);
      var jsonDataObj = {
      "rows":[
      {"c":[{"v":"DiChristine"},{"v":66},{"v":1}]},
      {"c":[{"v":"MatthewTwihard"},{"v":60},{"v":0}]},
      {"c":[{"v":"rirapido1"},{"v":12},{"v":18}]},
      {"c":[{"v":"rrobertjimenez"},{"v":1},{"v":23}]},
      {"c":[{"v":"edwardistheman"},{"v":0},{"v":22}]},
      {"c":[{"v":"DisneyStudios"},{"v":17},{"v":4}]},
      {"c":[{"v":"DisneyMaddux"},{"v":21},{"v":0}]},
      {"c":[{"v":"mmdude1"},{"v":20},{"v":0}]},
      {"c":[{"v":"KristaLovesJian"},{"v":20},{"v":0}]},
      {"c":[{"v":"VivekSrkian33"},{"v":19},{"v":0}]},
      ],
      "cols":[
      {"id":"2","label":"tweeter","type":"string"},
      {"id":"2","label":"retweets","type":"number"},
      {"id":"2","label":"tweets","type":"number"}
      ]
      };


      function drawChart() {
      var jsonData = jsonDataObj;
      var data = new google.visualization.DataTable(jsonData);
      var options = {
      width: 800,
      height: 480,
      isStacked: true,
      title: 'Top tweeters after cleaning',
      colors: ['#003399', '#DCB2FE']
      };
      var chart = new google.visualization.BarChart(document.getElementById('chart_div2'));
      chart.draw(data, options);
      }
    </script>
    <!--barchart-->

    <script type="text/javascript">
      google.charts.load('current', {'packages':['corechart']});
      google.charts.setOnLoadCallback(drawChart);

      function drawChart() {
        var data = google.visualization.arrayToDataTable([
          ['Date', 'Volume'],
          ['01/01',  2557],
          ['02/01',  2349],
          ['03/01',  1410],
          ['04/01',  1228],
          ['05/01',  795],
          ['06/01',  869],
          ['06/01',  608],
          ['06/01',  378],
        ]);

        var options = {
          title: 'Timeline during 8 days',
          curveType: 'function',
          legend: 'none',
          colors:['#003399']
        };

        var chart = new google.visualization.LineChart(document.getElementById('curve_chart1'));

        chart.draw(data, options);
      }
    </script>
    <script type="text/javascript">
      google.charts.load('current', {'packages':['corechart']});
      google.charts.setOnLoadCallback(drawChart);

      function drawChart() {
        var data = google.visualization.arrayToDataTable([
          ['Date', 'Volume'],
          ['07:00',  25],
          ['08:00',  29],
          ['09:00',  20],
          ['10:00',  26],
          ['11:00',  27],
          ['12:00',  31],
          ['13:00',  32],
          ['14:00',  35],
          ['15:00',  56],
          ['16:00',  51],
          ['17:00',  81],
          ['18:00',  72],
          ['19:00',  104],
          ['20:00',  794],
          ['21:00',  679],
          ['22:00',  277],
          ['23:00',  218],
        ]);

        var options = {
          title: 'Timeline during 01/01',
          curveType: 'function',
          legend: 'none',
          colors:['#003399']
        };

        var chart = new google.visualization.LineChart(document.getElementById('curve_chart2'));

        chart.draw(data, options);
      }
    </script>
    <!--linechart-->
  </body>
</html>

                
