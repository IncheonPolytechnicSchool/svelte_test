<head>
    
    <link rel="stylesheet" href="style.css">
    <script src="main.js"></script>
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
          <th onclick="sortTable(0)">Y<br><i class="fa fa-sort"></i></th> 
          <th onclick="sortTable(1)">M<br><i class="fa fa-sort"></i></th> 
          <th onclick="sortTable(2)">D<br><i class="fa fa-sort"></i></th>
          <th onclick="sortTable(3)">T<br><i class="fa fa-sort"></i></th>
          <th onclick="sortTable(4)">F<br><i class="fa fa-sort"></i></th>
          <th onclick="sortTable(5)">C1<br><i class="fa fa-sort"></i></th>
          <th onclick="sortTable(6)">C2<br><i class="fa fa-sort"></i></th>
        </tr>
        </thead>
        <tbody id = "myTable"> 
            <tr>
                <td>2023</td>
                <td>01</td>
                <td>20</td>
                <td>
                  21
                  <br>
                  :00
                </td>
                <td>
                  <!-- svelte-ignore a11y-missing-attribute -->
                  <img class="special-image" 
                       src = "https://upload.wikimedia.org/wikipedia/commons/e/e2/%EB%B0%B0%EC%84%B1%EC%9E%AC%EC%9D%98_%ED%85%90_%EC%B6%9C%EC%97%B0_%EC%B9%A8%EC%B0%A9%EB%A7%A8.jpg" 
                       width="100%">
                  <br>
                  Calm Down Man
                </td>
                <td>
                  BDRZ
                </td>
                <td>
                  <!-- svelte-ignore a11y-missing-attribute -->
                  <img class="special-image" 
                       src = "https://upload.wikimedia.org/wikipedia/en/4/4e/KR-logo-BlackBlue.png" 
                       width="100%">
                </td>
            </tr>
            <tr>
              <td>2023</td>
              <td>01</td>
              <td>20</td>
              <td>
                22
                <br>
                :00
              </td>
              <td>
                <!-- svelte-ignore a11y-missing-attribute -->
                <img class="special-image" 
                     src = "https://upload.wikimedia.org/wikipedia/commons/e/e2/%EB%B0%B0%EC%84%B1%EC%9E%AC%EC%9D%98_%ED%85%90_%EC%B6%9C%EC%97%B0_%EC%B9%A8%EC%B0%A9%EB%A7%A8.jpg" 
                     width="100%">
                <br>
                Calm Down Man
              </td>
              <td>
                BDRZ
              </td>
              <td>
                Goose Goose Duck
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

