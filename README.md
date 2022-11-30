$slider-name: typing-slider;
$slides: 3;
$typing-duration: 5s;
$tab-letters: 16 23 12; //number of characters in each paragraph
$slider-font-size: 3rem;
$background: #FFCC00;

body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: $background;
}

@keyframes cursor {
  from, to { border-color: transparent; }
  50% { border-color: black; }
}

@keyframes typing {
  from { width: 100%; }
  90%, to { width: 0; }
}

@keyframes slide {
  #{100% / $slides} { font-size: $slider-font-size; letter-spacing: 3px; }
  to { font-size: 0; letter-spacing: 0; }
}

.#{$slider-name} {
  font-family: Consolas, monospace;
  font-weight: bold;
  text-align: center;
  white-space: nowrap;
}

.#{$slider-name} p {
  position: relative;
  display: inline;
  font-size: 0;
  text-transform: uppercase;
  letter-spacing: 0;
  animation: slide $typing-duration * $slides step-start infinite;
}

.#{$slider-name} p::after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  border-left: 3px solid black;
  background-color: $background;
  animation: typing $typing-duration infinite,
             cursor 1s infinite;
}

@each $letters in $tab-letters {
  $i: index($tab-letters, $letters);
  .#{$slider-name} p:nth-child(#{$i}) {
    animation-delay:  $typing-duration * ($i - 1);
    &::after {
      animation-delay: $typing-duration * ($i - 1);
      animation-timing-function: steps(#{$letters}), step-end;
    }
  }
}
<div class="typing-slider">
  <p>Text slider with</p>
  <p>typing animation effect</p>
  <p>in pure CSS.</p>
</div>

<h1 align="center">Hi 👋, I'm Aniket Parmar</h1>
<h3 align="center">A passionate full stack web developer from India</h3>

<p align="center"> <img src="https://komarev.com/ghpvc/?username=aniketparmar29&label=Profile%20views&color=0e75b6&style=flat" alt="aniketparmar29" /> </p>


- 👨‍💻 All of my projects are available at <a href="https://aniketparmar29.github.io/" target="_blank">Portfolio</a>

- 💬 Ask me about **react,javascript**

- 📫 How to reach me <a href="https://www.linkedin.com/in/aniket-parmar-a42597239/" target="_blank">Linkedin</a>

- 📄 Know about my experiences <a href="https://drive.google.com/file/d/1LbPArwTFWUcw_OZZNMw0JCojAp1GcFa7/view?usp=sharing](https://drive.google.com/file/d/1LbPArwTFWUcw_OZZNMw0JCojAp1GcFa7/view?usp=sharing" target="_blank">Résumé</a>

- ⚡ Fun fact **I love Cricket**

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://twitter.com/aniket9904026" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="aniket9904026" height="30" width="40" /></a>
<a href="https://linkedin.com/in/aniket-parmar-a42597239" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="aniket-parmar-a42597239" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://getbootstrap.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://www.mongodb.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="mongodb" width="40" height="40"/> </a> <a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/> </a> <a href="https://redux.js.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/redux/redux-original.svg" alt="redux" width="40" height="40"/> </a> <a href="https://www.typescriptlang.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="typescript" width="40" height="40"/> </a> </p>
<p align="center"> <a href="https://github.com/ryo-ma/github-profile-trophy"><img src="https://github-profile-trophy.vercel.app/?username=aniketparmar29" alt="aniketparmar29" /></a> </p>

<p align="center"><img align="center" src="https://github-readme-stats.vercel.app/api/top-langs?username=aniketparmar29&show_icons=true&locale=en&layout=hybrid" alt="aniketparmar29" /></p>

<p align="center">&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=aniketparmar29&show_icons=true&locale=en" alt="aniketparmar29" /></p>

<p align="center"><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=aniketparmar29&" alt="aniketparmar29" /></p>
