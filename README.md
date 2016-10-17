# Vaystays Engineering Coding Challenges
## Introduction
Hello candidate!  Congratulations on making it to this point of the interview process.  We already have determined that you are a great culture-fit, and would like to better gauge your technical acumen, and your approach to solving problems.

Please review the four coding challenge prompts below and select **one** to complete.  We mainly use React/JS & Ruby/Rails, but feel free to use whatever language(s) or frameworks you're comfortable with\*. We love it when people can walk us through their setup in depth!  Be sure to also read the supporting information at the end of this file for some additional information to keep in mind.

## Prompts
### Prompt 1: Vaystays Search
The first prompt is to use sample Vaystays data to implement a search and filter page that allows a use to link to a product details page.  Do not worry about using the actual Vaystays API, but instead use the trimmed sample data in this repo to create a set of listings that can be sorted an filtered per the acceptance criteria below.

It is up to you to decide the fidelity of this solution, and which languages you use.  However, please be reminded that we are a Rails and React shop, and showcasing your familiarity with one or both of those languages is to your benefit.

For this prompt, please satisfy the following **acceptance criteria**:
* Use the **results.json** file as your backing data.
* We're leaving it up to you to decide what information is shown
* Cards are sorted by tiebreaker_sort, by default
* Implement a sort feature to re-sort cards by
 * user_rating, then tiebreaker_sort
 * sleeps_max, then sleeps_comfortably, then tiebreaker_sort
* Implement a filter that allows users to input a minimum number of beds needed, and remove properties which the sleeps_max disqualifies

### Prompt 2: API Mashup
This second prompt allows you to freely connect to third-party APIs that you are interested in.  Do not worry about using the actual Vaystays API, but instead use the trimmed sample data in this repo to create a set of listings that can be sorted an filtered per the acceptance criteria below.  The point of the prompt is to use the data provided in interesting ways to interact meaningfully with **two** third-party APIs.

It is up to you to decide the fidelity of this solution, and which languages you use.  However, please be reminded that we are a Rails and React shop, and showcasing your familiarity with one or both of those languages is to your benefit.
For this prompt, please satisfy the following **acceptance criteria**:
* Use the **results.json** file as your backing data.
* Use the data to connect to two different APIs
* Document why you chose these APIs, and how you used the data provided

### Prompt 3: Clone Wars
Choose one of your favorite online services (Tumblr, Etsy, Airbnb, etc.) and clone an MVP of it in the stack of your choice.  Data can be stubbed, but functionality should match what that service does.

It is up to you to decide the fidelity of this solution, and which languages you use.  However, please be reminded that we are a Rails and React shop, and showcasing your familiarity with one or both of those languages is to your benefit.

For this prompt, please satisfy the following **acceptance criteria**:
* Choose a service to clone, and briffly document why you chose that
* Create an MVP of that service's core functionality using the stack of your choice.


### Prompt 4: The Game of Life
The third option is not Vaystays-specific, and is instead a classic computer science question.  Please first take a moment to familiarize yourself with [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life), and its rules.

The gist of this prompt is to recreate the Game of Life programatically.  It is up to you to decide the fidelity of this solution, and which languages you use.  However, please be reminded that we are a Rails and React shop, and showcasing your familiarity with one or both of those languages is to your benefit.

For this prompt, please satisfy the following **acceptance criteria**:
* Initialize a 50x50 grid of cells, all considered dead, to begin with.
* Be able to take in the following cells [x,y] to set as live, in order to initialize the game:
 * [0][0]
 * [0][1]
 * [1][0]
 * [1][3]
 * [2][1]
 * [2][2]
* Print out the cells of the grid, either simply as outputted numbers, or (bonus points) rendered to an HTML document.
* Be able to, per the rules from the Game of Life wiki, take one step through the game of life, updating the cells correctly.
* Run through a game.  That is: While there are living cells, take one step, wait for a period (call it 1000ms), then take another step, until no cells are left alive.

## Supporting Information
A few things to keep in mind while solving these problems:

* We are a Rails and React shop.  You do not need to limit yourself to these languages when solving these problems, but showing expertise in these certainly earns you brownie points.
* We work towards a deliverable MVP as often as possible - while showing off beautiful design and interactions is nice, it is not the primary focus of these questions.
* The *only* acceptance criteria for these problems is what is given in the question.  If you have any questions, please email bill@vaystays.com, and if you make any assumptions, please supply a README detailing them.
* This prompt is equally a place to show off what you're good at, and document how you make decisions.  Remember that your answers here aid us in understanding what sort of work you are good at, and interested in doing.
* We are not expecting a perfect and polished project that looks like it took a week to complete, but more so a gauge of your familiarity and logic.  If you're having fun, go nuts, but you are not expected to spend more than a day's worth of effort on any of these projects.
* Most importantly, have fun!
