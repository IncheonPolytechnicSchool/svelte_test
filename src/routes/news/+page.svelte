<head>
    
    <link rel="stylesheet" href="style.css">
    <script src="main.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin><link href="https://fonts.googleapis.com/css2?family=Source+Sans+Pro:ital@1&display=swap" rel="stylesheet">
    <script src="js/includeHTML.js"></script>
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
        box-shadow: 0 2px 2px -1px rgba(0, 0, 0, 0.4)
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
        background-color: #fcfadc;
    }
    tr:hover {
        background-color:#def3ff;
        color: black;
    }
    .special-image {
        border-radius: 15px;
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

    <h1>#Letter_Korean</h1>
    <input id="myInput" type="text" placeholder="search">
    <table>
        <thead>
        <tr>
          <th onclick="sortTable(0)">Journalist<br><i class="fa fa-sort"></i></th> 
          <th onclick="sortTable(1)">title<br><i class="fa fa-sort"></i></th> 
          <th onclick="sortTable(2)">category1<br><i class="fa fa-sort"></i></th>
        </tr>
        </thead>
        <tbody id = "myTable"> 
        <tr>
                <td>
                  <!-- svelte-ignore a11y-missing-attribute -->
                  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/75/The_Guardian_2018.svg/2880px-The_Guardian_2018.svg.png" 
                       width="100%">
                  <br>
                  The Guardian
                </td>
                <td>
                  <a href="https://www.theguardian.com/world/2018/aug/07/china-bans-winnie-the-pooh-film-to-stop-comparisons-to-president-xi">
                    <br>
                    China bans Winnie the Pooh film after comparisons to President Xi
                  </a>
                </td>
            <td>
                <span style="font-size: 2em; color: Dodgerblue;">
                    <i class="fa-solid fa-microphone-lines-slash"></i>
                </span>    
                <br>
                censorship
            </td>
               
            </tr>
            <tr>
              <td>
                <!-- svelte-ignore a11y-missing-attribute -->
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8d/Reuters_Logo.svg/2880px-Reuters_Logo.svg.png"
                     width="100%">
                <br>
                 Reuters
              </td>
              <td>
                <a href="https://www.reuters.com/article/us-japan-southkorea-wto/south-korea-wto-appeal-succeeds-in-japanese-fukushima-food-dispute-idUSKCN1RN24X">
                  <br>
                  South Korea WTO appeal succeeds in Japanese Fukushima food dispute
                </a>
              </td>
              <td>
                <span style="font-size: 2em; color: Dodgerblue;">
                    <i class="fa-solid fa-handshake-slash"></i>
                </span>
                <br>
                Diplomacy_Negative 
              </td>
            </tr>
            <tr>
                <td>
                  The Korean Times
                  <br>
                  <!-- svelte-ignore a11y-missing-attribute -->
                  <img class="special-image"
                       src="https://upload.wikimedia.org/wikipedia/commons/1/15/The_Korea_Times_logo.png"
                       width="70%">
                </td>
                <td>
                  <a href="https://www.koreatimes.co.kr/www/nation/2022/02/803_324616.html">
                    Presidential candidate apologizes for remarks on Ukraine's leader
                  </a>
                </td>
                <td>
                    <span style="font-size: 2em; color: Dodgerblue;">
                        <i class="fa-solid fa-user-slash"></i>
                    </span>
                    <br>
                    Person_Negative    
                </td>
            </tr>
            <tr>
                <td>CNN
                  <br>
                  <!-- svelte-ignore a11y-missing-attribute -->
                  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b1/CNN.svg/350px-CNN.svg.png" 
                       width="30%">
                </td>
                <td>
                  <a href="https://edition.cnn.com/2018/01/08/entertainment/natalie-portman-all-male-director/index.html">
                  <br>
                  Natalie Portman calls out 'all male nominees' for best director
                  </a>
                </td>
                    <td>
                        <!-- svelte-ignore a11y-missing-attribute -->
                        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Feminism_symbol.svg/2048px-Feminism_symbol.svg.png" 
                             width="100%">
                        <br>
                        Feminism
                      </td>
                </tr>
          </tbody>
</table>

<script>
    $(document).ready(function(){
      $("#myInput").on("keyup", function() {
        var value = $(this).val().toLowerCase();
        $("#myTable tr").filter(function() {
          $(this).toggle($(this).text().toLowerCase().indexOf(value) > -1)
        });
      });
    });
    function sortTable(n) {
      var table, rows, switching, i, x, y, shouldSwitch, dir, switchcount = 0;
      table = document.getElementById("myTable");
      switching = true;
      dir = "asc"; 
      while (switching) {
        switching = false;
        rows = table.rows;
        for (i = 0; i < (rows.length - 1); i++) {
          shouldSwitch = false;
          x = rows[i].getElementsByTagName("TD")[n];
          y = rows[i + 1].getElementsByTagName("TD")[n];
          if (dir == "asc") {
            if (x.innerHTML.toLowerCase() > y.innerHTML.toLowerCase()) {
              shouldSwitch= true;
              break;
            }
          } else if (dir == "desc") {
            if (x.innerHTML.toLowerCase() < y.innerHTML.toLowerCase()) {
              shouldSwitch = true;
              break;
            }
          }
        }
        if (shouldSwitch) {
          rows[i].parentNode.insertBefore(rows[i + 1], rows[i]);
          switching = true;
          switchcount ++;      
        } else {
          if (switchcount == 0 && dir == "asc") {
            dir = "desc";
            switching = true;
          }
        }
      }
    }
    </script>

</body>

