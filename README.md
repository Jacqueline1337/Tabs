<!DOCTYPE html>
<html>
<head>
<style>
body {font-family: "Lato", sans-serif;}

/* Style the tab */
div.tab {
    overflow: hidden;
    border: 1px solid #ccc;
    background-color: #f1f1f1;
}

/* Style the buttons inside the tab */
div.tab button {
    background-color: inherit;
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
    background-color: #ddd;
}

/* Create an active/current tablink class */
div.tab button.active {
    background-color: #ccc;
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

.topright:hover {color: red;}
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

<div id="Student Discounts" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <p>Student Discounts info.</p>
</div>

<div id="Road to Success" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <p>Road to success info.</p>
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
     
</body>
</html> 
