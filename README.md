# Astroclub Website
As an amateur stargazer I have had the pleasure of engaging many acquaintances and sharing experiences and events about a topic that without exaggeration could be regarded as the beginning and end of all sciences. Yet for many it remains an abstract and an obscure puzzle not at all helped by the unsociable hours and the very hard to follow text-dense websites associated with this subject. This exercise will be a small attempt to rectify the latter.

Astroclub is designed to be a first version of a responsive website for an astronomy club based in  Dublin/ Ireland to rapidly illustrate the wow factor of astronomy, deliver some immediate use for first time and regular  visitors and be an entry point for club members and prospective registrants.

---
 
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
---
### Scope
Scope will be defined in terms of 3 types of user - the CLUB, the member and the visitor. Stories derived to achieve objectives are

1. As an astronomy club I want to provide in impactful landing page to attract visitors and new members in North Co. Dublin 
2. As a Visitor I want to leave a message with the club
3. As a Member/ Visitor I want to access a link to give me  observation conditions in North Co Dublin
4. As a Member/ Visitor a gallery of images to view latest member astrophotography contributions
5. As a Member/Visitor I want to access social media to allow access to relevant clu contributions there. 
6. As a Member/ Visitor I want look up a page to access the latest skymap and events for my area
7. As a member I want to be able to login to Astroclub to access other functions 
8. As a visitor I want to be able to register to become a member of Astroclub

---
### Structure
IXD/ Interaction design is for an audience of hobbiests/interested parties who need certain specific information which relates to the time of day and their location. The subject matter is astronomy and the questions being immediately addressed is why? What it like tonight in my area, what can you see? are there examples and finally, how can I become a member?

IA/ Information architecture will comprise a mix of a simple inked set of pages starting from the home and working out to a number of other facilitory pages.  It is one level deep and the information types comprise links, images, tables and forms.

## Project File Structure 
<img src="/assets/project/AstroFileStructure.jpg"> 

## Interaction/ Site layout 
<img src="/assets/project/AstroSiteMap.jpg">
---

### Skeleton

The approach is use the Bootstrap Framework leverage its grid structure by dividing site pages into 2 or 3 containers or grid columns to allow for a clean responsive design as one moves from a large screen down to mobile phone. Headers and footers will be consistent across all pages and will provide the website navigation elements as well as links to social media and ability to check viewing conditions and leave a message. The following 4 wireframes give the expanded large screen layout.  Pink lines indicate the grid/ container structure with a view of how this flows to smaller displays. 

## astroclub|home 
<img src="/assets/project/AstroHome.jpg">

## astroclub|yoursky 
<img src="/assets/project/AstroYourSky.jpg">

## astroclub|gallery 
<img src="/assets/project/AstroGallery.jpg">

## astroclub|members 
<img src="/assets/project/AstroMembers.jpg">

When moving to smaller devices(tablets and downwards) the navigation bar would collapse to a hamburger icon.

### Surface

As one would expect with this subject matter, the site will be dark with many examples of deep sky and planetary images used as background or as information. The colors are primary and bright yellow with shading and borders to help the images pop out more. The aim is to keep text to a minimum.  Images shall be the main conveyor of information.

## Features
 
### Existing Features
- Why Astronomy? - Pictorial carosel illustrating the wow factor See [home page code](index.html)
- Clear Outside? - allow user to check viewing conditions - it's a link to the Clear Outside website with geo coordinates supplied for Dublin. [Clear Outside](https://clearoutside.com/)
- Your Sky [Code here](yoursky.html)
    - Events for the month - provide table of key highlights
    - Skymap - Show current Skymap with approximate locations (where relevant) of events
(and yes, the west is correctly shown to be on the right)

- Gallery - shows latest set of astrophotography contributions. [Code Here](gallery.html)
- Members Page - [code here](members.html)
    - Member Login
    - Registration


### Features to Implement in future versions
- Allow site to track your GPS so it can give you specific information relevant to your location - e.g viewing conditions, skymap and events at your precise time/locale.
- Complete the backend to the membership login/ registration
- Complete backend for messages left on site
- Provide mechanism for selected members to upload images 
- Provide a new section for members on educational how-to and links to other sites of interest
- Provide membership functionality for astronomy related buy and sell and pointers to related links
- Implement a community events pages for meet-ups either inside or external to club.

## Technologies Used

- HTML 5 for main markup
- - used [HTML DOM](https://www.w3schools.com/js/js_htmldom_css.asp) to effect CSS changes eg
```
 <button onclick="regForm()" class="btn btn-secondary">Want to be a member&#63;</button>
-
-
<script>
        function regForm() {
            document.getElementById("registration").style.display = "block";
            document.getElementById("registration").style.background = "rgba(180, 180, 180, .8)";
        } </script>

```
- CSS 3 for styling
- [Bootstrap 4.2](https://getbootstrap.com/docs/4.2/getting-started/introduction) as a framework for styling, responsive design and some of the features
- JavaScript for buttons, modal forms and dynamic styling
- JQuery to support bootstrap
- [Font Awesome](https://fontawesome.com/) for the Icons - Social (Facebook, Twitter and Instagram), Cloud-Moon for CLear outside and Mail for leaving a message
- [Google Fonts](https://fonts.google.com/?query=zen+dots) to render the Zen Dots font for the club brand
- [Balsamiq](https://balsamiq.com/) for wireframing

## Testing 

### Code Testing
There were 4 HTML files  and 1 CSS file
HTML files Index, yoursky, gallery and members.html were put through the [W3C Markup Validation Service](https://validator.w3.org/).  All errors and warnings found were cleared.
Similarly, CSS file style.css was put through the [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/) and again all errors and warnings found were cleared.

### Responsiveness Testing
Used chrome browser developer tools and checked across a number of devices  Site seemed to collapse as expected as with smaller devices with no overlaps or unsightly issues with text, images or forms. Used a [responsiveness checker](https://www.responsivedesignchecker.com) to check across a range of devices with no issues found.

### Browser compatibility
Using [Powermapper](https://try.powermapper.com/) I checked IE, Edge, Firefox, Safari, Opera, Chrome, IoS and Android. All seem to check ok.

### Google Lighthouse Ratings
The biggest issue raised are the image load times.  Images vary in size and certainly would benefit from re-engineering for resolution and level of compression. 

### Behavioural testing
***
#### 1. As an astronomy club I want to provide in impactful landing page to attract visitors and new members in North Co. Dublin 

|Item to be tested|Expectation|Result|
|-----------------|-------------|------|
|Site loading|loads header and footer and background picture and plays carousel of 4 slides|ok|
|Slide captions|forward and back arrows for 4 images| ok|
|Colors,Fonts, Branding|fonts ,icons,color and sizing| ok|
|Navigation bar and links|bold for active page. Hamburger icon activating as one goes to tablet size and correctly activating dropdown menu with link for active site bold|ok|
|Hovering|Brand(Astroclub) and Icons all go to orange on hover|ok|
|Moving between pages|links going bod on active page and all working in each page|ok|

***
#### 2. As a Visitor I want to leave a message with the club

|Item to be tested|Expectation|Result|
|-----------------|-------------|------|
|Contact Us icon|  pops a modal form|ok|  
|Validation| Click submit on any combination of empty fields error message is shown|ok| 
|invalid email address format" and error message is shown|ok|
|Enter correct data|valid email in email field and  enter text in text area and it submits| ok|

***
#### 3. As a Member/ Visitor I want to access a link to give me  observation conditions in North Co Dublin

|Item to be tested|Expectation|Result|
|-----------------|-------------|------|
|Clear Outside icon|opens NEW tab on browser to https://clearoutside.com/forecast/53.52/-6.27 |ok|

***
#### 4. As a Member/ Visitor a gallery of images to view latest member astrophotography contributions

|Item to be tested|Expectation|Result|
|-----------------|-------------|------|
|Gallery Link|Redirects to gallery page and shows a gallery of 3 column wide (large display) one column wide other displays|ok|
***
#### 5. As a Member/Visitor I want to access social media to allow access to relevant club contributions there. 
|Item to be tested|Expectation|Result|
|-----------------|-------------|------|
|Social Networking Icons|select any of the social icons - Facebook, Twitter and Instagram and new page is opened in a NEW tab|ok|
***
#### 6. As a Member/ Visitor I want look up a page to access the latest skymap and events for my area
|Item to be tested|Expectation|Result|
|-----------------|-------------|------|
|YourSky link|redirects to YourSky page which displays a static table and static skymap for month of June 2021|ok|
***
#### 7. As a member I want to be able to login to Astroclub to access other functions 
|Item to be tested|Expectation|Result|
|-----------------|-------------|------|
| Members link|This redirects to the members page|ok|
|validation check|submit without entering data (email and/or password) and you should get an error message|ok|
|Email format check|you get an error message on clicking submit|ok|
|Submit correct data|Submits successfully|ok|

#### 8. As a visitor I want to be able to register to become a member of Astroclub
NB : still in "Members" Page
|Item to be tested|Expectation|Result|
|-----------------|-------------|------|
|click on Want to be a member?| A registration form is revealed (really a hidden image revealed bt HTML DOM CSS modifier)|ok|
|Validation Check|Click on submit button with any combination of fields firstname, lastname, email, password or repeat passwork empty and it should generate an error message|ok|
|Enter invalid email format|gives error message|ok|
|Experience dropdown| it works and allow change from "newbie"|ok|
|equipemnt checkboxes| Any combination can be ticked or unticked|ok|
|Primary Interest radio buttons| are working and that only one can be selected and that default is "fun"|ok|
|On submit with correct inputs|form dissappears|ok|

## Deployment
It is assumed that the entire project code and assets was pushed from GITPOD to the GITHUB repository at [My Repo](https://github.com/philmurtagh101/my-MS1-astroclub-site) 

Steps to enable site Deployment
1. Within [My Repo](https://github.com/philmurtagh101/my-MS1-astroclub-site) select settings
2. Scroll down to "GitHub Pages" and select "Check it out here!"
3. Under "Source" select branch "Branch:master" and select folder "/(root)"
4. Click on "Save" button

Website wwill publish from within the GITHUB repository to [AstroClub](https://philmurtagh101.github.io/my-MS1-astroclub-site/index.html) within 5-10 minutes.


## Credits 

### Content
What became evident as I researched many of the sites was the many features that could be leveraged to enhance one's own site. One trivial example being
[Clear Outside](https://clearoutside.com/) which would allow one to add latitude and longitude to customise for your own area.  Other sites offer skymaps that can give all the data to display your own dynamic map on your site (knowledge of using APIs and JS needed)


### Media
Images came from screen copy or image download from the following sites

- Sunspot Corona [wiki sunspot](https://en.wikipedia.org/wiki/Sunspot)
- NGC6543 Catseye [wiki catseye nebula](https://en.wikipedia.org/wiki/Cat%27s_Eye_Nebula)
- M31 Andromeda Galaxy [wiki andromeda](https://en.wikipedia.org/wiki/Andromeda_Galaxy)
- M27 Dumbell Nebula [wiki dumbell nebula](https://en.wikipedia.org/wiki/Dumbbell_Nebula)
- Planet Jupiter [wiki jupiter](https://en.wikipedia.org/wiki/Jupiter)
- Great Red Spot [wiki red spot](https://en.wikipedia.org/wiki/Great_Red_Spot)
- NGC 869 and NGC 884 Double Cluster [wiki double cluster](https://en.wikipedia.org/wiki/Double_Cluster)

- The Sky Map came from [In the Sky](https://in-the-sky.org/skymap2.php)

### Acknowledgements
- To my Mentor Antonija Simic for suggesting the carousel to use for the home page and bringing me on a whirlwind tour of Bootstrap and some testing methods.
- To Code Institute's Whiskey Drop Lesson for the approach on the Navbar and Modal forms and on the Resume lesson on the footer icons.
- To Code Institutes tech support for getting over road blocks on getting CDNs loaded.
