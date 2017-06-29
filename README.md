# JAAM

WHY we brought JAAM into existence
==================================

We decided to build a responsive mobile-first website for our burgeoning web development business which described our mission, our team and how to get in touch with us. 

We decided to go mobile-first because many websites are visited via mobile.

We wanted a bold eye-catching design with dynamic elements to engage our viewers, bring a smile to their face and encourage them to stay on our page.


WHAT our site does
==================

Splash Page
----------
Our site begins with a bold and dynamic but clean splash page which simply contains our company name and tagline. The background changes colour to keep the user's attention and is a photo of raspberries which is a playful pointer to our company's name.

The navigation bar sits to the left and is wide enough to draw the viewer's eye and tell them how to navigate across our site. On top of that, the navigation bar expands to the right slightly and each icon lights up upon hover to indicate to the user that they are using the bar properly.

About
-----
The about section loses the bold image from the splash page to draw more attention to the text. We decided to split the text into three columns to save desktop users having to read all the way from one side of the screen to the other, therefore encouraging them to read it all.

As text can be a bit boring, we've also included a nice photo of us looking thoughtful which also serves as a nice end to the section!

Team
----
The team section lays out the 4 of us in a nice 2x2 box. The jam icons used mimic our logo in slightly different formats - this emphasises that we are a cohesive team and is also just nice and fun! The icons also expand and increase opacity upon hover to make the section appear more dynamic. 

Each team member has their 'role' listed as well as their individual links to Codewars, Github and Linkedin. These links change to a nice jam colour and a finger pointer upon hover to show the user that they are active.

Contact
-------
Our contact page commands the user to 'Get in touch!' to show them that this section is interactive. 

The form is laid out in a standard way which asks for the user's information first and then offers a section for additional info. The nature of request is offered using a dropdown menu to categorise it more quickly. This helps both the user and us who are receiving the request!

We should have a footer....

HOW it happened
---------------------------------------------------------------------
We started by going through the user stories and discussing how we’d approach the page.

We doodled a little bit.

Then we created issues for each user story and within that, issues for each big element that needs creating.

Then we decided for one pair to work on the navigation bar and one pair to create the form.

## Problems we had

__Navigation Bar:__

We decided on a vertical navigation bar which expands upon hovering. We initially tried not to use flex boxes for this but struggled to centre the elements vertically. Using flex boxes on the ul item was much easier (ul is essentially the container for the list items and these are what we wanted centred).

Had issue with padding on the ul element - was pushing all our icons on the nav bar to the right. We solved it by inspecting the elements on the browser and seeing the highlighted areas to see how they differ (padding shows in green). Turns out we forgot to remove the ul's default padding (duh). 

__Form Location__

To create the form we looked at examples on other websites, such as Founders and Coders, among other websites containing contact forms similar to what we were looking for. We knew we wanted a simple interface that was easy to use whilst still being accessible, as well as being responsive enough to be comfortably used on phones, tablets and larger screens. We knew that the various form inputs and the larger message box could potentially pose an issue when accessed on very small screens.

When we had created a form we were happy with we ran into trouble with our navigation bar as it slides out slightly on hover which meant that it would sometimes obscure parts of the form on smaller view-ports. We could not reach a solution for quiet a while as when we were able to stop the form from being obscured in smaller view-ports by using a margin; in larger ones the entire form would be off center.

When we eventually discussed the problem with the rest of our team members they had found a solution to the problem that had been affecting a different element they were working on. They had simply added a margin to the encasing `<main>` element so that everything shifted together.

__Form Background__

Another problem we had with the form was that the background colour we had used would extend upwards to the top of the section above, crossing through a separate section. We had seen that when we set our form element to `float: left` the background acted as we had expected it too, however the form was not positioned where we wanted it. Samatar suggested that the floats we had used in the section above could be the cause of the problem, and after adding a `clear: both` to the form the problem had been solved.
