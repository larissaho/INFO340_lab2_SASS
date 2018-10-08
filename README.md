# Are you stuck?

One of the most important lessons that I have learnt in life is how to teach myself. That is because in your academic or career path, you will encounter many professors/instructors whose teaching styles will not match your learning style. Luckily, STEM nowadays is very easy to learn by yourself. So I really encourage you guys to learn things on your own. Here are some steps to follow when you are stuck:
  1. Go to the [documentation](http://sass-lang.com/documentation/file.SASS_REFERENCE.html) or Stack Overflow.
  2. Ask your neighbor. Getting to know your classmate might help you choose teammates for your project.
  3. I have a solution branch. Go look at it and see if it makes sense.
  4. Ask me!
  
If you guys don't agree with the paragraph above, I am more than willing to answer you guys.

# Let's Get SASS-y

Writing CSS kinda sucks. Many times when writing it, you copy paste a lot of code, and there isn't a great way to throw stuff into variables to be reused. An awesome library called [SASS](http://sass-lang.com/) fixes all of it!

## Installing

1. Go to your terminal or command line prompt. Type `npm install -g sass`.
    * If you don't like `npm`, check out the [installation instructions ](http://sass-lang.com/install).
2. Confirm that you have `sass` installed with `sass -v` in your terminal.

## Getting Started
We will install a plugging called *Live Sass Compiler* that will compile your `sass` to `css` on the go.
1. Go to `Extensions` in VSCode or `Shift + Cmd/Ctrl + X` and install *Live Sass Compiler*.
2. You will see that the *install* button just turned into *reload*. Click that and it should automatically restart your program.
3. Here we will begin the sass watcher. See the blue bar at the bottom of your IDE (VSCode)? There should be an option saying `Watch Sass` with an eye symbol next to it. Click that!
4. Once you do that, the `OUTPUT` tab will pop-out underneath your text editor. It means that whatever change you are making to `sass` files will automatically transpile to `css` files!
5. Open the `index.html` and `css/styles.scss` files!
6. Make a change to `h1` to give it the color of `red` to confirm that the styles are compiling. Also, see if there is a `syles.css` file in your `css` folder! BOOOM MAGIC :sparkles:.
  > Once you are done with the lab, you can mess around with *Live Sass Compiler* and tell it where you want your `css` files to be compiled at. You can go to user settings in VSCode and type `liveSassCompile.settings.format`. Click this [link](https://github.com/ritwickdey/vscode-live-sass-compiler/blob/master/docs/settings.md) for more info.

## Part 1: Variables and Math

1. Using a nesting structure, select all the `ul` and `ol` elements within the `.container` class and give them the color `red`.
2. Now, at the top of the file, declare a variable `$red`, and assign it the color `red`.
3. Now, go back to where you styled the `ul` and `ol` elements. Change that `red` to `$red`.
4. Now, change the value of the `$red` variable to `blue`, and see the change take place! :eyes:

Continue making variables & doing nesting selection with these steps:

1. Make the `ul` font family be `sans-serif` and the `ol` font family be `monospace`.
2. Make the background color of paragraphs in the the first container have blue color. In the second container, have those paragraphs be the color orange.
3. Make the width of `container` elements have a width of 100% minus 40 pixels.
> :bulb: Use the `calc` helper! Here is a [link](https://developer.mozilla.org/en-US/docs/Web/CSS/calc) :wink:
4. Set the background color of the containers to be pink.

## Part 2: Getting Sassier

Let's get a little more advanced!

1. Another great advantage of `sass` is that it allows you to import code from other `.scss` files. Make a new `css/colors.scss` file and define new color variables that are not in `styles.scss`. Import `colors.scss` into your `styles.scss` with `@import "color"` statement!
  * Use one of the color variables in `colors.scss` to change the color of `h1` in `styles.scss`.

2. Check out how to use [`mixins`](http://sass-lang.com/guide). Declare one called `side-margin` that takes in a `$margin` variable as a parameter to set both the left and right margins to the value of `$margin`. Since the `container` class lacks 40 pixels from the total width, try calling `side-margin` inside `container` and pass in `auto` to *auto*matically center it in the page. Play with the container width and different values passed into `side-margin`.

# Above and beyond!

Congratulations! At this point, you are done with the lab! You can keep learning about Sass and implement unique features into this exercise. Here are some suggestion if you are interested in learning more about `sass`.

## Syntactic Sugar

Try messing around with the [`& > ~`](https://css-tricks.com/the-sass-ampersand/) Sass operators and see how they work in Sass!

## Control directives (@if, @loop, @each)

Here is a [link](http://thesassway.com/intermediate/if-for-each-while) that will help you learn about control directives for `sass`.

## Survey

I will use the slides and material from today for future quarters. I also hope to see ways to improve so you guys are more excited to learn about materials for this course. You guys matter to me a lot and despite how informal I look, I will take your criticism and opinions very seriously.

Here is an optional and anounymous [survey](https://goo.gl/forms/O92NTvz6IYv2Cfq62).

## Be a nice classmate

Did you finish early? Help the people next to you if they have questions. Tell them a joke to make their day better as it will also make your day better. :satisfied:
