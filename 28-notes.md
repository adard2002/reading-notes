# Reading 22 Notes

[Home](README.md)

# MVC Forms

## Views in ASP.NET Core MVC

1. Layouts: this can be used to avoid or reduce the amount of code repetition. This usually contains the header, nav, menu elements along with the footer. This is kind of like the css part of the site. The header and footer most of the time contain a boilerplate markup for metadata elements and links and script and style assets. This is also used to avoid boilerplate or default markup in your site.
2. Partial views: This is also used to reduce the amount of code repitition by managing reusable parts of views. 
3. View Components: These are similar to the partial views since they both allow reducing duplicated code and are appropriate for the view content making sure that the code can run properly so the site can render to the webpage. This is useful for when the rendered content requires interaction with the database like a shopping cart on amazon. 

### Benefits of using views
- Easier to maintain due to organization. Views are usually groups by the app feature and makes it easier to find related views when working on a certain feature.
- Parts are loosely coupled, being able to build and update the views apart from the logic and data access components. The views are easily modifyable and not having to worry about necessarily updating other parts of the app.
- Easier to test the user interface parts since the views are in separate files or units.
- Less likely to repeat secions of code of the user interface.

