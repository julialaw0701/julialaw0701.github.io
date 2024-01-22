function search() {
    var input = document.getElementById("searchInput").value;
    // Perform search functionality using the input value
    console.log("Search query: " + input);
}

function openLink() {
    window.open("https://www.credithorum.com.hk", "_blank");
}

 // Change text color of navbar
 var navbar = document.querySelector('.navbar');
 navbar.style.color = 'white';


  document.addEventListener("DOMContentLoaded", function() {
    var myCarousel = document.querySelector("#myMissionCarousel");
    var carousel = new bootstrap.Carousel(myCarousel);
  });
 
// Get the button
let mybutton = document.getElementById("myBtn");

// When the user scrolls down 20px from the top of the document, show the button
window.onscroll = function() {scrollFunction()};

function scrollFunction() {
  if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
    mybutton.style.display = "block";
  } else {
    mybutton.style.display = "none";
  }
}

// When the user clicks on the button, scroll to the top of the document
function topFunction() {
  document.body.scrollTop = 0;
  document.documentElement.scrollTop = 0;
}
  
var navbarBrand = document.querySelector('.navbar-brand2');
navbarBrand.style.fontSize = '16px';
navbarBrand.target = '_blank';

var navbarBrand = document.querySelector('.navbar-brand2');

navbarBrand.addEventListener('click', function() {
  navbarBrand.style.color = 'green'; 
});


var sections = document.querySelectorAll('section');

  sections.forEach(function(section) {
    section.addEventListener('click', function() {
      this.classList.toggle('highlight');
    });

    section.addEventListener('select', function() {
      this.classList.add('highlight');
    });

    section.addEventListener('blur', function() {
      this.classList.remove('highlight');
    });
  });
