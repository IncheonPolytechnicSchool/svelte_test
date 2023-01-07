
  <head>
    
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin><link href="https://fonts.googleapis.com/css2?family=Source+Sans+Pro:ital@1&display=swap" rel="stylesheet">
    <style>
        table {
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width: 100%;
  font-size:4vw;
}

th {
  border: 1px solid #dddddd;
  border-radius: 50% 20% / 10% 40%;
  text-align: center;
  padding: 1px;
  background-color: #041a4f;
  cursor: pointer;
  color: white;
  position: sticky;
  top: 0; 
  box-shadow: 0 2px 2px -1px rgba(0, 0, 0, 0.4);
}

th:hover {
    background-color:#041a4f;
    color: white;    

  }
  
td{
   text-align: center;
   padding: 1px;
    border: 2px solid #000000;
  }

tr:nth-child(even) {
  background-color: #fcfadc
  ;
}
  
tr:hover {
    background-color:#def3ff;
    color: black;      
}

.special-image {
    border-radius: 15px;
}

.collapsible {
  background-color: #777;
  color: white;
  cursor: pointer;
  padding: 18px;
  width: 100%;
  border: none;
  text-align: left;
  outline: none;
  font-size: 15px;
}

.active, .collapsible:hover {
  background-color: #555;
}

.content {
  padding: 0 18px;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.2s ease-out;
  background-color: #f1f1f1;
}

body {
  margin: 0;
  font-family: 'Source Sans Pro', sans-serif;
}
    </style>

  </head>

<body>
    <h1>Exercise</h1>
    <table>
        <thead>
            <tr>
                <th>C</th>
                <th>C</th> 
                <th>C</th>
                <th>C</th>
                <th>N</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>
                    <span style="font-size: 2em; color: Dodgerblue;">
                        <i class="fa-solid fa-football"></i>
                    </span>
                    <br>
                    American Football
                </td>
                <td>
                    <!-- svelte-ignore a11y-missing-attribute -->
                    <img src="https://upload.wikimedia.org/wikipedia/en/thumb/a/a2/National_Football_League_logo.svg/1024px-National_Football_League_logo.svg.png" 
                         width="50%">
                    <br>
                    NFL
                </td>
                <td>
                     <!-- svelte-ignore a11y-missing-attribute -->
                     <img class="special-image"
                          src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5d/Touchdown_--_Texas_High_School_vs_Highland_Park_High_School_first-round_playoffs.jpg/1920px-Touchdown_--_Texas_High_School_vs_Highland_Park_High_School_first-round_playoffs.jpg" 
                          width="100%">
                     <br>
                     Touch Down
                </td>
                <td></td>
                <td>5</td>
            </tr>
            <tr>
                <td>
                    <span style="font-size: 2em; color: Dodgerblue;">
                        <i class="fa-solid fa-gamepad"></i>
                    </span>
                    <br>
                    E-Sports
               </td>
               <td>
               <!-- svelte-ignore a11y-missing-attribute -->
               <img class="special-image" 
                     src="https://upload.wikimedia.org/wikipedia/commons/e/e6/Faker_at_the_2015.10.02_S5_Paris_day2.jpeg" 
                     width="50%">
               <br>
               Faker
              </td>
              <td>
                VS Chovy
              </td>
              <td></td>
              <td>4</td>
            </tr>
            <tr>
                <td>
                    <span style="font-size: 2em; color: Dodgerblue;">
                        <i class="fas fa-car"></i>
                    </span>
                    <br>
                    Motorsports
                </td>
                <td>
                    <!-- svelte-ignore a11y-missing-attribute -->
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/33/F1.svg/2880px-F1.svg.png" 
                         width="100%">
                    <br>
                    F1
                </td>
                <td>
                    <!-- svelte-ignore a11y-missing-attribute -->
                    <img class="special-image" 
                         src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ab/2011_Italian_GP_-_Vettel.jpg/2880px-2011_Italian_GP_-_Vettel.jpg" 
                         width="100%">
                    <br>
                    Red Bull
                </td>
                <td>
                    <!-- svelte-ignore a11y-missing-attribute -->
                    <img class="special-image"
                         src="https://upload.wikimedia.org/wikipedia/commons/7/75/Max_Verstappen_2017_Malaysia_3.jpg" 
                         width="100%">
                    <br>
                    Max Verstappen
                </td>
                <td>6</td>
              </tr>
              <tr>
                <td>
                    <span style="font-size: 2em; color: Dodgerblue;">
                        <i class="fa-solid fa-baseball-bat-ball"></i>
                    </span>
                    <br>
                    Baseball
                </td>
                <td>
                    <!-- svelte-ignore a11y-missing-attribute -->
                    <img class="special-image" 
                         src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1f/Ohtani_2018.jpg/1280px-Ohtani_2018.jpg" 
                         width="100%">
                    <br>
                    Shohei Ohtani
                </td>
                <td>
                    <span style="font-size: 2em; color: Dodgerblue;">
                        <i class="fa-solid fa-baseball"></i>
                    </span>
                    <br>
                    pitcher
                </td>
                <td></td>
                <td>35</td>
              </tr>
              <tr>
                <td>
                    <span style="font-size: 2em; color: Dodgerblue;">
                        <i class="fa-solid fa-futbol"></i>
                    </span>
                    <br>
                    Association football
                </td>
                <td>
                    金玟哉
                    <br>
                    <!-- svelte-ignore a11y-missing-attribute -->
                    <img class="special-image" 
                         src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/84/%ED%86%A0%ED%8A%B8%EB%84%98-%EC%9C%A0%EB%B2%A4%ED%88%AC%EC%8A%A4_%EC%9D%B4%EC%A0%81%EC%84%A4%EC%97%90_%EC%A7%81%EC%A0%91_%EB%8B%B5%ED%95%9C_%EA%B9%80%EB%AF%BC%EC%9E%AC_1m_42s.jpg/440px-%ED%86%A0%ED%8A%B8%EB%84%98-%EC%9C%A0%EB%B2%A4%ED%88%AC%EC%8A%A4_%EC%9D%B4%EC%A0%81%EC%84%A4%EC%97%90_%EC%A7%81%EC%A0%91_%EB%8B%B5%ED%95%9C_%EA%B9%80%EB%AF%BC%EC%9E%AC_1m_42s.jpg" 
                         width="50%">
                  </td>
                <td>
                  UEFA
                  <br>
                  Europa League
                  <br>
                  <img src="https://upload.wikimedia.org/wikipedia/en/thumb/7/77/UEFA_Europa_League_%28football_competition%29_logo.svg/1024px-UEFA_Europa_League_%28football_competition%29_logo.svg.png" width="30%">
                </td>
                  <td>
                  </td>
                  <td>17</td> 
              </tr>
              <tr>
                <td>
                  hitter
                <br>
                <img class="special-image"
                     src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/af/Ohtani_batting_2019.08.04%283%29.jpg/800px-Ohtani_batting_2019.08.04%283%29.jpg" 
                     width="50%">
                </td>
                <td></td>
                <td>19</td>
              </tr>
    <tr>
    <td>
      Interception
      <br>
      <img class="special-image" 
           src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/09/Football_interception.jpg/440px-Football_interception.jpg" 
           width="50%">
    </td>
    <td></td>
    <td>4</td>
  </tr>
  <tr>
    <td>
    Sergio Pérez
    <br>
    <img class="special-image" 
         src="https://upload.wikimedia.org/wikipedia/commons/7/7a/Sergio_P%C3%A9rez_2019_%28cropped%29.jpg" 
         width="50%">
    </td>
    <td>6</td>
  </tr>
  <tr>
    <td>
      F1
      <br>
      <img class="special-image" 
           src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/33/F1.svg/2880px-F1.svg.png" 
           width="50%">
    </td>
    <td>
      Pit Stop
      <br>
      <img class="special-image" 
           src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c9/2012_Italian_GP_-_Ferrari_pit.jpg/1920px-2012_Italian_GP_-_Ferrari_pit.jpg" 
           width="70%">
    </td>
    <td></td>
    <td>6</td>
  </tr>
  <tr>
    <td style="background-color:#f2c0bd">
      LPL
      <br>
      <img src="https://upload.wikimedia.org/wikipedia/en/thumb/b/b4/League_of_legends_pro_league_logo.svg/440px-League_of_legends_pro_league_logo.svg.png" 
           width="30%">
    </td>
    <td style="background-color:#f2c0bd">
      Royal Never
      <br>
      Give Up
      <br>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/63/RNG_logo.svg/1920px-RNG_logo.svg.png" 
           width="30%">
    </td>
    <td></td>
    <td>94</td>
  </tr>
  <tr>
    <td rowspan="3">
      The Korean Zombie
      <br>
      <img class="special-image" 
           src="https://upload.wikimedia.org/wikipedia/commons/6/66/Jung_Chan-Sung_from_acrofan_%282%29.jpg" 
           width="50%">
    </td>
    <td>
      Zombie Trip:Looking for a fighter
      <br>
      <img class="special-image" 
           src="https://i.ytimg.com/vi/Exk36_ZiHQs/hqdefault.jpg?sqp=-oaymwEXCNACELwBSFryq4qpAwkIARUAAIhCGAE=&rs=AOn4CLAsgRYxrjYjGmGzP7FQBYxM-vbo_g" 
           width="80%">
    </td>
    <td></td>
    <td>27</td>
  </tr>
  <tr>
    <td rowspan="2">
      UFC
      <br>
      <img class="special-image" 
           src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/92/UFC_Logo.svg/440px-UFC_Logo.svg.png"
           width="80%">
    </td>
    <td>
      cornerman
      <br>
      <img class="special-image"
           src="https://upload.wikimedia.org/wikipedia/en/thumb/7/7c/Corner_person.jpg/440px-Corner_person.jpg"
           width="80%">
    </td>
    <td>17</td>
  </tr>
  <tr>
    <td>Fighter</td>
    <td>0</td>
  </tr>
  <tr>
    <td rowspan="2">
      East Asian
      <br>
      (Except Korean)
      <br>
      <img class="special-image" 
           src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ab/East_Asia_%28orthographic_projection%29.svg/440px-East_Asia_%28orthographic_projection%29.svg.png"
           width="50%">
    </td>
    <td>
      Shohei Ohtani
      <br>
      <img class="special-image"
           src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/12/Shohei_Ohtani_%2848343515351%29_%28cropped%29.jpg/800px-Shohei_Ohtani_%2848343515351%29_%28cropped%29.jpg"
           width="50%">
    </td>
    <td></td>
    <td>59</td>
  </tr>
  <tr>
    <td>
      Yu Darvish
      <br>
      <img class="special-image"
           src="https://upload.wikimedia.org/wikipedia/commons/8/89/Yu_Darvish_8.27.21.jpg"
           width="50%">
    </td>
    <td></td>
    <td>3</td>
  </tr>
  <tr>
    <td rowspan="2">
      Silver Slugger 
      <br>
      <img class="special-image" 
           src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/97/Rizzo_with_Silver_Slugger.jpg/1024px-Rizzo_with_Silver_Slugger.jpg" 
           width="50%">
    </td>
    <td>
      Shohei Ohtani
      <br>
      <img class="special-image"
           src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/12/Shohei_Ohtani_%2848343515351%29_%28cropped%29.jpg/800px-Shohei_Ohtani_%2848343515351%29_%28cropped%29.jpg" 
           width="50%">
    </td>
    <td></td>
    <td>59</td>
  </tr>
  <tr>
    <td>


    Aaron Judge
    <br>
    <img class="special-image"
         src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a6/Aaron_Judge_2018.jpg/1280px-Aaron_Judge_2018.jpg" 
         width="50%">
  </td>
  <td></td>
  <td>8</td>
</tr>
<tr>
  <td>
    UEFA Champions League
    <br>
    <img class="special-image"
         src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/UEFA_Champions_League_logo.svg/2880px-UEFA_Champions_League_logo.svg.png" 
         width="60%">
  </td>
  <td></td>
  <td></td>
  <td>58</td>
</tr>
<tr>
  <td>
    Mid-Season
    <br>
    Invitational
    <br>
    <img class="special-image" 
         src="https://upload.wikimedia.org/wikipedia/en/thumb/e/e7/LOL_MSI_logo.svg/1280px-LOL_MSI_logo.svg.png"
         width="30%">
  </td>
  <td>
    LCK
    <br>
    <img class="special-image"
         src="https://upload.wikimedia.org/wikipedia/en/thumb/1/13/League_of_Legends_Champions_Korea_logo.svg/440px-League_of_Legends_Champions_Korea_logo.svg.png"
         width="30%">
  </td>
  <td style="background-color:#f2c0bd">
    LPL
    <br>
    <img class="special-image"
         src="https://upload.wikimedia.org/wikipedia/en/thumb/b/b4/League_of_legends_pro_league_logo.svg/440px-League_of_legends_pro_league_logo.svg.png" 
         width="30%">
  </td>
  <td>37</td>
</tr>
<tr>
  <td>
    K League 1
    <br>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5a/K_League_1_Crest.svg/280px-K_League_1_Crest.svg.png" 
         width="30%">
  </td>
  <td>
    <a href="https://en.wikipedia.org/wiki/Promotion_and_relegation">
      Promotion and relegation
    </a>
  </td>
  <td></td>
  <td>24</td>
</tr>
    <tr>
        <td>權純雨
           <br>
           <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/84/Kwon_RG22_%2821%29_%2852144070731%29.jpg/800px-Kwon_RG22_%2821%29_%2852144070731%29.jpg" alt="Royal Never Give Up" width="30%"></td>
        <td></td>
        <td></td>
        <td>24</td>
    </tr>
    <tr>
        <td>The 
          <br>
          Championships,
          <br>
          Wimbledon
          <br>
          <img src="https://upload.wikimedia.org/wikipedia/en/thumb/b/b9/Wimbledon.svg/1280px-Wimbledon.svg.png" width="30%">
        </td>
        <td></td>
        <td></td>
        <td>24</td>
    </tr>
    <tr>
      <td style="background-color:#f2c0bd">
        Novak
        <br>
        Djokovic
        <br>
        <img src="https://upload.wikimedia.org/wikipedia/commons/4/48/Novak_Djokovi%C4%87_Trophy_Wimbledon_2019-croped_and_edited.jpg" alt="Royal Never Give Up" width="30%"></td>
      <td></td>
      <td></td>
      <td>24</td>
    </tr>
      <tr>
    <tr>
      <td>
        <a class="black"
           href="https://en.wikipedia.org/wiki/Japan%E2%80%93South_Korea_sports_rivalries">
          Japan–South 
          <br>
          Korea sports
          <br>
          rivalries
        </a>
      </td>
        <td>
          South Korea
          <br>
          <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/09/Flag_of_South_Korea.svg/1920px-Flag_of_South_Korea.svg.png" width="30%">
        </td>
        <td>
          Japan
          <br>
          <img src="https://upload.wikimedia.org/wikipedia/en/thumb/9/9e/Flag_of_Japan.svg/1920px-Flag_of_Japan.svg.png" width="30%">
        </td>
        <td>12</td> 
    </tr>
      <tr>
        <td style="background-color:#f2c0bd">
          DetonatioN
          <br>
          Gaming
          <br>
            <img src="https://upload.wikimedia.org/wikipedia/en/7/74/DetonatioN_Gaming_logo.png" width="30%">
          </td>
          <td></td>
          <td></td>
          <td>12</td>
      </tr>
      <tr>
        <td>
          <a href="https://en.wikipedia.org/wiki/Liverpool_F.C.%E2%80%93Manchester_City_F.C._rivalry">
            Liverpool F.C.
            <br>
            –Manchester City 
            <br>
            F.C. rivalry
            <br>
            <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/20180607_075505_-_Flickr_-_7beachbum.jpg" width="60%">
          </a>
        </td>
          <td>
            Liverpool F.C 
            <br>
            <img src="https://upload.wikimedia.org/wikipedia/en/thumb/0/0c/Liverpool_FC.svg/1024px-Liverpool_FC.svg.png" width="60%">
          </td>
          <td>
            Manchester 
            <br>
            City F.C. 
            <br>
            <img src="https://upload.wikimedia.org/wikipedia/en/thumb/e/eb/Manchester_City_FC_badge.svg/1280px-Manchester_City_FC_badge.svg.png" width="60%">
          </td>
          <td>13</td>\
      </tr>
      <tr>
        <td>
          <a href="https://edition.cnn.com/2022/04/11/football/manchester-city-liverpool-rivalry-premier-league-spt-intl/index.html">
            Pep Guardiola
            <br>
            [VS] 
            <br>
            Jürgen Klopp
          </a>
        </td>
          <td>
            Pep Guardiola
            <br>
            <img src="https://upload.wikimedia.org/wikipedia/commons/b/be/Pep_2017_%28cropped%29.jpg" width="30%">
          </td>
          <td>
            Jürgen Klopp
            <br>
            <img src="https://upload.wikimedia.org/wikipedia/commons/8/81/J%C3%BCrgen_Klopp%2C_Liverpool_vs._Chelsea%2C_UEFA_Super_Cup_2019-08-14_04.jpg" width="30%">
          </td>
          <td>13</td>
      </tr>
      <tr>
        <td>
          <a href="https://en.wikipedia.org/wiki/Japan%E2%80%93South_Korea_football_rivalry">
            Japan–South
            <br>
            Korea
            <br>
            football rivalry
          </a>
        </td>
          <td>
            South Korea national football team
            <br>
            <img src="https://upload.wikimedia.org/wikipedia/en/f/f8/South_Korea_national_football_team.png" width="30%">
          </td>
          <td>
            Japan national football team
            <br>
            <img src="https://upload.wikimedia.org/wikipedia/en/thumb/8/84/Japan_national_football_team_crest.svg/1024px-Japan_national_football_team_crest.svg.png" width="30%">
          </td>
          <td>8</td>
      </tr>
      <tr>
        <td>
           UEFA Champions League
           <br>
           <img src="https://upload.wikimedia.org/wikipedia/en/thumb/b/bf/UEFA_Champions_League_logo_2.svg/400px-UEFA_Champions_League_logo_2.svg.png" width="60%">
        </td>
        <td>
          Serie A
          <br>
          <img src="https://upload.wikimedia.org/wikipedia/en/thumb/c/c5/Logo_Serie_A_TIM_2021.svg/1024px-Logo_Serie_A_TIM_2021.svg.png" width="60%">
       </td>
         <td></td>
         <td>6</td>
     </tr>
      <tr>
        <td><a href="https://en.wikipedia.org/wiki/Iran%E2%80%93South_Korea_football_rivalry">
          Iran–South Korea 
          <br>
          football rivalry</a></td>
        <td>
          South Korea national football team
          <br>
          <img src="https://upload.wikimedia.org/wikipedia/en/f/f8/South_Korea_national_football_team.png" width="30%">
        </td>
        <td>
          Iran national football team
          <br>
          <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/ca/Flag_of_Iran.svg/2560px-Flag_of_Iran.svg.png" width="30%">
        </td>
        <td>5</td>
   </tr>
   <tr>
    <td rowspan="2">
      No.9
    </td>
    <td>Erling Haaland
      <br>
      <img class="special-image" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fe/FC_RB_Salzburg_versus_SV_Mattersburg_%284._Juli_2019%29_29.jpg/800px-FC_RB_Salzburg_versus_SV_Mattersburg_%284._Juli_2019%29_29.jpg" alt="Royal Never Give Up" width="30%">
    </td>
    <td></td>
    <td>5</td>
</tr>
  <td>
    Karim Benzema
    <br>
    <img class="special-image" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/Karim_Benzema_wearing_Real_Madrid_home_kit_2021-2022.jpg/440px-Karim_Benzema_wearing_Real_Madrid_home_kit_2021-2022.jpg" width="50%">
  </td>
  <td></td>
  <td>7</td>
    <tr>
      <td>El Clásico
        <br>
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f8/RealMadrid-Barcelona.svg/1920px-RealMadrid-Barcelona.svg.png" alt="Royal Never Give Up" width="30%">
      </td>
      <td>
        Real Madrid
        <br>
        CF
        <br>
        <img src="https://upload.wikimedia.org/wikipedia/en/thumb/5/56/Real_Madrid_CF.svg/1024px-Real_Madrid_CF.svg.png" alt="Royal Never Give Up" width="30%">
      </td>
      <td>FC Barcelona
        <br>
        <img src="https://upload.wikimedia.org/wikipedia/en/thumb/4/47/FC_Barcelona_%28crest%29.svg/1280px-FC_Barcelona_%28crest%29.svg.png" alt="Royal Never Give Up" width="30%">
      </td>
      <td>5</td>
  </tr>
    <tr>
      <td>FC Barcelona
        <br>
        <img src="https://upload.wikimedia.org/wikipedia/en/thumb/4/47/FC_Barcelona_%28crest%29.svg/1280px-FC_Barcelona_%28crest%29.svg.png" alt="Royal Never Give Up" width="30%">
      </td>
      <td></td>
      <td></td>
      <td>5</td>
  </tr>
  <tr>
    <td style="background-color:#f2c0bd">
      Real Madrid 
      <br>
      CF
      <br>
      <img src="https://upload.wikimedia.org/wikipedia/en/thumb/5/56/Real_Madrid_CF.svg/1024px-Real_Madrid_CF.svg.png" alt="Royal Never Give Up" width="30%">
    </td>
    <td></td>
    <td></td>
    <td>5</td>
</tr>
<tr>
<tr>
  <td>
    Twitch
    <br>
    <img class="special-image" src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/ce/Twitch_logo_2019.svg/2880px-Twitch_logo_2019.svg.png" width="50%">
  </td>
  <td>
    Starcraft
    <br>
    <img class="special-image" src="https://upload.wikimedia.org/wikipedia/commons/0/0a/StarCraft_Logo.png" width="50%">
  </td>
  <td>
  </td>
  <td>5</td>
</tr>
<tr>
  <td rowspan="2">
    Starcraft
    <br>
    <img class="special-image" src="https://upload.wikimedia.org/wikipedia/commons/0/0a/StarCraft_Logo.png" width="50%">
  </td>
  <td>
    The Protoss
    <br>
    <img class="scpecial-image" src="https://upload.wikimedia.org/wikipedia/en/8/8f/Zealot_%28StarCraft%29.png" width="50%">
  </td>
  <td>
  </td>
  <td>5</td>
</tr>
<tr>
  <td style="background-color:#f2c0bd">
    The Zerg
    <br>
    <img class="special-image" src="https://upload.wikimedia.org/wikipedia/en/b/be/Hydralisk_%28StarCraft%29.png" width="50%">
  </td>
  <td>
  </td>
  <td>5</td>
    </tbody>
  </table>
</body>