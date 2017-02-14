<!--
  CODE EXAMPLES FROM LECTURE

  $(document).ready(function() {

  $('').html('');
  $('').text(''); //returns text
  $('').css('font', 'red'); //changes value
  $('body').text('li')[2]; // pulls that item
  $('.button').click();
  $('li').last().remove(); //(removes from window)
  $('ul').append('<li>Item 5</li>'); //(adds to window)

var six = $('<li>item 6</li>');
  six // -> [li]
  six.appendTo(six).('Item whatever')


for (var = i=0; i < 100; i++) { $('ul').append('<li>Item ' + (7+i) + '</li>') }
adds a new list item from 7-100

---------------------------------------------------------------- -->

<!-- Hacking Panda the Bear's Resume

1) Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead (hint: use attr()). -->

$('.profile-image').attr('src','https://placekitten.com/g/400/400');

$('#left-image img').attr('src','https://placekitten.com/g/325/225');

<!-- 2) Select the heading that says "Panda the Bear" and change it to your own name. (hint: use text()) -->

$('h1').text('Valerie the Human');

<!-- 3) Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector) -->

$('#employment .info-title').html('Major Key');

<!-- 4) Panda the Bear is lying about their skills! Take the "time travel" skill off the page to satisfy your personal sense of justice. Use your googling and docs-skimming skillz to find a jQuery function that will allow you to remove elements from the DOM. (hint: there are multiple ways of doing this, but the parent() function might be useful when it comes to selecting the right element -->

  $('div#time-travel.bar-filled.highlight').last().remove();

  <!-- OR -->

  $('div.bar-default:nth-last-child(2)').last().remove();

<!-- 5) Change the colour of the body. (hint: use css()) -->

  $('body').css('color', 'red');

  <!-- 6) Change the colour used by the highlight class. -->

  $('.highlight').css('color','red');

  <!-- 7) Change the font family of the h1 to 'monospace'. -->

$('h1').css('font-family','monospace');

<!-- 8) Find a way to select the round icons in the sidebar and then change their colour. -->

$('a.action-icon-bg').css('background-color','red');

<!-- 9) Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself". -->

$('input#name.contact-info').attr('placeholder','identify yourself');

<!-- 10) Change the placeholder attribute of the message field to "state your business". -->

$('textarea#message').attr('placeholder', 'state your business');

<!-- 11) Give the name field a "value" attribute of "your nemesis". ********-->

$('input#name').val('your nemesis');

<!-- 12) Change the value attribute of the email field to "koalathebear@gmail.com".******** -->

$('input#email').attr('placeholder', 'koalathebear@gmail.com');
$('input#email').val('koalathebear@gmail.com');

<!-- 13) Change the value of the submit button on the contact form to "En garde!". -->

$('input#submit').attr('value', 'En garde!');

<!-- Bonus 1) We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute). -->

$('input#submit').appendTo('<input type= disabled>');

<!-- Bonus 2) We should help Panda protect their privacy by clearing their personal details from the sidebar. You can use empty() to do this. -->

$('.bio-info-value').empty('span:last-child');
