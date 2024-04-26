# Demo Game

This is a demo app to give an idea of the kinds of code and programming involved with programming web applications.

View the game live [here](https://make-school-labs.github.io/few-track-demo/).

# Instructions

- Download this project by clicking on the green `<> Code` button and selecting `Download ZIP`. Once downloaded, extract the files.
- Open the folder in VSCode. Here's a link to [Download VSCode](https://code.visualstudio.com/) if you don't have it installed yet. This is where you will be editing the code. (You can use Notepad, Textedit, or any plain text editor also but you won't the code hints and other features offered by a code editor.)
- Now open the file `index.html` in your file explorer to open it in the web browser. This is where you will see all the changes once they take effect.

1. Let's start in the `index.html` file using your code editor
    1. Find the `<title>` tag, and change it from `Page title here` to something fun. (NOTE! This set the name of the page or tab in the browser!)
    2. Find the `<h1>` tag that holds our `boring game title`, and update it with a new fun and exciting name. (NOTE! Everything inside the `<body>` tag is displayed in browser!)
    3. Find the `<link>` (its at the top) to our stylesheet and add in the `href` attribute to `href='style.css'` (NOTE! This links to the "stylesheet" file `style.css`)
    4. Take a look at what's changed on the page (refresh the webpage in your browser)
2. Now over to the `style.css` file
    1. Look through the images folder and find a cool alien you want to play as...
    2. In `style.css` find the `:root` rule, change the `--player-image` variable to your favorite alien. (NOTE! Since the images are inside the `images` folder use a value like: `./images/Alien-1-Blinking.gif`)
    3. Lets also change the `--background-image` to your favorite wall. (Same as above, there 4 wall images named `wall-1.png` to `wall-4.png`, try them all!) Be sure to refresh the browser to see these changes! 
    4. Now lets change the `--button-color` to something more readable. (NOTE! colors can be expressed with a name like: "red", "orange", "chocolate", "rebeccapurple", "lime" etc. You can also use a "hex" value in the form of three values 0 to f. For example: "fff", "000", "f0f", "6f3", "420", etc. Look up hex color.)
    5. The buttons look better, but them being square is a little weird, so lets find the `.button` rule (around line 147.) Inside the `.button` rule, add a new property `border-radius` and set it to a value of `50%`. Like this: `border-radius: 50%;` (Don't forget the semicolon!)
    6. Take a look at what's changed on the page (refresh the webpage in your browser)
3. Now the page looks a lot better, lets make it work
    1. Go back to the `index.html` file and find the `script` tag, add in the `src` attribute add: `main.js` (should read: `<script src="main.js">` don't forget the quotes around `main.js`!)
    2. Take a look at what's going on, things are moving now!
    3. Find the `timePerBomb` and `timePerFruit` variable and change them until you find a balance you like. (NOTE! The values here are in milliseconds! In other words: 1000 = 1 sec.) Be sure to refresh the game in the browser when you make changes to see the results!  
    4. Find `function makeObject() { ...`, inside the brackets `{ ... }`,  find where the objects speeds are set. These are `let bombSpeed = 1` and `let fruitSpeed = 3`
    5. Change the speed of the bombs and fruits until you find a balance you like. NOTE! `bombSpeed` is used as a multiplier. For example `bombSpeed = 2` means that bombs will move 2x speed of fruit. 
    6. Take a look at what's changed on the page (refresh the webpage in your browser)
    7. Stretch Challenge! Make these values random. You can do that with: `Math.random()` this generates a random number between 0 and 1. You'll need to multiply by the max value and add your minumum value! Something like: `let bombSpeed = Math.random() * 5 + 1` This will generate a random decimal between 1 and 6. 
4. Looks good!

🎉 Congrats! you've turned the starter project into a functional game with your own game mechanics. You made it possible using HTML, CSS and JS. Feel free to glance over the project files and see if there are things you understand and things you are not sure about just yet.

## Stretch Challenges

Here are a few things you can try to take it a step further:

1. Try to 'hack' the game score by changing the `score` variable in the `main.js` file to give yourself 1,000,000 points.
2. Maybe you're used to using WASD instead of arrow keys to move in games. Try adding some extra cases in the `switch` statement in the `main.js` file to allow for both. (Hint: we need to use the `event.code` property of the `event` object, eg. `KeyA`, `KeyW`, `KeyS`, `KeyD`).
3. Having to refresh the page after every change is a bit annoying. Try installing the `Live Server` extension in VSCode to see changes in real-time. You can do this by clicking on the extensions icon on the far left sidebar, search for `Live Server`, and click `Install`. After installing, look for a `Go Live` button at the very bottom right corner of your VSCode editor on the blue bar. Click the `Go Live` button to open the project in your browser. Now, every time you save a file, the browser will automatically refresh to show the changes.

<!-- ## Todo -

1. Some tasks to explore programming on the web.
  - Include comments with notes on possible values along side code
  - Building Web Applications
    - Need a branch to demo the completed game
    - Master branch should leave out some things that become and activity
      - Links to css files and js files
        - These files might be broken into separate files
  - HTML
    - Add some images of other characters
    - Add CSS styles
    - Add JS file
  - CSS
    - Can be better organized for demo
    - Add opportunities for students to make improvements to the appearance
      - #container overflow hidden
      - #contanier round corner
      - .button round corner changes colors
      - .button:hover change colors
      - add a box shadow to player
    - Change game images used as game elements
      - --player-image
      - --bg-image
      - --bomb-image
      - --fruit-*
  - JS
    - Add link to main.js
    - Change somethings in the JS to see what happens
      - Edit variables
        - change the speed and frequency of elements
          - speed of bombs and fruit
          - frequency of fruit vs bombs -->
