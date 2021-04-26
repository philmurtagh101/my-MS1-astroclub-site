# Astroclub Website
As an amateur stargazer I have had the pleasure of engaging many acquaintances and sharing experiences and events about a topic that without exaggeration could be regarded as the beginning and end of all sciences. Yet for many it remains an abstract and an obscure puzzle not at all helped by the unsociable hours and the very hard to follow text-dense websites associated with this subject. This exercise will be a small attempt to rectify the latter.

Astroclub is designed to be a first stage responsive website for an astronomy club based in  Dublin/ Ireland to rapidly illustrate the wow factor of astronomy, deliver some immediate use for first time and regular  visitors and be an entry point for club members and prospective registrants.
 
## UX
The UX process employs the 5 planes approach as follows:
### Astroclub Objectives
* (Enable a site called Astroclub) Provide site visitors and club members with a resource comprising regionally relevant information on astronomy mainly via YourSky
* (Provide callout or hero statement) Provide a small impactful showcase of what astronomy is about enabled by a carousel
* (Provide images showcase - NB: no member upload on this version) - Provide a gallery of astrophotography (images contributed by members of club)
* (Frontend Only - no data capture) Allow members to login / register to join club
* (Frontend Only - no data capture) Allow visitors to leave a message
* (Location specific link -from "ClearOutside") Give up to date information on nighttime viewing conditions
* (Static Only) - Give a monthly Astonomy related events list together with a map of the area's night sky
* (Not implemented - not feasible at this time) Provide member login and registration backend
* (Not implemented - not feasible at this time) Automate the YourSky features on Night Sky and Events - would require populating separate database 
* (Not implemented - not feasible at this time) Provide educational guides on observation and types of equipment and setups to use
* (Not implemented - not feasible at this time) Be a pointer to a selection of resources on astronomy - education, buy and sell, events and meetups etc.
* (Not implemented - not feasible at this time) Provision online tools to help members for observation
* (Not implemented - not feasible at this time) Provide database and resources for members to upload contributions, calendar of events etc
* (Not implemented - not feasible at this time) Capture locale information based on visitor IP and/or GPS to facilitate a geo context for nighttime viewing.

### Scope
Scope will be defined in terms of 3 types of user - the CLUB, the member and the visitor. This to be done in the context of those objectives that are 

* As an astronomy club I want to provide in impactful landing page to attract visitors and new members in North Co. Dublin 
* As a Visitor I want to leave a message with the club
* As a Member/ Visitor I want to access a link to give me  observation conditions in North Co Dublin
* As a Member/ Visitor a gallery of images to view latest member astrophotography contributions
* As a Member/Visitor I want to access social media to allow access to relevant clu contributions there. 
* As a Member/ Visitor I want look up a page to access the latest skymap and events for my area
* As a member I want to be able to login to Astroclub to access other functions 
* As a visitor I want to be able to register to become a member of Astroclub
* As an astronomy club I want to capture registration information to help  build a view of astronomy experience in membership.


### Structure
IXD/ Interaction design is for an audience of hobbiests/interested parties who need certain specific information which relates to the time of day and their location. The subject matter is astronomy and the questions being immediately addressed is why? What it like tonight in my area, what can you see? are there examples and finally, how can I become a member?

IA/ Information architecture will comprise a mix of a simple inked set of pages starting from the home and working out to a number of other facilitory pages.  It is one level deep and the information types comprise links, images, tables and forms.

The layout is HERE

In all, there will be 4 web pages.

### Skeleton
The  wireframe illustrating the home, yoursky, gallery and members pages is available HERE

The approach is use the Bootstrap Framework leverage its grid structure by dividing site pages into 3 columns (or 3 groups of 4 columns) to allow for a clean responsive design as one moves from a large screen down to mobile phone. Headers and footers will be consistent across all pages and will provide the website navigation elements as well as links to social media and ability to check viewing conditions and leave a message

### Surface

As one would expect with this subject matter, the site will be dark with many examples of deep sky and planetary images used as background or as information. The colors are primary and bright yellow with shading and borders to help the images pop out more. The aim is to keep text to a minimum.  Images shall be the main conveyor of information.

## Features
 
### Existing Features
- Why Astronomy? - Pictorial carosel illustrating the wow factor
- Clear Outside? - allow user to check viewing conditions - it's a link to the Clear Outside website with geo coordinates supplied for Dublin.
- Events for the month - provide table of key highlights
- Skymap - Show current Skymap with approximate locations (where relevant) of events
- Gallery - show latest set of astrophotography contributions
- Member Login/ registration
- Leave a message

Reference the specific project files that implement them?

### Featuresto Implement in future versions
- Allow site to track your GPS so it can give you specific information relevant to your location - e.g viewing conditions, skymap and events at your precise time/locale.
- Complete the backend to the membership login/ registration
- Complete backend for messages left on site
- Provide mechanism for selected members to upload images 
- Provide a new section for members on educational how-to and links to other sites of interest
- Provide membership functionality for astronomy related buy and sell and pointers to related links
- Implement a community events pages for meet-ups either inside or external to club.

## Technologies Used

HTML 5 for main markup
CSS 3 for styling
Bootstrap 4 as a framework for styling, responsive design and some of the features
JavaScript for buttons, modal forms and styling
JQuery to support bootstrap
Font Awesome for the Icons - Social (Facebook, Twitter and Instagram), Cloud-Moon for CLear outside and Mail for leaving a message
Google Fonts for the Zen Dots font for the club brand
Balsamique for wireframing

NB: provide a link to  official sites and a short sentence of why it was used.

## Testing 

In this section, you need to convince the assessor that you have conducted enough testing to legitimately believe that the site works well. Essentially, in this part you will want to go over all of your user stories from the UX section and ensure that they all work as intended, with the project providing an easy and straightforward way for the users to achieve their goals.

Whenever it is feasible, prefer to automate your tests, and if you've done so, provide a brief explanation of your approach, link to the test file(s) and explain how to run them.

For any scenarios that have not been automated, test the user stories manually and provide as much detail as is relevant. A particularly useful form for describing your testing process is via scenarios, such as:

1. Contact form:
    1. Go to the "Contact Us" page
    2. Try to submit the empty form and verify that an error message about the required fields appears
    3. Try to submit the form with an invalid email address and verify that a relevant error message appears
    4. Try to submit the form with all inputs valid and verify that a success message appears.

In addition, you should mention in this section how your project looks and works on different browsers and screen sizes.

You should also mention in this section any interesting bugs or problems you discovered during your testing, even if you haven't addressed them yet.

If this section grows too long, you may want to split it off into a separate file and link to it from here.

## Deployment

This section should describe the process you went through to deploy the project to a hosting platform (e.g. GitHub Pages or Heroku).

In particular, you should provide all details of the differences between the deployed version and the development version, if any, including:
- Different values for environment variables (Heroku Config Vars)?
- Different configuration files?
- Separate git branch?

In addition, if it is not obvious, you should also describe how to run your code locally.


## Credits (I am too vain to give anyone credit :-))

### Content
- The text for section Y was copied from the [Wikipedia article Z](https://en.wikipedia.org/wiki/Z)

### Media
- The photos used in this site were obtained from ...

### Acknowledgements

- I received inspiration for this project from X
