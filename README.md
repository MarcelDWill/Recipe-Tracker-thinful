Recipe Tracking App Thinkful

    A CRUD application for tracking recipes!

Capstone Project for React rendering and state management

This project makes use of 4 React components to:

    Create new recipes -
        RecipeCreate creates a form on screen for users to type in new recipes and submit them to the page to be displayed
        stores its own state for form inputs
        uses createRecipe() as props to handle when user submits the form
    Format new recipes -
        RecipeFormat handles the input of a single recipe, and returns it formatted as a <tr> element with nested <td> elements for each key-value of the recipe.
        Adds a delete button to the recipe, using handleDelete() when button is clicked.
    List all available recipes -
        RecipeList renders full table display for all current recipes, using RecipeFormat to map the list of recipes to <tbody> element.
    App component -
        stores state for recipes, so all children have access if needed through props
        holds handleDelete() and createRecipe() methods to manage state of recipes, methods are passed to children as props
        returns <div> element with a header, our RecipeList table display, and the RecipeCreate form
