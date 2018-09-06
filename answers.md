1.
var profImage = document.querySelector( "img.profile-image" );
profImage.src = 'https://placebear.com/g/400/400';

2.
var bioName = document.querySelector( "span.bio-info-name" );
bioName.textContent = 'David Ma';

3.
var employment = document.querySelector( '#employment h3.info-title' );
employment.textContent = 'Previous Work';

4.
var body = document.querySelector( 'body' )
body.style.color = 'red';

5.
var highlights = document.querySelectorAll ( '.highlight' );
for (var i = 0; i < highlights.length; i++) {
  highlights[i].style.color = 'cyan';
}

6.
var header = document.querySelector( 'h1' );
header.style.fontFamily = 'monospace';

7.
var roundIcons = document.querySelectorAll( 'a.action-icon-bg' );
for (var i = 0; i < roundIcons.length; i++) {
  roundIcons[i].style.backgroundColor = 'blue';
}

8.
var placeholderName = document.querySelector( '#name' );
placeholderName.placeholder = 'David Ma';

9.
var message = document.querySelector( '#message' );
message.placeholder = 'State your business.';

10.
var placeholderName = document.querySelector( '#name' );
placeholderName.setAttribute('value', 'your nemesis');

11.
document.querySelector( '#email' ).setAttribute('value', 'koalathebear@gmail.com')

12.
document.querySelector( '#submit' ).setAttribute('value', 'En garde!');

13.
document.querySelector( '#submit' ).setAttribute('disabled', true);

14.
var info = document.querySelectorAll( '.bio-info-value' );
for (var i = 0; i < info.length; i++) {
  info[i].textContent = '';
}

Part 2
1. Removing elements from the DOM
var timeTravel = document.querySelector( '.bar-default:nth-of-type(4)' );
timeTravel.parentNode.removeChild(timeTravel);

1. Adding Elements to the DOM
var pikachu = document.querySelector( '#right-image img' );
var clonePika = pikachu.cloneNode();

2. Looping ten times
var portContainer = document.querySelector( '.portfolio-container' );
portContainer.appendChild(clonePika);
for (var i = 0; i < 10; i++) {
  portContainer.insertAdjacentHTML('beforeend', clonePika,outerHTML);
}


3.
var bio = document.querySelector( '.bio-info' );
bio.appendChild(listItem);
var currentDate = new Date();
var rightSpan = document.createElement('span')
var dateText = document.createTextNode(currentDate);
rightSpan.appendChild(dateText);
listItem.appendChild(rightSpan);
rightSpan.setAttribute('class', 'bio-info-value .bio-info-date');
leftSpan.setAttribute('class', 'bio-info-title');
listItem.setAttribute('class', 'bio-info-item')
