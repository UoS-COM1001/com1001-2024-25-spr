# Week 1 &mdash; Coding Challenges

1. a) Create an app with multiple routes, which could be spread across multiple
   controller files (up to you). Each should be a profile page for an academic
   teaching COM1001, so `/phil`, `/donghwan` etc.

   Make a view for each route that has our name and profile picture in (you can
   take our profile pictures from the GitHub repository, or elsewhere on the web).

   b) Add a default route `/` to the app, with links to each profile page. When
   the app is launched, clicking this links will take the user to each profile page.

   c) Make each page have a standard header and footer, e.g., with the
   University's logo featuring in the header. How might you organise this so you
   do not have to repeat the same HTML code for the header and footer in each
   view file?

2. Change your app so that now there is just one generic route for a profile
   page that takes a parameter --- the person whose profile page it is. (For
   example `/profile?person=donghwan`). The route sets the name and file for
   the profile picture and passes this to the view.



