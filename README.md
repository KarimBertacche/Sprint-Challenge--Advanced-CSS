# Sprint Challenge: Advanced CSS - Space Walkers Web Page

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a concrete project. This Sprint explored advanced CSS techniques using Responsive Design and Preprocessing. During this Sprint, you studied how to use the viewport meta tag, media queries, setting up a preprocessor, and advanced use of preprocessing techniques. In your challenge this week, you will demonstrate proficiency by updating a website that is missing content as well as adding mobile styling.

## Instructions

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your PM and Instructor in your cohort help channel on Slack. Your work reflects your proficiency in advanced css and your command of the concepts and techniques in responsive web design and preprocessing.

You have three hours to complete this challenge. Plan your time accordingly.

## Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and your project manager.

## Description

The client for this challenge is _Spacewalkers Magazine_. Spacewalkers needs your help to build a small proof of concept website for their marketing team. They have provided designs for both desktop and phone views. In addition to designs and content they have most of the home page coded for you. You just need to finish the navigation and header as well as the mobile styles.

In meeting the minimum viable product (MVP) specifications listed below, your web page should look like the solution design files of the desktop and mobile views:

[Click here to review the home design](design-files/home-desktop.png)

[Click here to review the mobile design](design-files/home-mobile.png)

## Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your project manager

1. What is the difference between an adaptive website and a fully responsive website?
Adaptive layout uses media queries just like responsive but differs from it because it still uses hard coded pixel for layout purposes which make the design adapt to only the screen sizes and viewport of set media queries, all the others are not accounted for, this makes it quicker to deploy but less responsive overall.
However when using responsive design we get the best of all three worlds(Fixed, Fluid, and Adaptive) this is the most used and popular, it provides precise viewing experience for all screen sizes using responsive units and a fluid experience across many devices, also it has shorter loading time and multiple layout, making it easier to maintain and generally a better experience for the user. 

2. Describe what it means to be mobile first vs desktop first.
Mobile versus desktop first are considered the two main ways to approach design content, mobile first basically means that we start building starting from a mobile viewport and adjusting to larger screen sizes/viewports, going up to tablet and then desktop, and other larger screens, going from the smallest to the largest size, which is basically adding features and rearranging them instead of removing or hidding some of the featuers that would otherwise not feat into the smaller screen size. 
The other approach is starting from a desktop design and then scale back the opposite way to smaller screen sizes, generally the mobile first approach is considered the better approach, but really depends on the developer designing it.

3. What does `font-size: 62.5%` in the `html` tag do for us when using `rem` units?
When setting the root font-size to 62.5% we are basically changing the default value of 16px to a size of 10px which is easier to convert into rem, knowing that 1rem equal to 10px as it is a unit relative to the root element compared to the em unit which is relative to the first parent in which a font size is declared and which with nesting can easily go out of control and harder to calculate, using rem makes it also very easy to change all font sizes by just modifying the percentage of the root element instead of having to go all over the page changing every single font value, and also take into account visually impared people which tend to change their default percentage of fonts on their browsers making the screen content more readable(increase readability), when other fonts like fixed px do not.

4. How would you describe preprocessing to someone new to CSS?
Preprocessor are awesome, they facilitate the development and maintanance process and make life so much easier for a developer, writing css becomes quicker as we tend not to repeat ourselves(dry principle) when using preprocessor compared to vanilla css, also they implement features that are still lacking in css like variables that can be used repeatedly all over the file and modified from a single place on later date, with those changes getting immediately reflected all over the file, also we can use mixins to store chunks of key value pairs (properties & value) into a single spot and reuse them wherever we wish to implement them, this mixins can also take parameters and default values(parametric mixins) which makes them adaptive just like function constructors in javascript.
We can also use nesting when creating declarative blocks and make repeating selectors a thing of the past, this is a very useful feature when organising code, and it is possible because they are automatically converted behind the scene by an interpreter into more specific selectors that then gets stored into a css file that is used to render the webpage, this goes for both selectors and media queries, least but not last we can also use preset functions just like in javascript to for example increase or decrease color shades like with the darken() and lighten() methods. 

5. What is your favorite concept in preprocessing? What is the concept that gives you the most trouble?
My favourite concept in preprocessing is the ability to use mixins that makes the coding process much simplier and quicker, this at the same time is a concept that has endless possibilities and that is exciting and terrifying at the same time.

You are expected to be able to answer all these questions. Your responses contribute to your Sprint Challenge grade. Skipping this section *will* prevent you from passing this challenge.

## Project Set Up

Follow these steps to set up your project:

### Git Set up

- [ ] Create a forked copy of this project.
- [ ] Add your project manager as collaborator on Github.
- [ ] Clone your OWN version of the repository (Not Lambda's by mistake!).
- [ ] Create a new branch: git checkout -b `<firstName-lastName>`.
- [ ] Implement the project on your newly created `<firstName-lastName>` branch, committing changes regularly.
- [ ] Push commits: git push origin `<firstName-lastName>`.
 
Follow these steps for completing your project.

- [ ] Submit a Pull-Request to merge <firstName-lastName> Branch into master (student's  Repo). **Please don't merge your own pull request**
- [ ] Add your project manager as a reviewer on the pull-request
- [ ] Your project manager will count the project as complete by merging the branch back into master.
 

### Preprocessor Set up

* [ ] Verify that you have LESS installed correctly by running `lessc -v` in your terminal, if you don't get a version message back, reach out to your project manager for help.
* [ ] Open your terminal and navigate to your preprocessing project by using the `cd` command
* [ ] Once in your project's root folder, run the following command `less-watch-compiler less css index.less`
* [ ] Verify your compiler is working correctly by changing the `background-color` on the `html` selector to `red` in your `index.less` file.
* [ ] Once you see the red screen, you can delete that style and you're ready to start on the next task

## Minimum Viable Product

Your finished project must include all of the following requirements:

### Import LESS Files

* [ ] Navigate to your `index.less` file. Notice the file is blank. You have been asked to use a certain import order. That order is as follows:

```markdown
1.variables.less
2.mixins.less
3.reset.less
4.global.less
5.navigation.less
6.footer.less
7.home-page.less
```

_You will know everything is working properly when you see the styles enabled for the provided content._  

### Home Page - Desktop HTML & LESS

* [ ] Take 10 minutes to review the code that has already been provided for you. Take time to see how the home page was built.

* [ ] Add a viewport meta tag to the head of your index.html page

* [ ] [Review the provided home desktop design file](design-files/home-desktop.png). You are to build the missing navigation system and header image. You have been provided all content necessary in the [index.html file](index.html)

* [ ] Navigation Styles: Use the `navigation.less` file for styling.

* [ ] Main Content Styles: Use the `home-page.less` file for styling

* [ ] LESS Mixins: Create and use 2 different mixins to aid your styling. Use the `mixins.less` file for your mixins

* [ ] LESS Parametric Mixin: create a parametric mixin that is used to create the `sign up` button styles.

* [ ]  Use at least 2 parameters to create your button

* [ ] Create a hover state that swaps the background color and font color of the base button styles.

### Mobile Design

* [ ] Create a `@phone` variable that contains a `max-width: 500px` media query string. Use the `@phone` variable for all your nested mobile styling.

* [ ] [Review the provided home mobile design file](design-files/home-mobile.png). Match your mobile styling the best you can using the design file.

* [ ] Push your changes and create a pull request if you haven't already.

In your solution, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Stretch Problems

After finishing your required elements, you can push your work further. These goals may or may not be things you have learned in this module but they build on the material you just studied. Time allowing, stretch your limits and see if you can deliver on the following optional goals:

* [ ] Build a page of your choosing from the navigation items. Come up with content and images that fit the theme.

* [ ] Introduce CSS animations to your site.

* [ ] Create a fixed navigation and add some opacity to the background

* [ ] Create a form that would allow someone to sign up for a Spacewalkers Magazine subscription