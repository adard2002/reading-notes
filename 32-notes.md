# Reading 32 Notes

[Home](README.md)

# View Components

## What are view components?
View components are similar to partial views but more powerful. View components don't use model binding, they only depend on data provided when it's being called into. 

### View Component:
- Renders 1 chunk rather than a whole response.
- Includes the same separation of concerns and testablility benefits found between controllers and views.
- Can have parameters and business login.
- Typically invoked from a layout page.

### Where view components are usually intended for. Where ever you have reusable logic that is too complex for a partial view.
- Dynamic nav menus
- Tag cloud which is where it queries the database
- Login panel
- Shopping card like on amazon
- Recent published articles
- Sidebar content
- Login panel that would be rendered on every page and shows the links to login or log out, depending on the state of the user

## Parts of a view component
A view component has 2 parts: the class and the result it returns. 

### The view component class
A view component class can be created by the following:
- Deriving from ViewComponent
- Decorating a class with the [ViewComponent] attribute or derivin from a class with that attribute
- Creating a class where the name ends with the ViewComponent suffix
- Fully supports constructor dependency injection
- Doesn't take part in controller lifecycle. Meaning you can't use filters in the view component.