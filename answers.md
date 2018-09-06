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
