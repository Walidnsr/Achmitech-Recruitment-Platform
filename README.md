# RecruitmentPlatform

## Description
RecruitmentPlatform is the source code of a sophisticated recruitment application developed for Achmitech. It serves as a bridge between recruiters and candidates, particularly freelancers. This repository contains the frontend code, which is built using Vue.js.

## Installation Instructions
To set up the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/NAJIilyass/RecruitmentPlatform.git
   cd RecruitmentPlatform
   ```

2. Install the dependencies:
   ```bash
   npm install
   ```

3. Run the development server:
   ```bash
   npm run serve
   ```

## Features
RecruitmentPlatform offers a wide array of features designed to facilitate the recruitment process for both clients and candidates. Key features include:

- **Home Page and User Interface (UI) for Authentication:** A welcoming home page and a seamless authentication process for users.
- **Client and Candidate Sections:** Separate interfaces tailored to the needs of clients and candidates.
  - **Clients:** Can post job opportunities, review candidate applications, manage profiles, and communicate with potential hires.
  - **Candidates:** Can browse job listings, submit applications, manage their profiles, and message recruiters.
- **Profile Management:** Both clients and candidates can create and maintain detailed profiles.
- **Messaging Functionalities:** An integrated messaging system to streamline communication between recruiters and candidates.

## Contact
For any questions or suggestions, feel free to open an issue or contact me at najiilyassoo@gmail.com.

```
RecruitmentPlatform-master
├─ .browserslistrc
├─ .gitignore
├─ babel.config.js
├─ jsconfig.json
├─ package-lock.json
├─ package.json
├─ postcss.config.js
├─ public
│  ├─ favicon.ico
│  └─ index.html
├─ README.md
├─ src
│  ├─ App.vue
│  ├─ assets
│  │  ├─ comments
│  │  │  ├─ ferme.png
│  │  │  ├─ Img1.png
│  │  │  ├─ Img2.jpg
│  │  │  ├─ Img3.jpeg
│  │  │  ├─ Img4.jpg
│  │  │  └─ ouvert.png
│  │  ├─ entreprises
│  │  │  ├─ aws.png
│  │  │  ├─ cgi.png
│  │  │  ├─ coatsal.png
│  │  │  ├─ dxc.png
│  │  │  ├─ ibm.png
│  │  │  └─ oracle.png
│  │  ├─ Eye.png
│  │  ├─ great
│  │  │  ├─ Ima1.png
│  │  │  ├─ Ima2.png
│  │  │  ├─ Ima3.png
│  │  │  └─ Ima4.png
│  │  ├─ Intro.png
│  │  ├─ left.png
│  │  ├─ Logo.png
│  │  ├─ Logo1.png
│  │  ├─ Popular
│  │  │  ├─ Img1.png
│  │  │  ├─ Img2.png
│  │  │  ├─ Img3.png
│  │  │  ├─ Img4.jpg
│  │  │  ├─ Img5.jpg
│  │  │  └─ Img6.jpg
│  │  ├─ right.png
│  │  ├─ SignUp
│  │  │  ├─ Img1.png
│  │  │  └─ Img2.png
│  │  ├─ Something
│  │  │  ├─ Img1.png
│  │  │  ├─ Img2.png
│  │  │  ├─ Img3.png
│  │  │  └─ Img4.png
│  │  └─ styles.css
│  ├─ components
│  │  ├─ componentsCandidat
│  │  │  ├─ accueilCandidat.vue
│  │  │  ├─ appCandidat.vue
│  │  │  ├─ appsCandidat.vue
│  │  │  ├─ menuNavBar.vue
│  │  │  │  ├─ messageMenu.vue
│  │  │  │  ├─ notifsMenu.vue
│  │  │  │  └─ profileMenu.vue
│  │  │  ├─ messagesCandidat.vue
│  │  │  ├─ msgBody.vue
│  │  │  ├─ msgCandidat.vue
│  │  │  ├─ navBar.vue
│  │  │  ├─ opportunitiesCandidat.vue
│  │  │  ├─ opportunityCandidat.vue
│  │  │  ├─ profileCandidat.vue
│  │  │  └─ sideBar.vue
│  │  ├─ componentsHome
│  │  │  ├─ ChiffresHome.vue
│  │  │  ├─ CommentsHome.vue
│  │  │  ├─ IntroHome.vue
│  │  │  ├─ NavBar.vue
│  │  │  ├─ NeedSomething.vue
│  │  │  ├─ OneComment.vue
│  │  │  ├─ OneGreat.vue
│  │  │  ├─ OneNeed.vue
│  │  │  ├─ OnePopular.vue
│  │  │  ├─ PopularHome.vue
│  │  │  └─ WhatGreat.vue
│  │  ├─ componentsSignUp
│  │  │  ├─ SignCandidat.vue
│  │  │  └─ SignClient.vue
│  │  └─ FooterView.vue
│  ├─ data
│  │  └─ data.js
│  ├─ main.js
│  ├─ pages
│  │  ├─ candidat
│  │  │  └─ HomeCandidat.vue
│  │  └─ layout
│  │     ├─ EntrepriseVue.vue
│  │     ├─ HomeView.vue
│  │     ├─ HowItWorksVue.vue
│  │     ├─ LoginView.vue
│  │     └─ SignUpView.vue
│  └─ router
│     └─ index.js
├─ tailwind.config.js
└─ vue.config.js

```