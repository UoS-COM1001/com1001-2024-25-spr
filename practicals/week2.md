# Week 2: Queries and Forms

**In your teams**, if you haven't already, decide what forms are going to be
needed as part of your web application. How will the different pages are your
application link together, and how much of this will be driven by forms and
query strings?

Before getting started on writing any forms for your team project, try the
following exercises first to be sure you understand the basics. You can do these
on your own, or collaboratively as members of your a team.

Try to write a simple Sinatra application that handles a form, like the examples
covered in lectures. Then:

1. Set up a view with a form that has three fields. Make two versions, one that
   uses the `get` method to submit the form and one `post` that uses the post.

2. Get the receiving route (the one that the `action` attribute in the `form`
   tag sends the form data to) to print the values of each of the form fields
   entered to the web page. Don't forget to "escape" those values! (See the
   lecture slides as to how to do this)

3. Add some sanitisation and validation to the form. Ensure leading and trailing
   spaces are stripped from the user entered form field values. Ensure the first
   field is a valid string of no more than 10 characters. Ensure the second
   field is an integer. (Think about how to program the code needed to do these
   checks.) Ensure your view properly reports errors to the user if one or both
   of the fields is not entered correctly.

4. Try to achieve the same effect as the `get` form submission by
   programming a view with a link where the URL has a query string that encodes
   two values corresponding to each field of the form. Again, if you're unsure,
   consult the lecture slides. If you're still unsure, ask your demonstrator!

5. Finally, attempt this week's [challenges](../challenges/week2.md).