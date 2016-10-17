# Engineering Interview Prompts
Interview prompts for Vaystays engineering candidates.

## Introduction
Hello candidate!  Congratulations on making it to this point of the interview process.  We already have determined that you are a great culture-fit, and would like to better gauge your technical acumen, and your approach to solving problems.

Please review the three coding challenge prompts below and select **one** to complete.  Each of the three prompts have a different area of focus, and while some of the data is Vaystays specific, we more want to see how you tackle problems, and what sort of languages you consider your strongest.

A few things to keep in mind while solving these problems:

* We are a Rails and React shop.  You do not need to limit yourself to these languages when solving these problems, but showing expertise in these certainly earns you brownie points.
* We work towards a deliverable MVP as often as possible - while showing off beautiful design and interactions is nice, it is not the primary focus of these questions.
* The *only* acceptance criterita for these problems is what is given in the question.  If you have any questions, please email bill@vaystays.com, and if you make any assumptions, please supply a README detailing them.
* This prompt is equally a place to show off what you're good at, and document how you make decisions.  Remember that your answers here aid us in understanding what sort of work you are good at, and interested in doing.

## Prompt 1
### Interacting with Vaystays Data
The first prompt is to use sample Vaystays data to implement a search and filter page that allows a use to link to a product details page.  Do not worry about using the actual Vaystays API, but instead use the trimmed sample data in this repo to create a set of listings that can be sorted an filtered per the acceptance criteria below.

It is up to you to decide the fidelity of this solution, and which languages you use.  However, please be reminded that we are a Rails and React shop, and showcasing your familiarity with one or both of those languages is to your benefit.

For this prompt, please satisfy the following **acceptance criteria**:
* Use the **results.json** file as your backing data.
* Display all of the results, at minimum as:
 * A card that links to product details
 * Card shows the property name
 * Card shows the the property image if available
 * Card shows rating if available
* Cards are sorted by tiebreaker_sort, by default
* Implement a sort feature to re-sort cards by
 * user_rating, then tiebreaker_sort
 * sleeps_max, then sleeps_comfortably, then tiebreaker_sort
* Implement a filter that allows users to input a minimum number of beds needed, and remove properties which the sleeps_max disqualifies

## Prompt 2
### Connecting to Third-Party APIs
This second prompt allows you to freely connect to third-party APIs that you are interested in.  Do not worry about using the actual Vaystays API, but instead use the trimmed sample data in this repo to create a set of listings that can be sorted an filtered per the acceptance criteria below.  The point of the prompt is to use the data provided in interesting ways to interact meaningfully with **two** third-party APIs.

It is up to you to decide the fidelity of this solution, and which languages you use.  However, please be reminded that we are a Rails and React shop, and showcasing your familiarity with one or both of those languages is to your benefit.

For this prompt, please satisfy the following **acceptance criteria**:
* Use the **results.json** file as your backing data.
* Use the data to connect to two different APIs
* Document why you chose these APIs, and how you used the data provided

## Prompt 3
### The Game of Life
The third option is not Vaystays-specific, and is instead a classic computer science question.  Please first take a moment to familiarize yourself with [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life).

The gist of this prompt is to recreate the Game of Life programatically.  It is up to you to decide the fidelity of this solution, and which languages you use.  However, please be reminded that we are a Rails and React shop, and showcasing your familiarity with one or both of those languages is to your benefit.

The rules of the Game of Life are as follows:

The universe of the Game of Life is an infinite two-dimensional orthogonal grid of square cells, each of which is in one of two possible states, alive or dead, or "populated" or "unpopulated" (the difference may seem minor, except when viewing it as an early model of human/urban behavior simulation or how one views a blank space on a grid). Every cell interacts with its eight neighbors, which are the cells that are horizontally, vertically, or diagonally adjacent. At each step in time, the following transitions occur:

* Any live cell with fewer than two live neighbors dies, as if caused by under-population.
* Any live cell with two or three live neighbors lives on to the next generation.
* Any live cell with more than three live neighbors dies, as if by over-population.
* Any dead cell with exactly three live neighbors becomes a live cell, as if by reproduction.

The initial pattern constitutes the seed of the system. The first generation is created by applying the above rules simultaneously to every cell in the seed—births and deaths occur simultaneously, and the discrete moment at which this happens is sometimes called a tick (in other words, each generation is a pure function of the preceding one). The rules continue to be applied repeatedly to create further generations.

For this prompt, please satisfy the following **acceptance criteria**:

* Initialize a 50x50 grid of cells, all considered dead, to begin with.
* Be able to take in the following cells to set as live, in order to initialize the game:
 * [0][0]
 * [0][1]
 * [1][0]
 * [1][3]
 * [2][1]
 * [2][2]
* Print out the cells of the grid, either simply as outputted numbers, or (bonus points) rendered to an HTML document.
* Be able to, per the rules above, take one step through the game of life, updating the cells correctly.
* Run through a game.  That is: While there are living cells, take one step, wait for a period (call it 1000ms), then take another step, until no cells are left alive.
