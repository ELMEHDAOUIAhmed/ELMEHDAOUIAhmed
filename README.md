# Hi there, I'm ELMEHDAOUI Ahmed zine el abdine - aka [AhmedZin]👋 
---
<!-- [![YouTube Channel Subscribers](https://img.shields.io/youtube/channel/subscribers/UCDCHcqyeQgJ-jVSd6VJkbCw?logo=youtube&logoColor=red&style=for-the-badge)][youtube]
[![Website](https://img.shields.io/website?label=codeSTACKr.com&style=for-the-badge&url=https%3A%2F%2Fcodestackr.com)](https://codestackr.com)
[![Twitter Follow](https://img.shields.io/twitter/follow/codeSTACKr?color=1DA1F2&logo=twitter&style=for-the-badge)](https://twitter.com/intent/follow?original_referer=https%3A%2F%2Fgithub.com%2FcodeSTACKr&screen_name=codeSTACKr) 

[![Visual Studio Marketplace Rating (Stars)](https://img.shields.io/visual-studio-marketplace/stars/codestackr.codestackr-theme?label=codeSTACKr%20VS%20Code%20Theme&logo=visualstudiocode&logoColor=ff652f&style=for-the-badge)](https://marketplace.visualstudio.com/items?itemName=codestackr.codestackr-theme)
[![Become A VS Code SuperHero](https://img.shields.io/badge/-Become%20A%20VS%20Code%20SuperHero%20%E2%86%92-gray.svg?colorB=ff652f&style=for-the-badge)](https://vsCodeHero.com) -->



# I'm a Computer scientist ,Junior Web Developer, a Future Software Engineer !!
---

<!-- - 🔭 Check out my VS Code course: [Become A VS Code SuperHero!][course]!
- 🌱 I’m currently learning everything 🤣
- 👯 I’m looking to collaborate with other content creators
- 🥅 2022 Goals: Learn more about web3
- ⚡ Fun fact: I love to draw and play guitar / drums
- 😻 Check out the NFT collection I created: [CodeCats](https://opensea.io/collection/codecats?search[sortAscending]=true&search[sortBy]=PRICE&search[toggles][0]=BUY_NOW) -->

<!-- ### Connect with me:

[![website](./img/globe-light.svg)](https://codestackr.com#gh-light-mode-only)
[![website](./img/globe-dark.svg)](https://codestackr.com#gh-dark-mode-only)
&nbsp;&nbsp;
[![website](./img/youtube-light.svg)](https://youtube.com/codestackr#gh-light-mode-only)
[![website](./img/youtube-dark.svg)](https://youtube.com/codestackr#gh-dark-mode-only)
&nbsp;&nbsp;
[![website](./img/twitter-light.svg)](https://twitter.com/codestackr#gh-light-mode-only)
[![website](./img/twitter-dark.svg)](https://twitter.com/codestackr#gh-dark-mode-only)
&nbsp;&nbsp;
[![website](./img/linkedin-light.svg)](https://linkedin.com/in/codeSTACKr#gh-light-mode-only)
[![website](./img/linkedin-dark.svg)](https://linkedin.com/in/codeSTACKr#gh-dark-mode-only)
&nbsp;&nbsp;
[![website](./img/instagram-light.svg)](https://instagram.com/codeSTACKr#gh-light-mode-only)
[![website](./img/instagram-dark.svg)](https://instagram.com/codeSTACKr#gh-dark-mode-only) -->



          
### 🧰 Languages and Tools:

<img align="left" alt="Visual Studio Code" width="36px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" style="padding-right:10px;" />
<img align="left" alt="HTML5" width="36px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" style="padding-right:10px;"/>
<img align="left" alt="CSS3" width="36px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" style="padding-right:10px;" />
<img align="left" alt="JavaScript" width="36px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" style="padding-right:10px;" />

<img align="left" alt="PHP" width="36px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/php/php-plain.svg" />

<img align="left" alt="Flutter" width="36px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flutter/flutter-original.svg" />

<img align="left" alt="MongoDB" width="36px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original.svg" style="padding-right:10px;" />
<img align="left" alt="MySQL" width="36px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" style="padding-right:10px;" />
<img align="left" alt="Oracle" width="36px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/oracle/oracle-original.svg"/>

<img align="left" alt="Firebase" width="36px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/firebase/firebase-plain.svg" />


### Guess the Number:

## How to Play

1. The computer will randomly select a number between 1 and 100.
2. You have to guess the number.
3. If your guess is too high, the computer will tell you to guess lower.
4. If your guess is too low, the computer will tell you to guess higher.
5. Keep guessing until you guess the correct number.





<!DOCTYPE html>
<html>
<head>
<title>Guess the Number</title>
<meta charset="utf-8">
</head>
<body>
    <h1>Guess the Number</h1>
    <p>The computer will randomly select a number between 1 and 100. You have to guess the number. If your guess is too high, the computer will tell you to guess lower. If your guess is too low, the computer will tell you to guess higher. Keep guessing until you guess the correct number.</p>
    <p id="result"></p>
    <input type="number" id="guess" placeholder="Enter your guess...">
    <button onclick="checkGuess()">Guess</button>
    <button onclick="reset()">Reset</button>

<script>
      // Generate random number
      var randomNumber = Math.floor(Math.random() * 100) + 1;
      console.log(randomNumber);

      // Initialize number of guesses
      var numGuesses = 0;

      function checkGuess() {
        var guess = parseInt(document.getElementById('guess').value);
        var result = document.getElementById('result');

        if (guess < 1 || guess > 100) {
          result.innerHTML = "Please enter a number between 1 and 100.";
        } else if (guess === randomNumber) {
          numGuesses++;
          result.innerHTML = "Congratulations! You guessed the number in " + numGuesses + " tries.";
        } else if (guess > randomNumber) {
          numGuesses++;
          result.innerHTML = "Too high! Guess lower.";
        } else if (guess < randomNumber) {
          numGuesses++;
          result.innerHTML = "Too low! Guess higher.";
        }
      }

      function reset() {
        randomNumber = Math.floor(Math.random() * 100) + 1;
        console.log(randomNumber);
        numGuesses = 0;
        document.getElementById('result').innerHTML = "";
        document.getElementById('guess').value = "";
      }
</script>
</body>
</html>


<!-- 
<details>
  <summary>:zap: GitHub Stats</summary>

  <img align="left" alt="codeSTACKr's GitHub Stats" src="https://github-readme-stats.vercel.app/api?username=codeSTACKr&show_icons=true&hide_border=false&title_color=ff652f&icon_color=FFE360&bg_color=09131B&text_color=ffffff&border_color=0c1a25" />

</details> -->

<!-- [website]: https://codeSTACKr.com
[course]: http://vsCodeHero.com
[twitter]: https://twitter.com/codeSTACKr
[youtube]: https://youtube.com/codeSTACKr
[instagram]: https://instagram.com/codeSTACKr
[linkedin]: https://linkedin.com/in/codeSTACKr
[webdevplaylist]: https://www.youtube.com/playlist?list=PLkwxH9e_vrAJ0WbEsFA9W3I1W-g_BTsbt
[jsplaylist]: https://www.youtube.com/playlist?list=PLkwxH9e_vrALRJKu7wfXby3MKeflhTu6B
[cssplaylist]: https://www.youtube.com/playlist?list=PLkwxH9e_vrALSdvZuEh6gqQdmDoDIoqz4
[reactplaylist]: https://www.youtube.com/playlist?list=PLkwxH9e_vrAK4TdffpxKY3QGyHCpxFcQ0 -->