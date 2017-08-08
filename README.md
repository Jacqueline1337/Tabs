<!DOCTYPE html>
<html>
<head>
<style>
body {font-family: "Lato", graduate;}


/* Style the tab */
div.tab {
    overflow: hidden;
    border: 1px solid #ccc;
    background-color: #f1f1f1;
}

/* Style the buttons inside the tab */
div.tab button {
    background-color: #f1faee;
    float: left;
    border: none;
    outline: none;
    cursor: pointer;
    padding: 14px 16px;
    transition: 0.3s;
    font-size: 17px;
}

/* Change background color of buttons on hover */
div.tab button:hover {
    background-color: #a8dadc;
   
}

/* Create an active/current tablink class */
div.tab button.active {
    background-color: #378E7D;
}

/* Style the tab content */
.tabcontent {
    display: none;
    padding: 6px 12px;
    border: 1px solid #ccc;
    border-top: none;
}

/* Style the close button */
.topright {
    float: right;
    cursor: pointer;
    font-size: 20px;
}

.topright:hover {color: black;}
</style>
</head>
<body>



<div class="tab">
  <button class="tablinks" onclick="openDetail(event, 'College Hacks')" id="defaultOpen">College Hacks</button>
  <button class="tablinks" onclick="openDetail(event, 'Study Tips')">Study Tips</button>
  <button class="tablinks" onclick="openDetail(event, 'Scholarships')">Scholarships</button>
   <button class="tablinks" onclick="openDetail(event, 'Studying Abroad')" id="defaultOpen">Studying Abroad</button>
   <button class="tablinks" onclick="openDetail(event, 'Student Discounts')" id="defaultOpen">Student Discounts</button>
   <button class="tablinks" onclick="openDetail(event, 'Road to Success')" id="defaultOpen">Road to Success</button>
</div>

<div id="College Hacks" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <p>College Hacks info.</p>
</div>

<div id="Study Tips" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <p>Study Tips info.</p> 
</div>

<div id="Scholarships" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <p>Scholarships info.</p>
</div>

<div id="Studying Abroad" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <p>Studying abroad info.</p>
</div>

<div style="background-color:teal;color:white;padding:20px:"id="Student Discounts" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <h3> Student Discounts</h3>
  <p style="font-family:graduate;">As you may know, college is the time when lack of money becomes quite persistent, so saving up becomes quite 
  essential. Fortunately, there are places such as stores and cafes which provide students with discounts.</p>
</div>


<div id="Road to Success" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <p>Road to success info.</p>
</div>
<div style="background-color:lightBlue;color:white;padding:20px;">
  <h2>About Us</h2>
  <p style="font-family:graduate;">Hello! We are 3 young girls from a program named Girls Who Code! Here in GWC we learn the basics of JavaScript, C++, HTML, Python, etc. During our final 2 weeks we come together and start brainstorming ideas for our final project. We got placed in groups depending on what we wanted from the options available. Finally we were put into groups and started to work on our final projects. Which has brought us to the creation of this website! While planning what we were going to do for our website we all emphasized the desire to help high school students or anyone interested towards attending college. </p> <p>Creators: Jacqueline Marchan, Julia Devine, Vanesa Marar</p>
</div> 

<script>
function openDetail(evt, detailName) {
    var i, tabcontent, tablinks;
    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
        tabcontent[i].style.display = "none";
    }
    tablinks = document.getElementsByClassName("tablinks");
    for (i = 0; i < tablinks.length; i++) {
        tablinks[i].className = tablinks[i].className.replace(" active", "");
    }
    document.getElementById(detailName).style.display = "block";
    evt.currentTarget.className += " active";
}

// Get the element with id="defaultOpen" and click on it
document.getElementById("defaultOpen").click();
</script>
<div id="google_translate_element"></div>

<script type="text/javascript">
function googleTranslateElementInit() {
  new google.translate.TranslateElement({pageLanguage: 'en'}, 'google_translate_element');
}
</script>

<script type="text/javascript" src="//translate.google.com/translate_a/element.js?cb=googleTranslateElementInit"></script>
</body>
</html> 


