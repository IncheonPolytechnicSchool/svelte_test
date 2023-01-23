
  <head>
    <link rel="stylesheet" href="style.css">
    <script src="main.js"></script>
    <script src="js/includeHTML.js"></script>
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


    
<h1>#Study_ING</h1>
<p>study</p>
<input id="myInput" type="text" placeholder="Search">

<br>

<table>
    <thead>
        <tr>
            <th onclick="sortTable(0)">date <i class="fa fa-sort"></i></th> 
            <th onclick="sortTable(1)">time <i class="fa fa-sort"></i></th> 
            <th onclick="sortTable(2)">category1 <i class="fa fa-sort"></i></th>
            <th onclick="sortTable(3)">category2 <i class="fa fa-sort"></i></th>  
        </tr>
    </thead>
    <tbody id = "myTable">
        <tr>
            <td>2023-01-21</td>
            <td>03:57~05:44</td>
            <td>
                <span style="font-size: 2em; color: Dodgerblue;">
                <i class="fab fa-js"></i> 
                </span>
            <br>
            JavaScript
            </td>
            <td>google chart</td>
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
        
<script>
var coll = document.getElementsByClassName("collapsible");
var i;ƒ
            
for (i = 0; i < coll.length; i++) {
    coll[i].addEventListener("click", function() {
        this.classList.toggle("active");
        var content = this.nextElementSibling;
        if (content.style.maxHeight){
            content.style.maxHeight = null;
        } else {
            content.style.maxHeight = content.scrollHeight + "px";
        } 
    });
}
</script>
 
    </body>

