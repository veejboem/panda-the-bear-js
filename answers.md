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

2)
