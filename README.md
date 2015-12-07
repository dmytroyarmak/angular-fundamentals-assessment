# Angular Fundamentals Assessment

Create a simple Angular.js application to manage shopping list.

Prerequirenments:
- basic knowladge of JS
- basic knowladge of Angular.js:
  - [AngularJS Fundamentals](https://egghead.io/series/angularjs-app-from-scratch-getting-started)

Shopping list is a list of shopping items that have following properties:
- name:string - name of an item
- quantity?:number - a quantity of items (optional)
- unit?:string - unit of measurement for quantity (optional)

List of items:
- When a user opens the application, there should be a default list of items (3 - 5). 
- All properties of an item should be visible on the list.

Deleting of items:
- Each item in the list should have delete button 
- A user should submit deleting of an item by clicking "OK".
- Confirmation window should have the text: "You are going to delete ${name of item}. Are you sure?".

Adding new items:
- There should be a button to add a new item to the list of items.
- By clicking add new item button, form with three fields, submit and cancel button should appear.
- Name field should be required.
- A new item shouldn't be created on form submit if the form is invalid.
- Submit button should be disabled when the form is invalid, and the user tried to submit the form.
- If the user tried to submit the form and the 'name' input is invalid, there should be the message "Name of an item is required" under the input.
- If the form is valid and the user submits it, and a new item should be created, added to the end of the list and "add new item" form should be closed.
- If the user clicks "Cancel" button, "add new item" form should be closed without creating an item.

Editing of items:
- Each item in the list should have edit button
- When the user clicks "edit" button, form similar to "add new item" form should appear under the list.
- All validation logic should be the same as for "add new item" form.
- Data in the list shouldn't be changed when the user is editing fields in inputs.
- Only when the user submits the form, data in the list should be updated.
- Form should be hidden after successful submitting
- When the user clicks "edit" button, and there is "add new item" form that already opened, there should be confirmation window with text: "You're creating new item already. Do you want to edit ${name of item} instead?". If the user clicks yes, "add new item" form should be closed, and "edit item" form should be opened instead.
- When the user clicks "edit" button, and there is "edit item" form that already opened, there should be confirmation window with text: "You're editing an item already. Do you want to edit ${name of item} instead?". If the user clicks yes, current "edit item" form should be changed to the new one.

What you shouldn't do:
- No routing.
- No data persistence.
- No user authentication and authorization.
- No backend.
