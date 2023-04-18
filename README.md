Overview
--------

This project is a React web application that integrates with AdminJS, an open-source admin panel solution, to allow administrators to create customized forms for claiming EU flight delay and cancellation compensation. The application features automatic translation, unique URL generation, form auto-filling, and saving all entries to a CSV file.

Requirements
------------

*   Node.js
*   React
*   Formik
*   Yup
*   react-i18next (for translation)
*   AdminJS
*   Backend server (e.g., Express.js or similar)
*   Database (MongoDB) for storing unique form links and admin data

Main Components
---------------

### 1\. Admin Dashboard (AdminJS)

A secure dashboard built using AdminJS that allows administrators to create new forms and manage existing ones. Features include:

*   Authentication and user management
*   Creating new forms
*   Generating unique URLs for each form
*   Adding pre-filled data to eliminate repetitive entries
*   Viewing and managing existing forms

### 2\. Custom Form UI

A separate user interface for the form component, built using React, Formik, and Yup, for users to fill out and submit their claims. Features include:

*   Automatic translation using react-i18next
*   Auto-filling of form fields based on received data (e.g., phone number or email)
*   Validation of form fields
*   Submission of form data to the backend server

### 3\. Backend Server

A server built using Express.js (or a similar framework) to handle form submissions, unique URL generation, and interaction with AdminJS. Features include:

*   Integration with AdminJS for authentication and user management
*   Storing form data in a database
*   Generating unique URLs for each form
*   Providing endpoints for the custom form UI to interact with the server
*   Saving submitted form data to a CSV file

User Flow
---------

1.  The administrator logs into the AdminJS dashboard.
2.  The administrator creates a new form using the dashboard.
3.  A unique URL is generated for the form.
4.  The administrator adds pre-filled data (e.g., phone number or email) to the form.
5.  The form is sent to users via a link containing the unique URL.
6.  Users fill out the form in the custom form UI, which is auto-filled based on the received data.
7.  Users submit the form.
8.  Form data is saved to a CSV file on the server.


Form libraries to be implemented in the form or equivalent ones
---------------------------------------------------------------

//https://github.com/nchaulet/node-geocoder

//https://github.com/kenany/icao

//https://www.npmjs.com/package/react-datepicker

//https://github.com/tunyanghevond/react-airlines-list



# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
