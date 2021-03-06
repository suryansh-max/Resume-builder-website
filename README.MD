# Resume Builder

**Gotta find a job!** Alright, let's make a new resume with this awesome template I found on Google, the problem is, this template might not be as awesome next month, or you might need to constantly add your new experience to the document. Gosh. Wouldn't be better to focus on adding new experiences in a raw format and let a automation process handle the layout? I agreed, and that's why Resume Builder is here.

#### You take care of the data and we take care of the template.

> "Imagine you're an employer, and you have two resumes in front of you. One is filled wall-to-wall with text and uses four different fonts. It's also peppered with dozens of bolded, italicized, and underlined words and phrases.
   The second resume also offers a lot of information, but you can quickly scan the document because it makes good use of white space, features clear and consistent section headings, and uses bullets to make important items stand out.
   Which resume would you look at first?"
- [http://monster.com](https://www.monster.com/career-advice/article/resume-look-important-as-content)

<img src="/screenshots/v3/resume_builder.gif?raw=true" width="890px">

**TESTED ONLY ON GOOGLE CHROME**

## About
[Resume Builder](https://resume-builder.js.org) is a free open-source project that allows anyone to easily maintain and build any kind of resume using Google Spreadsheets. This was develop as a personal project to help a friend who was struggling spending up to an hour to make a custom resumes. **[TRY IT NOW](https://resume-builder.js.org).**

For version 1 [check here](https://github.com/suryansh-max/Resume-Builder/blob/main/README_V1.MD) and for version 2 [check here](https://github.com/blopa/Resume-Builder/blob/main/README_V2.MD).

## Features
- Multiple Resume templates (soon)
- Parse data from Google Spreadsheet URL, .xls file or .json file.
- Support Json format from [jsonresume.org](https://jsonresume.org/schema/).
- Convert Google Spreadsheet data into [jsonresume.org](https://jsonresume.org/schema/) format.
- Theme created with [material-ui-theme-editor](https://in-your-saas.github.io/material-ui-theme-editor/), so it's easy for you to customize.



## Usage
First of all you need to create a Google Spreadsheet following the same rules as [this one](https://docs.google.com/spreadsheets/d/1UCdsEiyO68IEdfVhW-Gfrg7FfI4pLaij37D5Eh-v8hQ/copy) (you can make a copy if you like) and populate with your resume information.
- **name:** Your full name
- **label:** Your resume Job Title
- **picture:** A URL for your picture
- **summary:** Summary of yourself
- **website/url:** Your website URL
- **email:** Your email
- **phone:** Your phone number
- **address:** Your address
- **postalCode:** Your postal code
- **city:** City where you're located
- **region:** Region where you're located
- **countryCode:** Country code where you're located
- **network:** Social media name
- **username:** Social media name

## Libraries
- I'm using [gatsby.js](https://github.com/gatsbyjs/gatsby), [react.js](https://github.com/facebook/react), [js-xlsx](https://github.com/sheetjs/js-xlsx) and [Material UI](https://material-ui.com/).
- Honorable mentions: [babel](https://github.com/babel/babel), [webpack](https://github.com/webpack/webpack), [IntelliJ IDEA](https://github.com/JetBrains/intellij-community).
- Gatsby template from [gatsby-material-ui-blog-starter](https://github.com/suryansh-max/gatsby-material-ui-blog-starter)

So a big thanks to all the developers that worked really hard on these libs and make our day easier :D.

## Deployment
Run `npm run build` then copy the `public/` folder into your website root directory. Done.

## Example
The following ``JSON`` is a result of [this Google Spreadsheet](https://docs.google.com/spreadsheets/d/1UCdsEiyO68IEdfVhW-Gfrg7FfI4pLaij37D5Eh-v8hQ/edit). For a better view of the ``JSON`` [click here](https://codebeautify.org/jsonviewer/cb7c68a1).
```json
{
  "basics": {
    "name": "John Doe",
    "label": "Programmer",
    "picture": "",
    "email": "john@gmail.com",
    "phone": "(912) 555-4321",
    "website": "http://johndoe.com",
    "summary": "A summary of John Doe...",
    "location": {
      "address": "2712 Broadway St",
      "postalCode": "CA 94115",
      "city": "San Francisco",
      "countryCode": "US",
      "region": "California"
    },
    "profiles": [{
      "network": "Twitter",
      "username": "john",
      "url": "http://twitter.com/john"
    }]
  },
  "work": [{
    "company": "Company",
    "position": "President",
    "website": "http://company.com",
    "startDate": "2013-01-01",
    "endDate": "2014-01-01",
    "summary": "Description...",
    "highlights": [
      "Started the company"
    ]
  }],
  "volunteer": [{
    "organization": "Organization",
    "position": "Volunteer",
    "website": "http://organization.com/",
    "startDate": "2012-01-01",
    "endDate": "2013-01-01",
    "summary": "Description...",
    "highlights": [
      "Awarded 'Volunteer of the Month'"
    ]
  }],
  "education": [{
    "institution": "University",
    "area": "Software Development",
    "studyType": "Bachelor",
    "startDate": "2011-01-01",
    "endDate": "2013-01-01",
    "gpa": "4.0",
    "courses": [
      "DB1101 - Basic SQL"
    ]
  }],
  "awards": [{
    "title": "Award",
    "date": "2014-11-01",
    "awarder": "Company",
    "summary": "There is no spoon."
  }],
  "publications": [{
    "name": "Publication",
    "publisher": "Company",
    "releaseDate": "2014-10-01",
    "website": "http://publication.com",
    "summary": "Description..."
  }],
  "skills": [{
    "name": "Web Development",
    "level": "Master",
    "keywords": [
      "HTML",
      "CSS",
      "Javascript"
    ]
  }],
  "languages": [{
    "language": "English",
    "fluency": "Native speaker"
  }],
  "interests": [{
    "name": "Wildlife",
    "keywords": [
      "Ferrets",
      "Unicorns"
    ]
  }],
  "references": [{
    "name": "Jane Doe",
    "reference": "Reference..."
  }]
}
```

## Screenshot
**[Google Spreadsheet example](https://docs.google.com/spreadsheets/d/1q8ladKrXRa9BhBybB_2q0ujMRHy2VytWFDxwOrOJlK4/edit?usp=sharing)**
![ScreenShot](https://raw.githubusercontent.com/blopa/Resume-Builder/main/screenshots/v3/screenshot_1.png)

  www.github.com/suryansh-max/Resume-builder-website/screenshots
 


