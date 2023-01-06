<head>
    
    <link rel="stylesheet" href="style.css">
    <script src="main.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin><link href="https://fonts.googleapis.com/css2?family=Source+Sans+Pro:ital@1&display=swap" rel="stylesheet">
    <script src="js/includeHTML.js"></script>
  </head>

<nav class="navbar">
    <div class="navbar__logo">
      <i class="fa fa-users"></i>
      <a class="white" href="index.html">Study</a>
    </div>

    <ul class="navbar__menu">
      <li>
        <div class="dropdown">
          <button class="dropbtn">Study
          <i class="fa fa-caret-down"></i>
        </button>
        <div class="dropdown-content">
          <a href="/code">code</a>
          <a href="pages/study_ing.html">ing</a>
          <a href="pages/book_complete.html">Book_Complete</a>
        </div>
      </div>
      </li>
      <li>
        <a class="white" 
             href="pages/exercise.html">
             Exercise
        </a>
      </li>
      <li>
        <div class="dropdown">
          <button class="dropbtn">Film
          <i class="fa fa-caret-down"></i>
        </button>
        <div class="dropdown-content">
          <a href="pages/film_history.html">History</a>
          <a href="pages/film_history_1945.html">1945</a>
        </div>
      </div>
      </li>
      <li>
        <div class="dropdown">
          <button class="dropbtn">0
          <i class="fa fa-caret-down"></i>
        </button>
        <div class="dropdown-content">
          <a href="pages/0_booking.html">booking</a>
          <a href="pages/0_goods.html">booking</a>
          <a href="pages/0_tiamo.htmm">tiamo</a>
        </div>
      </div>
      </li>
   </ul>

    <ul class="navbar__icons">
      <li><i class="fa fa-youtube"></i></li>
      <li><i class="fa fa-instagram"></i></li>
    </ul>
</nav>
<style>
  
.navbar {
  overflow: hidden;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #263343;
  padding: 8px 12px;
}

.navbar__logo {
  font-size: 24px;
  color: white;
}

.navbar__logo i {
  color: #d49466
}

.navbar__menu {
  display: flex;
  list-style: none;
  padding-left: 0;
}

.navbar__menu li {
  padding:8px 12px;
}

.navbar__menu li:hover, .dropdown:hover .dropbtn {
  background-color: #d49466;
  border-radius: 4px;
  
}

.navbar__icons {
  list-style: none;
  color: white;
  display: flex;
}

.navbar__icons li {
  padding: 8px 12px;
}

a.white {
text-decoration: none;
color: white;
}

.dropdown {
  float: left;
  overflow: hidden;
}

.dropdown .dropbtn {
  font-size: 16px;
  border: none;
  outline: none;
  color: white;
  background-color: inherit;
  font-family: inherit;
  margin: 0;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  float: none;
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown-content a:hover {
  background-color: #ddd;
}

.dropdown:hover .dropdown-content {
  display: block;
}
</style>
<slot></slot>
