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
    background-color: #83BAB0;
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

<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {box-sizing:border-box}
body {font-family: Verdana,sans-serif;}
.mySlides {display:none}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
  background-color: #BF8B85;
}

/* Caption text */
.text {
  color: #f2f2f2;
  font-size: 15px;
  padding: 8px 12px;
  position: absolute;
  bottom: 8px;
  width: 100%;
  text-align: center;
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* The dots/bullets/indicators */
.dot {
  height: 13px;
  width: 13px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}


/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

/* Caption text */
.text {
  color: #f2f2f2;
  font-size: 15px;
  padding: 8px 12px;
  position: absolute;
  bottom: 8px;
  width: 100%;
  text-align: center;
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* The dots/bullets/indicators */
.dot {
  height: 13px;
  width: 13px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active {
  background-color: #717171;
}

/* Fading animation */
.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.5s;
  animation-name: fade;
  animation-duration: 1.5s;
}

@-webkit-keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

/* On smaller screens, decrease text size */
@media only screen and (max-width: 300px) {
  .text {font-size: 11px}
}
</style>
</head>


</style>
</head>
<head>
<style>
div.Title {
    background-color: teal;
    color: white;
    margin: 20px 0 20px 0;
    padding: 20px;
}
</style>
</head>

<body>

<div class="Title">
<h2 img align="middle"><font size="18">College Knowledge</font>
</div> 

</body>
<body>


<div class="tab">
  <button class="tablinks" onclick="openDetail(event, 'College Hacks')" id="defaultOpen">College Hacks</button>
  <button class="tablinks" onclick="openDetail(event, 'Study Tips')">Study Tips</button>
  <button class="tablinks" onclick="openDetail(event, 'Scholarships')">Scholarships</button>
   <button class="tablinks" onclick="openDetail(event, 'Studying Abroad')" id="defaultOpen">Studying Abroad</button>
   <button class="tablinks" onclick="openDetail(event, 'Student Discounts')" id="defaultOpen">Student Discounts</button>
   <button class="tablinks" onclick="openDetail(event, 'Road to Success')" id="defaultOpen">Road to Success</button>
   <button class="tablinks" onclick="openDetail(event, 'References')" id="defaultOpen">References</button>
   <button class="tablinks" onclick="openDetail(event, 'The Creators')" id="defaultOpen">The Creators</button>
</div>

<div class="slideshow-container" img align="middle">

<div class="mySlides fade">
  <div class="numbertext">1 / 3</div>
  <img src="http://i67.tinypic.com/w6uwhx.jpg" border="0" alt="Image and video hosting by TinyPic"></a>
  <div class="text"></div>
</div>

<div class="mySlides fade">
  <div class="numbertext">2 / 3</div>
  <img src="http://preview.ibb.co/b33PPv/IMG_2901.jpg" alt="IMG_2901" border="0"></a><br /><a target='_blank' href='http://imgbb.com/'></a><br />
  <div class="text"></div>
</div>

<div class="mySlides fade">
  <div class="numbertext">3 / 3</div>
  <img src="http://preview.ibb.co/caocBa/1728697_Anthony_D_Williams_Quote_Knowledge_comes_from_learning_Wisdom.jpg" alt="1728697_Anthony_D_Williams_Quote_Knowledge_comes_from_learning_Wisdom" border="0"></a><br /><a target='_blank' href='http://imgbb.com/'></a><br />
  <div class="text"></div>
</div>

</div>
<br>

<div style="text-align:center">
  <span class="dot"></span> 
  <span class="dot"></span> 
  <span class="dot"></span> 
</div>

<script>
var slideIndex = 0;
showSlides();

function showSlides() {
    var i;
    var slides = document.getElementsByClassName("mySlides");
    var dots = document.getElementsByClassName("dot");
    for (i = 0; i < slides.length; i++) {
       slides[i].style.display = "none";  
    }
    slideIndex++;
    if (slideIndex> slides.length) {slideIndex = 1}    
    for (i = 0; i < dots.length; i++) {
        dots[i].className = dots[i].className.replace(" active", "");
    }
    slides[slideIndex-1].style.display = "block";  
    dots[slideIndex-1].className += " active";
    setTimeout(showSlides, 5000); 
}
</script>

<div style="background-color:teal;color:white;padding:20px:"id="College Hacks" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <h3> College Hacks</h3>
  <p style="font-family:graduate;">Shortcuts are everywhere to simplify the difficulty of tasks, which is greatly needed for a college student in an environment where everything appears to be intricate.</p>
    <h4> Never Buy a Textbook Again!</h4>
    <p> Here are 10 websites where you can get them for free </p>
  <ul>
  <li style="font-family:graduate;">TextBookNova.com</li>
  <li style="font-family:graduate;">eBookee.org</li>
  <li style="font-family:graduate;">ManyBooks.net</li>
  <li style="font-family:graduate;">FeedUrBrain.com</li>
  <li style="font-family:graduate;">AllenG.ru</li>
  <li style="font-family:graduate;">2020Ok.com</li>
  <li style="font-family:graduate;">FreeTextBooks.com</li>
  <li style="font-family:graduate;">Gutenberg.org</li>
  <li style="font-family:graduate;">Eknigu.com</li>
  <li style="font-family:graduate;">En.Bookfi.org</li>
  </ul>
    <h4> Top 6 Editing Tools for College Students</h4>
  <ul>
  <li style="font-family:graduate;"> Grammarly </li>
  <p style="font-family:graduate;"> Grammarly can spot your usual spelling errors, as well as identify grammar, stylistic, and contextual spelling errors with a detailed explanation to explain your mistake.</p>
  <li style="font-family:graduate;"> ProWritingAid</li>
  <p style="font-family:graduate;"> ProWritingAid will help you improve your writing chops when it comes to clarity, sentence length, phrasing, style, and repetition.
  <li style="font-family:graduate;"> Help.PragTracker </li>
  <p style="font-family:graduate;"> You can have your paper edited by a professional to make sure your paper is 100% plagiarism-free, as well as contact their helpfull staff through their live chat app.</p>
  <li style="font-family:graduate;"> The Hemingway Editor </li>
  <p style="font-family:graduate;"> The Hemingway Editor will help you achieve clarity in your writing by clearing cliches, redundant structures, phrases, adverbs, and more. </p>
  <li style="font-family:graduate;"> Wordcounter </li>
  <p style="font-family:graduate;"> Wordcounter keeps track of how many times you have used every word, and ranks them according to frequency of use so that you don't rely too much on some words. </p>
  <li style="font-family:graduate;"> After the Deadline </li>
  <p style="font-family:graduate;"> After the Deadline is a Grammarly alternative that will also explain why a word is wrong, and provide an appropriate replacement in about 90% of cases </p>
  </ul>
    <h4> Here Are Some Other Life Hacks for College </h4>
  <ul>
  <li style="font-family:graduate;"> Take notes using different colored pens </li>
  <li style="font-family:graduate;"> Prepare meals in advance </li>
  <li style="font-family:graduate;"> Hack your wifi router </li>
  <li style="font-family:graduate;"> gGet a laptop lock </li>
  <li style="font-family:graduate;"> Hang pics with washi tape </li>
  <li style="font-family:graduate;"> Use visa gift cards to get free trials online </li>
  <li style="font-family:graduate;"> Wrap drinks in wet paper towels and put in fridge for 15 min to chill quickly </li>
  <li style="font-family:graduate;"> Tape dryer sheets over the AC/ fan and turn on the appliance to make dorm smell better </li>
  <li style="font-family:graduate;"> When giving a presentation, tell a friend to ask you a question you already know the answer to </li>
  <li style="font-family:graduate;"> Get the wifi passwords on most establishments by checking the comments on foursquare </li>
  <li style="font-family:graduate;"> Use command strips to mount tablets wherever you want </li>
  <li style="font-family:graduate;"> Tape a power strip near your bed </li>
  <li style="font-family:graduate;"> Freshmen, set your schedule as your lock screen so that you're not 'that' lost freshie </li>
  <li style="font-family:graduate;"> Put nailpolish on your keys to know which one is which </li>
  <li style="font-family:graduate;"> Collect change in a change jar all year </li>
  <li style="font-family:graduate;"> Find mug recipes online </li>
  <li style="font-family:graduate;"> Be stealthy and fill up empty containers in cafeteria </li>
  <li style="font-family:graduate;"> 'File' your T-shirts </li>
  <li style="font-family:graduate;"> Download SelfControl app to help with study time </li>
  </ul>
</div>

<div style="background-color:teal;color:white;padding:20px:"id="Study Tips" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <h3> Study Tips</h3>
  <p style="font-family:graduate;">One key to success in college is intertwined with your studying habits, since your grade primarily comes from the assessments you take in class. It is important you find the studying method which is best for you.</p> 
  <h4> Studying for an exam? </h4>
    <p style="font-family:graduate;"> Google "site:edu [subject] exam". You'll get a bunch of college exams from the same course. A great way to quiz yourself before your actual exam.</p> 
   <h4> List of Useful Study Tips </h4>
   <ul> 
  <li style="font-family:graduate;"> Utilize spaces and materials provided by the library </li>
  <li style="font-family:graduate;"> Find study and homework groups </li>
  <li style="font-family:graduate;"> Use flashcards! </li>
  <li style="font-family:graduate;"> Turn something that you need to memorize into a song </li>
  <li style="font-family:graduate;"> Teach the subject to someone else </li>
  <li style="font-family:graduate;"> Make sure you are getting enough sleep </li>
  <li style="font-family:graduate;"> Go to class, obviously, how else will you learn </li>
  <li style="font-family:graduate;"> Go to office hours as well </li>
  <li style="font-family:graduate;"> Planners are highly recommended </li>
  <li style="font-family:graduate;"> Manage your time wisely </li>
  <li style="font-family:graduate;"> Minimize Procrastination </li>
  </ul>
</div>

<div style="background-color:teal;color:white;padding:20px:"id="Scholarships" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <h3> Scholarships</h3>
  <p style="font-family:graduate;">Who doesn't want a free education? Scholarships are a great way to obtain financial assistance for tuition and supplies.</p>
</div>

<div style="background-color:teal;color:white;padding:20px:"id="Studying Abroad" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <h3> Studying Abroad</h3>
  <p style="font-family:graduate;">Culture comes into play when studying outside the borders, which enables a lot 
  of opportunities for a college student, not only fulfilling their education, but their interests and hobbies as well.</p>
  <h4> Remember! </h4>
  <ul>
  <li style="font-family:graduate;"> Go into the experience knowing what you will accomplish and what you will get out of it </li>
  <li style="font-family:graduate;"> Consider multiple factors when choosing your location: academics, language, duration, independence, location, career </li>
  <li style="font-family:graduate;"> Make sure you can afford the trip (financially and academically) </li>
  <li style="font-family:graduate;"> Discuss your plan with advisors. Make sure you are making the right move </li>
  </ul>
</div>

<div style="background-color:teal;color:white;padding:20px:"id="Student Discounts" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <h3> Student Discounts</h3>
  <p style="font-family:graduate;">As you may know, college is the time when lack of money becomes quite persistent, so saving up becomes quite essential. Fortunately, there are places such as stores and cafes which provide students with discounts.</p>
  <h4> Restaurants That Do Student Discounts </h4>
  <ul>
  <li style="font-family:graduate;"> Subway - 10% off </li>
  <li style="font-family:graduate;"> Chipotle - Free Drink </li>
  <li style="font-family:graduate;"> Qdoba - Free Drink - meal for $5 </li>
  <li style="font-family:graduate;"> Burger King - 10% off </li>
  <li style="font-family:graduate;"> Waffle House - 10% off </li>
  <li style="font-family:graduate;"> Chick-Fil-A - Free Drink </li>
  <li style="font-family:graduate;"> Arby's - 10% off </li>
  <li style="font-family:graduate;"> McDonalds - 10% off </li>
  <li style="font-family:graduate;"> Buffalo Wild Wing - 10% off </li> 
  <li style="font-family:graduate;"> Dairy Queen - 10% off </li>
  <li style="font-family:graduate;"> Domino's - 10% off </li>
  <li style="font-family:graduate;"> Pizza Hut - 10-20% off </li>
  <li style="font-family:graduate;"> Papa John's - 10-20% off </li>
  <li style="font-family:graduate;"> IHOP - 10% off </li>
  <li style="font-family:graduate;"> Hard Rock Cafe - discounted menu with ISID </li>
  <li style="font-family:graduate;"> Buca Di Beppo - 10% off </li>
  <li style="font-family:graduate;"> Kroger - 5% off </li>
  <li style="font-family:graduate;"> Firehouse Subs - 10% off </li>
  <li style="font-family:graduate;"> Sweet Tomatoes - 10% off </li>
  </ul>
  <h4>  Supplies Stores That Do Student Discounts</h4>
  <ul>
  <li style="font-family:graduate;"> FedEx Office - 30% off documents - 20% off with their shipping services </li>
  <li style="font-family:graduate;"> Amazon - free two-day shipping for 6 months </li>
  <li style="font-family:graduate;"> Ben Franklin Crafts - Tuesdays, take 10% off </li>
  <li style="font-family:graduate;"> Jo-Ann Fabric Store - 10% off </li>
  <li style="font-family:graduate;"> Hancock Fabrics - 10% off </li>
  <li style="font-family:graduate;"> Discount Dance Supply - 10% off </li>
  </ul>
  <h4> Bookstores That Do Student Discounts</h4>
  <ul>
  <li style="font-family:graduate;"> Guilford Press - 40% off and free shipping </li>
  <li style="font-family:graduate;"> The Economist - up to 69% with International Student ID Card </li>
  <li style="font-family:graduate;"> The New York Times - 99 cents first 4 weeks - 50% off afterwards </li>
  <li style="font-family:graduate;"> The Wall Street Journal - 75% off regular rates delivery </li>
  </ul>
  <h4> Clothing and General Merchandise</h4>
  <ul>
  <li style="font-family:graduate;"> Eddie Bauer - depends on location </li>
  <li style="font-family:graduate;"> Necessary Clothing - 20% off online purchases of $100 </li>
  <li style="font-family:graduate;"> Sam's Club - discount on membership - savings on college essentials </li>
  <li style="font-family:graduate;"> J.Crew - 15% off </li>
  <li style="font-family:graduate;"> Oasis - 20% off </li>
  <li style="font-family:graduate;"> Toms - free shipping - donates pair to child in need for every pair bought </li>
  <li style="font-family:graduate;"> Banana Republic - %15 off </li>
  <li style="font-family:graduate;"> Asos - free shipping </li>
  <li style="font-family:graduate;"> Eastern Mountain Sports - up to 20% off </li>
  <li style="font-family:graduate;"> Ralph Lauren Rugby - 15% off </li>
  <li style="font-family:graduate;"> CollegeBudget - major discounts on clothing, electronics, paintballing </li>
  <li style="font-family:graduate;"> Charlotte Russe - 10% off </li>
  <li style="font-family:graduate;"> Sally Beauty Supply - monthly specials and email offers </li>
  <li style="font-family:graduate;"> Juicy Couture - 15% off </li>
  <li style="font-family:graduate;"> The Limited - 15% off </li>
  <li style="font-family:graduate;"> Club Monaco - 15-20% off </li>
  <li style="font-family:graduate;"> Madewell - 15% off </li>
  <li style="font-family:graduate;"> Medelita - 25% off lab coats, scrubs, clogs and more </li>
  <li style="font-family:graduate;"> Kate Spade - 15% off </li>
  <li style="font-family:graduate;"> Good Will - 10% off (check location) </li>
  <li style="font-family:graduate;"> ModCloth - 15% off </li>
  <li style="font-family:graduate;"> Steve Madden - 10% off in store </li>
  <li style="font-family:graduate;"> Top Shop - 10% off </li>
  </ul>
  <h4> Electronics and Digital Services</h4>
  <ul>
  <li style="font-family:graduate;"> Apple Store - up to $200 off new Mac </li>
  <li style="font-family:graduate;"> Sprint - Sprint Discount Program </li>
  <li style="font-family:graduate;"> Paul C. Buff - 10% off </li>
  <li style="font-family:graduate;"> Adobe - Adobe software for cheap if student edition software is purchased </li>
  <li style="font-family:graduate;"> Norton - up to 50% off protection software for PC, Mac, and more </li>
  <li style="font-family:graduate;"> HP - exclusive education discount savings for custom PCs </li>
  <li style="font-family:graduate;"> JourneyEd - academic software discounts and hardware for students </li>
  <li style="font-family:graduate;"> AT&T - discounts on wireless phones and services by validating email </li>
  <li style="font-family:graduate;"> Das Keyboard - get DK at a discount using their education discount program </li>
  <li style="font-family:graduate;"> Logitech - 30% off on Logitech.com </li>
  <li style="font-family:graduate;"> WordsRU - academic and proofreading online - 10% off editing jobs </li>
  <li style="font-family:graduate;"> Ableton - 40% off </li>
  <li style="font-family:graduate;"> Lenovo - access to offers and discounts on laptops and more </li>
  <li style="font-family:graduate;"> Kinleaves - 20% off gadget skins - free worldwide shipping with ISID </li>
  <li style="font-family:graduate;"> B&H Photo Video - discounted prices on products in imaging and audio </li>
  <li style="font-family:graduate;"> DELL - savings and special packages </li>
  <li style="font-family:graduate;"> Trustive - half off wireless internet access with ISID </li>
  <li style="font-family:graduate;"> Fujitsu - 5% off Lifebook notebook and Tablet PCs </li>
  <li style="font-family:graduate;"> Ai Squared - 50% off single-user copies of ZoomText </li>
  <li style="font-family:graduate;"> Sony - 10% off </li>
  </ul>
  <h4> Services </h4>
  <ul>
  <li style="font-family:graduate;"> State Farm Insurance - up to 25% off </li>
  <li style="font-family:graduate;"> T-Mobile - 10% off monthly rates - exclusive discounts on devices </li>
  <li style="font-family:graduate;"> Zipcar - discounted membership rates </li>
  <li style="font-family:graduate;"> Esurance - discounts </li>
  <li style="font-family:graduate;"> CorePower Yoga - specialty pricing </li>
  <li style="font-family:graduate;"> Jiffy Lube - $10 or 10% off </li>
  <li style="font-family:graduate;"> Nationwide Insurance - Good Student discounts </li>
  <li style="font-family:graduate;"> 24 Hour Fitness - special pricing at the clubs </li>
  <li style="font-family:graduate;"> Travelers Insurance - Travelers Insurance's Good Student Discount </li>
  <li style="font-family:graduate;"> Allstate Insurance - up to 25% off </li>
  <li style="font-family:graduate;"> Moo.com - 20% off order </li>
  <li style="font-family:graduate;"> Geico - up to 15% off </li>
  </ul>
  <h4> Travel, Entertainment, Transportation </h4>
  <ul>
  <li style="font-family:graduate;"> Rail Europe - Youth Pass </li>
  <li style="font-family:graduate;"> Lonely Planet - 30% off LP guides and PDF eBooks using ISID </li>
  <li style="font-family:graduate;"> Madame Tussauds - 15% off admission </li>
  <li style="font-family:graduate;"> AMC Theaters - Thursdays with cheaper admission rate </li>
  <li style="font-family:graduate;"> Greyhound - 20% off on fares and more </li>
  <li style="font-family:graduate;"> TravelSIM - 60% off SIM cards with ISID </li>
  <li style="font-family:graduate;"> STA Travel - special pricing for student travel </li>
  <li style="font-family:graduate;"> HolidayCars.com - 10% off using ISID </li>
  <li style="font-family:graduate;"> StudentUniverse - special deals on travel and experience </li>
  <li style="font-family:graduate;"> Ski Colorado - special college passes for skiing in Colorado </li>
  <li style="font-family:graduate;"> New England Pass - discounted pass to skii in England </li>
  <li style="font-family:graduate;"> The Met - discounted student tickets to select performances </li>
  <li style="font-family:graduate;"> Eurail - 35% off adult price </li>
  <li style="font-family:graduate;"> Penske Truck Rental - 10% off </li>
  <li style="font-family:graduate;"> General Motors - special deals and features </li>
  <li style="font-family:graduate;"> Memphis Symphony Orchestra - $5 student tickets for select concerts </li>
  <li style="font-family:graduate;"> Amtrak - save 15% on fares - up to 50% off on clothes, food, entertainment </li>
  <li style="font-family:graduate;"> Public Transportation - reduced student rider rates </li>
  <li style="font-family:graduate;"> Cinemark - special student rate </li>
  <li style="font-family:graduate;"> Carnegie Hall - tickets $10 </li>
  <li style="font-family:graduate;"> Lincoln Center - discounted tickets for world-class performing arts </li>
  <li style="font-family:graduate;"> New England Aquarium - discounted aquarium admission tickets </li>
  <li style="font-family:graduate;"> Houston Ballet - $10 tickets </li>
  <li style="font-family:graduate;"> Choice Hotels - 15% off </li>
  <li style="font-family:graduate;"> Coach USA - discounts - free V.I.P Student Travel Club </li>
  </ul>
</div>

<div style="background-color:teal;color:white;padding:20px:"id="References" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <h3> References</h3>
  <ul> 
  <li style="font-family:graduate;"> studyreadwrite.com </li>
  <li style="font-family:graduate;"> tun.com </li>
  <li style="font-family:graduate;"> 1000lifehacks.com </li>
  <li style="font-family:graduate;"> bestcollegesonline.com </li> 
  <li style="font-family:graduate;"> hercampus.com </li>
  <li style="font-family:graduate;"> https://www.buzzfeed.com/peggy/important-life-hacks-every-college-student-should-know?utm_term=.ekPJXGgRj#.wkKljgKDq </li>
  <li style="font-family:graduate;"> http://www.huffingtonpost.com/2010/09/08/study-tips-for-college-_n_709096.html?slideshow=true#gallery/10344/9 </li>
  </ul>
</div>

<div style="background-color:teal;color:white;padding:20px:"id="The Creators" class="tabcontent">
   <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
   <h3> The Creators</h3>
   <p style="font-family:graduate;"> Here is a little synopsis of each of the authors of this website.</p>
</div>

<div style="background-color:teal;color:white;padding:20px:"id="Road to Success" class="tabcontent">
  <span onclick="this.parentElement.style.display='none'" class="topright">x</span>
  <h3> Road to Success</h3>
   <p style="font-family:graduate;">To pursue a life of success and prosperity relies heavily on choices that you make as a student. Getting your habits and motivations in check are prime factors in planning out your future and acquiring it later on.</p>
   <h4> College Search Tools </h4>
   <ul>
   <li style="font-family:graduate;"> Niche.com </li>
   <li style="font-family:graduate;"> College Counselors - search on Google for counselors in your region </li>
   <li style="font-family:graduate;"> College Expos </li>
   <li style="font-family:graduate;"> Fiske Guide - buy or check them out online </li>
   </ul>
   <h4> Visit These Links to View Supply Lists </h4> 
   <ul> 
   <li style="font-family:graduate;"> http://www.huffingtonpost.com/marjorie-hansen-shaevitz/the-most-outrageously-tho_b_3412396.html </li>
   <li style="font-family:graduate;"> https://bigfuture.collegeboard.org/get-in/making-a-decision/off-to-college-checklist </li> 
   <li style="font-family:graduate;"> http://jessicaslaughter.co/blog/college-shopping-list/ </li>
   <li style="font-family:graduate;"> https://www.hercampus.com/life/campus-life/what-bring-college-best-college-packing-list-ever </li>
   <li style="font-family:graduate;"> https://www.collegemagazine.com/college-packing-list/ </li>
</div>
<div style="background-color:#82B2B1;color:white;padding:20px;">
  <h2>About Us</h2>
  <p style="font-family:graduate;">Hello! We are 3 young girls from a program named Girls Who Code! Here in GWC we learn the basics of JavaScript, C++, HTML, Python, etc. During our final 2 weeks we come together and start brainstorming ideas for our final project. We got placed in groups depending on what we wanted from the options available. Finally we were put into groups and started to work on our final projects. Which has brought us to the creation of this website! While planning what we were going to do for our website we all emphasized the desire to help high school students or anyone interested towards attending college. </p> 
  <p style="font-family:graduate;">Creators: Jacqueline Marchan, Julia Devine, Vanesa Marar</p>
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
