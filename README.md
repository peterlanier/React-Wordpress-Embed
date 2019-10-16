This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## React WordPress Embed
A good starting point is the first commit which is ready for a new app. I followed [this](https://medium.com/@CodeCareerCoach/react-app-inside-a-wordpress-page-or-post-4c7d38181b3d/?target=_blank) tutorial.

#### Add filters to functions.php
```
remove_filter( 'the_content', 'wpautop' );
remove_filter( 'the_excerpt', 'wpautop' );
```
#### Add homepage to package.json
```
"name": "wp-react-component",
"version": "0.1.0",
"homepage": "http://domain.com/wordpress/permalink/here/",
"dependencies": {
...
```
#### Setup a unique DOM target in the WP page and App.js
```
<noscript>
  You need to enable JavaScript to view this page.
</noscript>
<div id="my-box-page">
</div>

<script src="/demo/wpsandbox/react/static/js/main.bdd480c8.js"></script>
```

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

This project was ejected from the first commit
