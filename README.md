# MS1 – Tobias Kast Portfolio / Resume Website

![Am I responsive screenshot](/readme_assets/Am_I_Responsive.jpg)

[The website](https://apometricstk.github.io/ci_ms1_portfolio/index.html) is intended to give recruiters and potential employers a fast and conclusive overview of my skills, experiences and qualifications.
As it is for educational purposes right now, not every skill is in mentioned state (e.g. "dummy content").

# Table of Contents
1. [UX](#UX)
2. [Features](#Features)
3. [Technologies](#Technologies)
4. [Testing](#Testing)
5. [Deployment](#Deployment)
6. [Credits](#Credits)
 
## UX

### Strategy & Scope

A selection of the major objectives and selected ways to achieve them in form of user stories and conclusions.

As a…

#### recruiter…

* I want to have a **fast** and **openly available** source of information on candidates to assess, so that I can make a quick screening and don’t waste my time and money on candidates not fitting my case. → Homepage

* I want to gather and connect my key information in a **quick first screening** and only dive deeper if the profiles match. → Key Information on landing page, accessible without further click.

* I want to **further assess** a potential candidate before contact. → More relevant Information on the site and connected sites. Use of known concepts in tech CVs (e.g. progress bars, tech-shortlits)

* I want to have a **fast** and **reliable** way to contact candidates on my shortlist, so that my recruitment process is not blocked by timing or contact issues. → Not too many, but reliable contact information, widely-used technology, business-orientation

#### website-owner…

* I want to get job offers fitting my profile. -> Selection of information to serve, prioritizing the focus bits (e.g. backend before frontend in tech skillsets)

* I do not want to publicly share my direct contact (phone number) with anyone visiting my homepage. I want to offer a fast and reliable way to contact me. → a contact form, connected with an e-mail alert and business networks

* I do not want a recruiter to misjudge me as a mainly design orientated person. -> Clean and fact orientated layout with some gimmicks (e.g. custom bullet-point), portfolio projects will set a focus, as soon as available.

### Structure & Skeleton

The major design decisions in form of wireframes.

"Burger-Button" / Navbar fixed top to scroll with screen.

![wireframes mobile](/readme_assets/wireframe_mobile.jpg)

![wireframes bigger as mobile](/readme_assets/wireframe_bigger.jpg)

### Surface

As pharma is a "white collar" business sector, I decided to match it with clean and plain colors, font and style.

![color palette](/readme_assets/coolors_palette2.jpg)

---

## Features

### Existing Features

### Meta
- The navigation menu allows every user to have full control over positioning on the homepage (as long as JavaScript is enabled in the browser). On small screens the collapse to a burger-menu saves “dead” screen-space and therefore enhances screen-space usable for information.

- The hero-image with name and title allows every user to remind himself on the person the information he reviews is connected to. It transports a core information to: The person reviewed is not a CS graduate but has working experiences in retail, healthcare, pharma and distributed organizations/branches.
Assess: dont show hero image on small screens (just show title) for all not-landing pages to enhance active screen-space?

- The disclaimer reminds users of the educational purpose of the website – some skills were added just to “have something to show” as part of the learning process. The intention is to replace the dummy content with actual skills as soon as the course is finished.

- The footer allows the user to jump to his preferred way of contact – e.g. contact-form, business networks or github.

- The color change of the link-buttons on mouse-over(hover) gives visual feedback to transport the click-ability to the user.

### Landing
- Key information is provided in an easy accessible and structured way.

- Key information for the recruiter: experience-fields (coding, sectors, development) and a link to the tech-skillset for further assessment.

- Key information for the recruiter: portfolio showcase (with tech-shortlist and short description) the external links to projects (dummies right now) provide work samples in detail.

### Work-History
Provides a classic CV. On wider screens a parallel column for educational and working history was chosen, to emphasize the parallel timelines of full-time work and education.

### Tech skill sets
Provides a tech-CV-like classification of different technology fields and skill-sets. The subgroups were provided with well-known logos to ease orientation for the viewer.

### Contact
Provides a contact form to allow users a direct contact. A text field provides space for messages and is with names and e-mail required to allow an answer.
A checkbox allows an urgent callback-message.

A modal informs about educational purpose of the homepage and that no data has been saved/submitted after “submit”-button has been clicked.
Note: As the “submit” button does not transmit the input messages, the “required” part of the inputs is not fully functional (just a red border, no mandatory-message). 

### Features left to Implement
* Build a dynamic timeline for the working history section, to emphasize the ongoing further education parallel to full-time-work by temporal positioning of elements.

* Contact form
    * Bind contact form to email-service (so the required feature works as intended)
    * Phone number required if urgency checked

* Add a schedule for occupied / free/bookable time.

* Add a "change-language" button and add translated german content.

* Add a "remote-work" or "based at" section, as soon as a preferred way of collaboration is chosen.

## Technologies Used

The website is build in a simple way on purpose. The user should not wait for many downloaded media-files or animations. Major CDNs were included (aware of the conflict with the aforementioned statement) to include up-to-date security patches of implemented JavaScript. 

The base technologies are HTML and CSS. Some JavaScript is used to achieve more efficient use of the viewport on mobiles (collapsing navigation-menu).

The hand made “cards” which are used as main design element for the different lists where chosen in preference of Bootstrap cards, as the [documentation (v4.1.x)](https://getbootstrap.com/docs/4.1/components/card/#card-layout) states layout options for series of cards are not yet a responsive element.

#### HTML
- for the main pages

#### CSS
- for everything styling related

#### JavaScript
- just for the Bootstrap nav-collapse feature

#### [Bootstrap](https://getbootstrap.com/)
- for the grid, the navigation menu, buttons and the contact-form modal

#### [Fontawesome](https://fontawesome.com/)
- for the logos to ease visual orientation

#### [Google Font *Roboto*](https://fonts.google.com/specimen/Roboto?sidebar.open=true&selection.family=Roboto)
- Roboto for a clean readable impresion

#### [gitpod](https://gitpod.io)
- as IDE

#### [code institute gitpod template](https://github.com/Code-Institute-Org/gitpod-full-template)
- as a starter for the gitpod environment

#### [code institute readme template](https://github.com/Code-Institute-Solutions/readme-template)
- as a starter for the readme.md

## Testing

### Validators
Validators were used by copy and pasting the code into the validator.
Strg+A, Strg+C -> Strg+V

#### HTML Validator
As the [HTML validator](https://validator.w3.org/) highlights an error...
* the attribute "type="text" was removed from the textarea of the contact.html.

As validator warns...
* about a misuse of "aria-label" if used to label non focusable Font-Awesomne icons, and the icons just help with visual orientation by representing the corresponding heading, the labels were removed.

* about a missing heading in disclaimer, a heading was added to the section.

Afterwards
* index.html
* work-history.html
* skillset.html
* contact.html
passed without errors or warnings.

#### CSS Validator
The styles.css was validated by [jigsaw validator](https://jigsaw.w3.org/css-validator/validator) and passed without errors.

### Manual testing

#### Firefox, deployed page
* All htmls were successfully "tabbed" in circle in desktop and mobile mode to assure keyboard-only usability and focusability of all links.

* All buttons were hovered and clicked to check the effect.

* All html were examined in small mode (340px width) and at major breakpoint (575, 576px). A previously, just sometimes observed bug of the "burger-button" moving to the left side of the screen and the media-query being ignored (Browser and machine independent, but not every-time reproducible) seems to be fixed.

* The inspector just throws an 404 error for the favicon. I dont expect ongoing bookmarking of the site and the title speaks for itself. The research just resulted in [presenting an empty favicon link](https://stackoverflow.com/questions/1321878/how-to-prevent-favicon-ico-requests). As the objective is not to present myself as a visual designer, the creation of a favicon was declined and doesn't seem to be necessary.

#### Chrome, deployed page
* The progress bars on the skillset.html seem to be slightly out of bound when observed on a big screen.  
    ![Chrome1](/readme_assets/chrome1.jpg) ![Chrome2](/readme_assets/chrome2.jpg)  
    but the problem were not observed on a smartphone or on a laptop with Chromium.
    ![Chrome3](/readme_assets/chrome3.jpg)  
    
    A further test on the laptop exposed an out of bound behaviour on Windows 10 with Chrome, but not on Manjaro with Chromium on the same display.
    Further investigation with the developer tools, Windows 10 scaling behaviour and zooming with Chrome suggests a dependency of the position of the bar and display-solution, scaling and zooming if the bug appears or not at all. Further investigation or trying to fix this minor issue was declined.  
    ![Chrome4](/readme_assets/chrome4.jpg)

* All htmls were scaled in viewport width and responsive behaviour was observed. On index.html the grid layout of the first skill group was eased.

### Slack review
The project was posted to Slack the Code Institute community channel peer-code-review for different pairs of eyes.

## Deployment

The content was deployed via GitHub pages by configuring the repository according to the [documentation](https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages).
Mainly setting the repository on “public” and configuring the “GitHub Pages” section in “settings – Options” of the repository.

For local use just download the code and open the files with your browser. I recommend to start by opening the index.html file.

## Credits

* Screen Size information by [hobo-web – Shaun Anderson](https://www.hobo-web.co.uk/best-screen-size/)

* Browser features by [caniuse.com](https://caniuse.com/)

* Wireframes drawn with [Draw.io](https://app.diagrams.net/)

### Content

* [Bootstrap](https://getbootstrap.com/) components used
    * Layout system
    * Navbar
    * Button
    * Modal

### Media

* The Font Awesome symbols were made by [Font Awesome](https://fontawesome.com/).

* The hero-image was taken out of private stock.

* The first readme screenshot was taken with [ami.reponsive](http://ami.responsivedesign.is/)

* The color palette screenshot was taken with [coolors.co](https://coolors.co/)

### Acknowledgments

* My mentor Brian Macharia for his support and feedback.

* The Code Institute slack community for their support.

* Inspiration was taken from 
    * [LouParkers MS1](https://github.com/louparker/iportfolio)
    * [thaysom22 MS1](https://github.com/thaysom22/portfolio_project)