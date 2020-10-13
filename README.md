
<!DOCTYPE html>
<html>
<style>

/* Full-width input fields */

input[type=text],
input[type=password] {
    width: 100%;
    padding: 12px 20px;
    margin: 8px 0;
    display: inline-block;
    border: 1px solid #ccc;
    box-sizing: border-box;
}

/* Set a style for all buttons */

button {
    background-color: #48d1cc;
    color: white;
    padding: 14px 20px;
    margin: 8px 0;
    border: none;
    cursor: pointer;
    width: 100%;
}

.cancelbtn {
    width: auto;
    padding: 10px 18px;
    background-color: #4682b4;
}

/* Center the image and position
the close button */

.imgcontainer {
    text-align: center;
    margin: 24px 0 12px 0;
    position: relative;
}

img.avatar {
    width: 40%;
    border-radius: 50%;
}

.container {
    padding: 16px;
}

span.psw {
    float: right;
    padding-top: 16px;
}

/* The Modal (background) */

.modal {
   display: none;
   position: fixed;
   z-index: 1;
   left: 0;
   top: 0;
   width: 100%;
   height: 100%;
   overflow: auto;
   background-color: rgb(0,0,0);
   background-color: rgba(0,0,0,0.4);
   padding-top: 60px;
}

.modal-content {
    background-color: #fefefe;
    margin: 5% auto 15% auto;
    border: 1px solid #888;
    width: 80%;
}

/* The Close Button (x) */

.close {
    position: absolute;
    right: 25px;
    top: 0;
    color: #000;
    font-size: 35px;
    font-weight: bold;
}

.close:hover,
.close:focus {
    color: red;
    cursor: pointer;
}

/* Add Zoom Animation */

.animate {
-webkit-animation: animatezoom 0.6s;
animation: animatezoom 0.6s
}

@-webkit-keyframes animatezoom {
from {-webkit-transform: scale(0)}
to {-webkit-transform: scale(1)}
}

@keyframes animatezoom {
    from {transform: scale(0)}
    to {transform: scale(1)}
}

/* Change styles for span and cancel
button on extra small screens */

@media screen and(max-width: 300px){
    span.psw {
       display: block;
       float: none;
    }
    .cancelbtn {
       width: 100%;
    }
}
</style>
<body>

<h2> Znakekele Health Clinic</h2>

<button onclick="document.
getElementById('id01')

.style.display='block'"
style="width:auto;">Login
</button>

<div id="id01" class="modal">

<form class="modal-content animate"
action="action_page.php">
<div class="imgcontainer">
<span onclick="document
.getElementById('id01')

.style.display='none'"
class="close" title="Close Modal">
    &times;</span>

<img src="img_profile.png"
alt="Avatar"
class="avatar">
    </div>

<div class="container">
  <label><b>Username</b></label>
  <input type="text" placeholder=
  "Enter Username"
  name="uname" required>

<label><b>Password</b></label>
<input type="password" placeholder=
"Enter Password" name="psw" required>

<button type="submit">Login</button>
<input type="checkbox"
checked="checked">
Remember me
</div>

<div class="container"
style="background-color:#f1f1f1">
<button type="button"
onclick="document.getElementById
('id01').style.

display='none'" class="cancelbtn">
Cancel</button>
<span class="psw">Forgot
<a href="#">password?

</a></span>
  </div>
  </form>
</div>

<script>

// Get the modal

var modal = document.getElementById
('id01');

// When the user clicks anywhere
outside of the modal, close it

window.onclick = function(event) {
    if (event.target == modal) {
     modal.style.display = "none";
    }
}
</script>

</body>
</html>


 
<!DOCTYPE html>
<html>
<head>
<style>

#myInput {
  background-image:
  url('/img/search.png');

  background-position: 10px 12px;
  background-repeat: no-repeat;
  box-sizing: border-box;
  width: 100%;
  font-size: 16px;
  padding: 12px 20px 12px 40px;
  border: 1px solid #ddd;
  margin-bottom: 12px;
}

#myUL {
  list-style-type: none;
  padding: 0;
  margin: 0;
}

#myUL li a {
  border: 1px solid #ddd;
  margin-top: -1px;
  background-color: #f6f6f6;
  padding: 12px;
  text-decoration: none;
  font-size: 18px;
  color: black;
  display: block
}

#myUL li a.header {
  background-color: #e2e2e2;
  cursor: default;
}

#myUL li a:hover:not(.header) {
  background-color: #eee;
}

</style>

</head>

<body>

<h2>PATIENTS LIST</h2>

<input type="text" id="myInput"
onkeyup="myFunction()" placeholder=
"Search Here.."title="Type in a name">

<ul id="myUL">

<li><a href="#" class="header">A</a></li>
<li><a href="#">Abel</a></li>
<li><a href="#">Akgonne</a></li>
<li><a href="#">Ajela</a></li>

<li><a href="#" class="header">B</a></li>
<li><a href="#">Badimo</a></li>
<li><a href="#">Bagaka</a></li>

<li><a href="#" class="header">C</a></li>
<li><a href="#">Cheka</a></li>
<li><a href="#">Chuku</a></li>
<li><a href="#">Chaka</a></li>

</ul>

<script>

/* Declare variables */

function myFunction() {

var input, filter, ul, li, a, i;
input=document.getElementById("myInput");
filter = input.value.toUpperCase();
ul = document.getElementById("myUL");
li = ul.getElementsByTagName("li");

/* Loop through all list items, and hide
those who don't match the search query */

for (i = 0; i < li.length; i++) {
a = li[i].getElementsByTagName("a")[0];

if (a.innerHTML.toUpperCase()
.indexOf(filter) > -1) {
  li[i].style.display = "";

    } else {
      li[i].style.display = "none";

        }
    }
}

</script>

</body>
</html>




<!DOCTYPE html>
<html>
<head>
<style>

.dropbtn {
    background-color: #48d1cc;
    color: white;
    padding: 16px;
    font-size: 16px;
    border: none;
    cursor: pointer;
}

.dropbtn:hover, .dropbtn:focus {
    background-color: #7effa5;
}

#myInput {
  border-box: box-sizing;
  background-image:url('search.png');
  background-position: 14px 12px;
  background-repeat: no-repeat;
  font-size: 16px;
  padding: 14px 20px 12px 45px;
  border: none;
}

.dropdown {
    position: relative;
    display: inline-block;
}

.dropdown-content {
    display: none;
    position: absolute;
    background-color: #f6f6f6;
    min-width: 230px;
    overflow: auto;
    box-shadow: 0px 8px 16px 0px
    rgba(0,0,0,0.2);
}

.dropdown-content a {
    color: black;
    padding: 12px 16px;
    text-decoration: none;
    display: block;
}

.dropdown a:hover
{background-color: #ddd}

.show {display:block;}

</style>
</head>
<body>

<h2>Znakekele Patients Treatments</h2>
<p>Click on the button to open the
dropdown menu,and use the input field
to search for a specific
dropdown link.</p>

<div class="dropdown">

<button onclick="myFunction()"
class="dropbtn">Dropdown</button>

<div id="myDropdown"
class="dropdown-content">

<input type="text"
placeholder="Search.."
id="myInput"onkeyup="filterFunction()">
    <a href="#about">About</a>
    <a href="#base">Base</a>
    <a href="#blog">Blog</a>
    <a href="#contact">Contact</a>
    <a href="#custom">Custom</a>
    <a href="#support">Support</a>
    <a href="#">Medication</a>
  </div>

</div>

<script>

function myFunction() {
document.getElementById("myDropdown")
.classList.toggle("show");
}

function filterFunction() {
  var input, filter, ul, li, a, i;

  input = document.getElementById
  ("myInput");

  filter = input.value.toUpperCase();

  div = document.getElementById
  ("myDropdown");

  a = div.getElementsByTagName("a");

  for (i = 0; i < a.length; i++) {

  if (a[i].innerHTML.toUpperCase()
  .indexOf(filter) > -1) {

           a[i].style.display = "";
        } else {
          a[i].style.display="none";
        }
    }
}

</script>

</body>
</html>

<html>
<head>

<style>

body {
  margin: 0;
  min-width: 250px;
}

ul {
  margin: 0;
  padding: 0;
}

ul li {
  cursor: pointer;
  position: relative;
  padding: 12px 8px 12px 40px;
  background: #eee;
  font-size: 18px;
  transition: 0.2s;

  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

ul li:nth-child(odd) {
  background: #f9f9f9;
}

ul li:hover {
  background: #ddd;
}

ul li.checked {
  background: #888;
  color: #fff;
  text-decoration: line-through;
}

ul li.checked::before {
  content: '';
  position: absolute;
  border-color: #fff;
  border-style: solid;
  border-width: 0 2px 2px 0;
  top: 10px;
  left: 16px;
  transform: rotate(45deg);
  height: 15px;
  width: 7px;
}

.close {
  position: absolute;
  right: 0;
  top: 0;
  padding: 12px 16px 12px 16px
}

.close:hover {
  background-color: #f44336;
  color: white;
}

.header {
  background-color: #00b867;
  padding: 30px 40px;
  color: white;
  text-align: center;
}

.header:after {
  content: "";
  display: table;
  clear: both;
}

input {
  border: none;
  width: 75%;
  padding: 10px;
  float: left;
  font-size: 16px;
  box-sizing: border-box;

}

.addBtn {
  padding: 10px;
  box-sizing: border-box;
  width: 25%;
  background: #d9d9d9;
  color: #555;
  float: left;
  text-align: center;
  font-size: 16px;
  cursor: pointer;
  transition: 0.3s;
}

.addBtn:hover {
  background-color: #bbb;
}

</style>
</head>

<body>

<div id="myDIV" class="header">

<h2 style="margin:5px"> To Do List
Medication</h2>

<input type="text" id="myInput"
placeholder="Title...">

<span onclick="newElement()"
class="addBtn">Add</span>

</div>

<ul id="myUL">

  <li>Panado</li>
  <li class="checked">Bruffen</li>
  <li>Cough Mixture</li>
  <li>High Blood Pressure</li>
  <li>Other Pills</li>
  <li>Other Medication</li>

</ul>

<script>

var myNodelist = document
.getElementsByTagName("LI");

var i;
for(i=0; i < myNodelist.length;i++){
var span=document.createElement
("SPAN");

var txt=document.createTextNode
("\u00D7");

span.className = "close";
span.appendChild(txt);
myNodelist[i].appendChild(span);
}

var close = document
.getElementsByClassName("close");
var i;

for(i=0; i < close.length;i++){
  close[i].onclick = function() {
    var div = this.parentElement;
    div.style.display = "none";
  }
}

var list=document.querySelector('ul');
list.addEventListener('click',
function(ev) {
if (ev.target.tagName === 'LI') {
ev.target.classList.toggle('checked');
  }
}, false);

function newElement() {
var li=document.createElement("li");

var inputValue=document
.getElementById("myInput").value;

var t = document.createTextNode
(inputValue);

li.appendChild(t);
if (inputValue === '') {
alert("You must write something!");
  } else {
    document.getElementById("myUL")
    .appendChild(li);
  }
  document.getElementById("myInput")
  .value = "";

var span=document.createElement
("SPAN");

var txt=document.createTextNode
("\u00D7");

  span.className = "close";
  span.appendChild(txt);
  li.appendChild(span);

for (i = 0; i < close.length; i++) {
    close[i].onclick = function() {
      var div = this.parentElement;
      div.style.display = "none";
    }
  }
}

</script>

</body>
</html>




<!DOCTYPE html>
<html>
<head>
<style>

button.accordion {
    background-color: #eee;
    color: #444;
    cursor: pointer;
    padding: 18px;
    width: 100%;
    border: none;
    text-align: left;
    outline: none;
    font-size: 15px;
    transition: 0.4s;
}

button.accordion.active,
button.accordion:hover {

    background-color: #ddd;
}

button.accordion:after {

/* Unicode character for "plus" sign
(+) is '\02795' */

    content: '\02795';
    font-size: 13px;
    color: #777;
    float: right;
    margin-left: 5px;
}

button.accordion.active:after {

/* Unicode character for "minus" sign
(-) is '\2796' */

    content: "\2796";
}

div.panel {
    padding: 0 18px;
    background-color: white;
    max-height: 0;
    overflow: hidden;
    transition: 0.6s ease-in-out;
    opacity: 0;
}

div.panel.show {
    opacity: 1;
    max-height: 500px;
}

</style>
</head>
<body>

<h2>Treatment&Prescription</h2>

<p>In this example we have added a
"plus" sign to each button. When the
user clicks on the button,the "plus"
sign is replaced with"minus"sign.</p>

<button class="accordion">TB
</button>

<div class="panel">

<p>The TB is the largest flu
species, most recognisable for its
pattern of attacking lungs of patints for a long time
.</p>

</div>

<button class="accordion">Cancer</button>
<div class="panel">

<p>The Cancer is one of the big kilkers
in the region</p>

</div>

<button class="accordion">HighBlood Pressure
</button>
<div class="panel">

<p>if managed well like cancer it too can be cured eventually</p>

</div>

<script>

var acc = document
.getElementsByClassName("accordion");

var i;

for (i = 0; i < acc.length; i++) {
acc[i].onclick = function(){
  this.classList.toggle("active");
  this.nextElementSibling.classList
  .toggle("show");
  }
}

</script>

</body>
</html>
