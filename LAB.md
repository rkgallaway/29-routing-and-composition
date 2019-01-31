![CF](http://i.imgur.com/7v5ASc8.png) LAB - Component Composition
=================================================================

## Before you begin

**For Each of these tasks, implement a router into the application.**

* Wrap your `<App />` component in `<BrowserRouter />` context at the index level
* Implement a simple navigation bar that links to Home and Code
* `/` should render "Hello World" or anything else you choose
* `/code` should render the output of the assignments below ...


## Practice Component Composition
### Assignment 1 - Warmups
* Fork the [Starter Code Sandbox](https://codesandbox.io/s/2zpknvmk0n)
* Create a new component called "Story"
* Render this component from the App component with markup/content inside of the `<div>`
* Create a new component called "Details"
* Have `<Story>` render `<Details>` with the `<span>` tags nested within it
* Refactor to have the `<Details>` component render the div and then the `<span>` tags using the children property

### Assignment 2  - Modularize and Functionalize
* Fork your completed sandbox
* Refactor your work using new modules/files for each component
* Be prepared to discuss/defend file & directory structures chosen
  * Do this will class based components
  * Repeat the process with functional components in different files
    * `<FunctionalStory />` and `<FunctionalDetails />`
  * Your output should repeat, once with each component set
  
### Assignment 3  - Conditionals
* Create a new component (in its own folder) called `If`
* Code this component to use logic to hide/show it's `props.children`
  * `<If condition> <Then> (render when true) <Else> (render when false)`
  * `<Unless condition...>` (only displays if condition is false)
  * `<When condition ...>` (only displays if condition is true)
* Use this component to conditionally render items from the previous assignments.

### Assignment 4  - Modal
* Fork the [star wars fetcher sandbox](https://codesandbox.io/s/1o64l8pqm4) 
* Create a new component (in its own folder) called `Modal`
* Replace the `<h3>` tag that shows the person with a `<Modal>` with the `<h3>` inside it
* Code out the modal component with the following features:
  * When active, it should render it's `{props.children}`
  * It should draw itself with a close icon/link
  * It should be able to close (i.e. not render)
  
### Assignment 5 - Cards and Decks
Fork This Sandbox: [Cards and Decks Starter Code](https://codesandbox.io/s/km24yvxx8v)

* Using the `content.json` file in the starter code as a guide/source, create a page of cards and decks with the following baseline considerations:
  * `<Page />` should be a collection of Deck Components 
    * (as given in the array in the content.json file)
  * `<Deck />` should be a collection of Card Components 
    * (as provided as an array within each section of the content.json file)
  * `<Card />` should be the representation of a content record in markup
    * (as provided in each detail in the content.json file)
  * From a markup standpoint ...
    * Decks are sections with a class of 'deck'
    * Cards are divs with a class of 'card'
  * From a styling standpoint ...
    * Each component should carry it's own .scss, responsible for basic layout, based on options.
    * Each component should import the design to gain access to variables and mixins
    * Lean on the design for actual styling, animations, etc.


### Testing
* Complete basic render testing on these components
* Complete logical and render testing on the if components

### Deployment
* The `<If>` series of components and the `<Card/><Deck/><Page/>` series are components that should become part of your official library.  Create sandboxes just for those and keep them separate.  
* Later in the course, we will build a re-usable library.

##  Documentation
Complete the README.md file included in the lab folder
