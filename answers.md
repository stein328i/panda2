
Part 1:

<!-- Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead. -->

image = document.querySelector(".profile-image").src = "http://s3.media.squarespace.com/production/375883/6042936/_EWVgQCn5LlA/SMZ1YxGcLHI/AAAAAAAAFgw/K6rZYi-T3H4/s400/pandas.jpg"

<!-- Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing. -->

image = document.querySelector(".photography").src = "https://placebear.com/325/302";

<!-- Select the heading that says "Panda the Bear" and change it to your own name. -->

title = document.querySelector("h1").innerText = "Stein Tan";

<!-- Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector) -->

experience = document.querySelector("#employment > h3").innerText = "Experience";
<!-- experience = document.querySelector("info-title").innerText = "Experienceeeee"; -->

<!-- Change the colour of the body. -->
body_background_color = document.querySelector('body'); body.style.backgroundColor = 'beige'
body_text_colour = document.body.style.color = "rasberry";

<!-- Change the colour used by the highlight class. -->

font = document.querySelector('h1'); font.style.fontFamily = 'monospace';

<!-- Change the font family of the h1 to 'monospace'. -->

title = document.querySelectorAll("h1"); for (i = 0; i < title.length; i++) {title[i].style.fontFamily = "monospace"};

<!-- Find a way to select the round icons in the sidebar and then change their colour. -->

circles = document.querySelectorAll(".action-icon-bg"); for (i = 0; i < circles.length; i++) {circles[i].style.backgroundColor = "green"};

<!-- Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself". -->

document.getElementById("name").placeholder = "Identify Yourself";

<!-- Change the placeholder attribute of the message field to "state your business". -->

document.getElementById("message").placeholder = "State your business";

<!-- Give the name field a "value" attribute of "your nemesis". -->

document.getElementById("name").value = "Your nemesis";

<!-- Change the value attribute of the email field to "koalathebear@gmail.com". -->

document.getElementById("email").value = "koalathebear@gmail.com";

<!-- Change the value of the submit button on the contact form to "En garde!". -->

document.getElementById("submit").value = "En garde";

<!-- We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute). -->

document.getElementById("submit").disabled = true;

<!-- We should help Panda protect their privacy by clearing their personal details from the sidebar. You can use reset() to do this. -->

document.getElementById("myform").reset();


Part 2:

var div = document.querySelector('section > div'); var bar = document.querySelectorAll('div.bar-default')[2]; div.removeChild(bar);

var div = document.querySelectorAll('section > div')[1]; var pikachu = document.querySelector('img[title="Pikachu"]'); var pikachuTwo = pikachu.cloneNode(true); div.appendChild(pikachuTwo);

for (var i = 0; i < 10; i++) { var pikachuTwo = pikachu.cloneNode(true); div.appendChild(pikachuTwo); }

var listItem = document.createElement('li') var leftSpan = document.createElement('span') var lastUpdated = document.createTextNode('Page last updated on') leftSpan.appendChild(lastUpdated) listItem.appendChild(leftSpan) var rightSpan = document.createElement('span') var currentDate = document.createTextNode(new Date()) rightSpan.appendChild(currentDate) listItem.append(rightSpan) var personalDetails = document.querySelectorAll('ul.bio-info > li')[2] personalDetails.appendChild(listItem)
