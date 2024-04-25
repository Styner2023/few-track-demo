# Demo Game

This is a demo app to give an idea of the kinds of code and programming involved with programming web applications.

View the game live [here](https://make-school-labs.github.io/few-track-demo/).

# Instructions

- Download this project by clicking on the green `<> Code` button and selecting `Download ZIP`. Once downloaded, extract the files.
- Open the folder in VSCode. Here's a link to [Download VSCode](https://code.visualstudio.com/) if you don't have it installed yet. This is where you will be editing the code.
- Now open the file `index.html` in your file explorer to open it in the web browser. This is where you will see all the changes once they take effect.

1. Let's start in the `index.html` file using your code editor
   1. Find the `title` tag, and change it from `demo game` to something fun
   2. Find the `h1` tag that holds our `boring game title`, and update it with a new fun and exciting name
   3. Find the `link` to our stylesheet and add in the `href` attribute
   4. Take a look at what's changed on the page (refresh the webpage in your browser)
2. Now over to the `style.css` file
   1. Look through the images folder and find a cool alien you want to play as
   2. In the `:root` rule, change the `--player-image` variable to your favorite alien
   3. Lets also change the `--background-image` to your favorite wall
   4. Now lets change the `--button-color` to something more readable
   5. The buttons look better, but them being square is a little weird, so lets find the `.button` rule
   6. Inside the `.button` rule, let's add a new property `border-radius` and set it to a value of `50%`
   7. Take a look at what's changed on the page (refresh the webpage in your browser)
3. Now the page looks a lot better, lets make it work
   1. Go back to the `index.html` file and find the `script` tag, add in the `src` attribute
   2. Take a look at what's going on, things are moving now!
   3. Find the `timePerBomb` and `timePerFruit` variable and change them until you find a balance you like.
   4. Find the `makeObject` function, and inside find where the objects speeds are set.
   5. Change the speed of the bombs and fruits until you find a balance you like
   6. Take a look at what's changed on the page (refresh the webpage in your browser)
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
