
### Welcome

Welcome to the craft demonstration portion of your interview. After a brief introduction to the team, you will be asked to demonstrate your web development talent by implementing an application based upon the below requirements. Allow yourself about 45 minutes to develop your application. At the end of the session, you will have an opportunity to ask the team any questions you may have.

The machine provided to you has some commonly used tools. Feel free to install anything else you need to be productive. Installed already are:
  - homebrew (`brew install foo`)
  - npm (`npm install bar`)
  - create-react-app (`create-react-app`)
  - yeoman's create-redux-app (`yo create-redux-app`)
  - atom, vscode, and sublime
  - chrome, firefox, and safari

You may start from scratch, or may decide to **clone this repo**, which has been bootstrapped with `create-react-app`:
  - `git clone https://github.com/pabo/react-app-interview.git`
  - `cd react-app-interview/my-react-app`
  - `npm install`
  - `npm start`

### Exercise Requirements

Develop an Interview Wizard Application (IWA). The purpose of the IWA is to ask the user one or more questions in order to learn more about them. The expectation is that each question is displayed on its own screen/view inside the wizard. In addition, it is also expected that the wizard can be embedded on a page easily in widget-type form; thus, this widget must assume that it can’t control the page that it’s on. After the user has answered all three questions, all questions and answers should be displayed to the user.
The following are specific requirements:

  - Coding:
    - **React JS** framework is preferred, but you may choose another
    - Must be **mobile responsive**
    - A CSS pre-processor can be used, but is not required (e.g. Less/Sass)
  - How it should work:
    - Ask three questions, one question per screen
    - The user should be able to give their answer through an input field
    - The question ordering should be easy to change
    - After the the last question, the user should be taken to a final summary page with all the questions and answers displayed
  - If you have time:
    - The user should be able to revisit previous questions
    - Each question in the wizard should display one of the provided images
      - https://github.com/pabo/react-app-interview/raw/master/images/icon-accurate-retina.png
      - https://github.com/pabo/react-app-interview/raw/master/images/icon-max-refund-retina.png
      - https://github.com/pabo/react-app-interview/raw/master/images/icon-audit-support-retina.png
    - add CSS styling
    
---    
    
### Design Specs 

> See the design spec in `./specs/widget_spec.png`

#### Questions Screen

- Widget should be vertically and horizontally centered in screen
- Widget max-width is 700px
- Internal elements should be horizontally centered (image, question, input)
  - Question and Input should not exceed 500px in width
- Nav buttons should left aligned and right aligned respectfully to the width of the above elements
- Image is dynamic. Each question should show a different image
  - The image is to be done as a background-image, not an <img />
  - Find the images in ``./images`
- Remove the "back" button for first question   


#### Answers Screen

- List out the questions and answers
- No need for any input
- Remove the "next" button
- Remove the image, or add a custom hero image for bonus points 