# campUS(Web Version)
-------
A University based community building app/website that enables students on campus to help each other and gain points, resulting in them being more recognized. Students can post their requests, and other people on campus can view their requests and attend to their requests, enabling students on campus to assist each other at times of need, while ensuring that they form valuable connections and networks in the process.

<hr>

## Project Structure

Here's an overview of the project structure:

- **public**: Contains static assets like HTML files and images.
- **src**: The main source code directory.
  - **assets**: Store your project's assets such as images, fonts, and styles.
  - **components**: React components used throughout the project.
  - **pages**: Individual page components or route components.
  - **firebase**: Firebase configuration and related files.
  - **App.jsx**: The main application component.
  - **index.js**: Entry point for the application.
- **.env**: Environment variables for development.
- **vite.config.js**: Vite configuration file.
- **package.json**: Project dependencies and scripts.

<hr>

## Tech stack used:
The tech stack used here is:

- React JS
- Tailwind CSS
- Google Firebase
- Vite

<hr>

#### Before contributing look into [CONTRIBUTING GUIDELINES](./CONTRIBUTING.md)
#### Our Code of Conduct: [CODE OF CONDUCT](./CODE_OF_CONDUCT.md)
<hr>

## Project setup instructions:
 
- **Fork the repository** to your GitHub account by clicking the "Fork" button at the top-right corner of this page. This will create a copy of the repository under your account.

- **Clone your forked repository** to your local machine using Git. Replace `your-username` with your GitHub username:

   ```
   git clone https://github.com/your-username/campUS-Web.git
   cd campUS-Web
   ```
   
- **Install project dependencies** using npm (Node Package Manager):
  ```
  npm install
  ```

- **Create a new branch** for your contribution. Replace *'feature/your-feature-name'* with a descriptive branch name related to your contribution:
  
### Replace Firebase Configuration

To use your own Firebase project with campUS-Web, follow these steps to replace the Firebase configuration:

1. **Create a Firebase Project**:

   - Go to the [Firebase Console](https://console.firebase.google.com/).
   - Click on "Add project" and follow the on-screen instructions to create your project.
   - Once your project is created, navigate to the project settings.

2. **Generate Firebase Configuration**:

   - In the Firebase project settings, scroll down to the "Your apps" section.
   - Click on the "Web" app icon (</>) to add a web app to your project.
   - Register your app by giving it a nickname and enabling Firebase Hosting if needed.
   - After registering your app, you'll be provided with a Firebase configuration object that looks like this:

     ```javascript
     const firebaseConfig = {
       apiKey: "YOUR_API_KEY",
       authDomain: "YOUR_AUTH_DOMAIN",
       projectId: "YOUR_PROJECT_ID",
       storageBucket: "YOUR_STORAGE_BUCKET",
       messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
       appId: "YOUR_APP_ID"
     };
     ```

3. **Replace Firebase Configuration**:

   - Open the `src/firebase/firebase.js` file in your campUS-Web project.
   - Replace the existing Firebase configuration with the configuration you obtained from Firebase Console.

   Example:

   ```javascript
   // src/firebase/firebase.js

   import { initializeApp } from "firebase/app";

   const firebaseConfig = {
     apiKey: "YOUR_API_KEY",
     authDomain: "YOUR_AUTH_DOMAIN",
     projectId: "YOUR_PROJECT_ID",
     storageBucket: "YOUR_STORAGE_BUCKET",
     messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
     appId: "YOUR_APP_ID"
   };

   const app = initializeApp(firebaseConfig);

   export default app;


### Development

- Make your changes or additions to the codebase. Test your changes to ensure they work as expected. To run the website on your localhost:
   ```
  npm run dev
   ```

- Commit your changes with a descriptive commit message:
  ```
  git commit -m "Add your descriptive message here"
  ```

### Push Changes

- Push your changes to your forked repository on GitHub:
  ```
  git push origin feature/your-feature-name
  ```

<hr>

## Getting started with contributions

- ### Create a Pull Request (PR)

Visit the [campUS-Web](https://github.com/gdsc-jssstu/campUS-Web) repository on GitHub.
Click the "Compare & pull request" button next to your recently pushed branch.
Follow the PR template and guidelines. Provide details about your changes.
Submit the PR.

- ### Review and Merge

The maintainers will review your PR and may request changes or provide feedback.
Once your PR is approved, it will be merged into the main repository.

<hr>

## Final version of the project

<!--- Place the link to the Figma file inside () --->
Click [here](https://www.figma.com/proto/MfbtIqwt0fjPtmWOuQ7yCQ/CampUs?type=design&node-id=12-364&t=9JuB3TEFpHrqwBXt-1&scaling=min-zoom&page-id=0%3A1&starting-point-node-id=12%3A364) for the UI design and prototype of the project.

<hr>

## Intended final project:

A responsive and aesthetically designed university-community building website called campUS(Web version).

 <hr>

## Thank You

Thank you for contributing to campUS-Web! Your contributions help make this project better for everyone.
If you have any questions or need further assistance, please don't hesitate to reach out to us.

<hr>

## Maintainers
1) [Syed Hisham Akmal](https://github.com/sikehish)
1) [Sanjay M](https://github.com/sanjay14073)
