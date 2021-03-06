# **Project - Team Collaboration App**

## Overview

Use react-router, CSS modules and the advanced concepts of React that you have learnt in the Sprint 5 to create a Team Collaboration App.

<br />

## Learning pre-requisites

Before you begin this session, kindly ensure that you have completed learning the following topics and solved the corresponding quizzes:

- Accessibility in React.

- Context APIs.

- Refs and the DOM.

- Fragments and HOC.

- Error Boundaries.

- React Hooks.

- Setting styles dynamically in React.

- CSS Modules.

- Switching using React Router.

- History, location and match using react-router.

- The withRouter package.

- Redirections and conditional redirects.

<br />

Additionally, to complete the project successfully,

- External pre-requisite 1:
  
  You need to have a clear understanding of what a team collaboration application is and how does it work. You can check out [Trello](https://trello.com/home) which is the de-facto task organizer/team collaboration tool in most of the top companies in the world. Here is a [guided video](https://trello.com/home) on how a Trello application works. We will not be creating an exact replica of the Trello application but we will be developing a majority of the features of Trello.

- External pre-requisite 2:

  In this project, you will be using CSS modules to style the elements. Although the latest version of CSS Modules no longer asks the users to eject their CRA's default configuration, it is highly recommended that you do eject your configurations to have a better control on your code as well as getting a hands-on experience.

- External pre-requisite 3:
  
  You will be using the ``react-router`` and ``react-router-dom`` package in this application. So, ensure that you have added all the dependencies before you begin working on the project.

- External pre-requisite 4:
  
  If you are not aware about HTML5's drag and drop functionality, do read up on it before beginning this project. You should be able to drag an element from any part of the HTML and drop it at another designated point.


## Web application mock up

(pictures to be added here)

<br />

## User Stories

### User Story #1

User should be able to view all his boards.

#### Details

The homepage which can be opened using the URL ```https://localhost:8080``` should show a list of all the boards that are created by the user. If there are no boards created by the user, then the following message should be shown on the screen:
```
You haven't created any boards. Kindly click on the 'Create Board' button in the navigation bar to create a board.
```

On clicking a board, the user should be directed to the details of that particular board.

<br />

### User Story #2

User should be able to create a new board.

#### Details

You should create a component which shows a form to create a board. This form should be available as a 'new page' in SPA context, that is, on typing in the URL ```https://localhost:8080/createboard```, it should open the page with the form. There should also be a button on the navigation bar which will open this page.

The form should ask for the following inputs from the user:
- Name of the board.
- Team members who will be a part of this board. (Member names should be separated by commas)
- Type of board (e.g. Design board, Testing board, etc.) [This should be an optional field]

On clicking the <kbd>Create Board</kbd> button in the form, the details entered by the user should be added to a database on Firebase and the corresponding board should be shown on the home page.

<br />

### User Story #3

User should be able to view all the columns and cards inside his created board.

#### Details

When the user clicks on a particular board, he/she should be directed to a board details page where he/she can view the columns and cards. When the user clicks on a card, he/she should be able to see the following:
- Title
- Subtitle which should have the board name.
- Description (if any)
- Members name in circular representation with the initials.
- Due date.

Additionally, every card should have an ```Edit``` option as a button. Once the user clicks on Edit, a form pre-filled with the current information should be shown to the user for editing.

<br />

### User Story #4

User should be able to create a new column inside a board.

#### Details

The user should be able to create a new column by clicking on the **Add Column** button as shown in the diagram below. On clicking the button, a modal should open which asks the user to enter a name for the column. On hitting **Create**, a new column should now be shown in the board details page.

<br />

### User Story #5

User should be able to create a new card in any board.

#### Details

Inside every column, there should be 'Add Card' button which will open up a modal with a form containing the following input boxes:

- Title of the card
- Members that should be a part of this card (this should be a dropdown from which the users can multi-select the members)
- Description
- Due Date

On clicking <kbd>Add Card</kbd> button, the modal should vanish and the card should be added to the corresponding column.

<br />

### User Story #6

User should be able to drag and drop a card from one column to another.

#### Details

Using the principles of HTML5's drag and drop functionality, the user should be able drag a card from one column and move it to another. If the user moves a card from, say, column A to column B, the card should no longer be seen in column A and it should only be seen in column B. Use Firebase to maintain a central data repository for achieving this.

<br />

### User Story #7

User should be able to archive and he should be able to delete a column or even a board.

#### Details

Buttons for deleting should be appropriately placed on every card/column/board, allowing the user to delete it. On deletion, the same should be reflected on Firebase and inside the application.



The above functionalities are the minimum expected of you. You are free to add as much personalization as you want in terms of style.











