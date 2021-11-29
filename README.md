# Tic-Tac-Toe

![MIT LICENSE](https://img.shields.io/github/license/William-Krug/tic-tac-toe)
![REPO SIZE](https://img.shields.io/github/repo-size/William-Krug/tic-tac-toe)
![TOP_LANGUAGE](https://img.shields.io/github/languages/top/William-Krug/tic-tac-toe)
![FORKS](https://img.shields.io/github/forks/William-Krug/tic-tac-toe)

# Tic-Tac-Toe

## Description

_Duration: 2 Week Sprint_

Directly above this is how long it took you to develop the project. Your project description goes here. What problem did you solve? How did you solve it?

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed aliquam at massa in faucibus. Etiam volutpat, risus non mollis convallis, velit nisi pulvinar mi, eu faucibus orci nisi eget nibh. Integer a velit pretium, volutpat arcu eleifend, fringilla elit. Cras erat sapien, convallis venenatis tellus vitae, feugiat dictum felis.

Suspendisse euismod volutpat aliquet. Maecenas vulputate mauris in pellentesque facilisis. Phasellus varius malesuada semper. Cras sollicitudin diam mollis maximus aliquam.

To see the fully functional site, please visit: [DEPLOYED VERSION OF APP](www.heroku.com)

## Screen Shot

Include one or two screen shots of your project here (optional). Remove if unused.

### Prerequisites

Link to software that is required to install the app (e.g. node).

- [Node.js](https://nodejs.org/en/)
- List other prerequisites here

## Installation

How do you get your application up and running? This is a step by step list for how another developer could get this project up and running. The good target audience in terms of knowledge, would be a fellow Primer from another cohort being able to spin up this project. Note that you do not need a paragraph here to intro Installation. It should be step-by-step.

If your application has secret keys (for example -- Twilio), make sure you tell them how to set that up, both in getting the key and then what to call it in the `.env` file.

1. Create a database named `your database name`,
2. The queries in the `tables.sql` file are set up to create all the necessary tables and populate the needed data to allow the application to run correctly. The project is built on [Postgres](https://www.postgresql.org/download/), so you will need to make sure to have that installed. We recommend using Postico to run those queries as that was used to create the queries,
3. Open up your editor of choice and run an `npm install`
4. Run `npm run server` in your terminal
5. Run `npm run client` in your terminal
6. The `npm run client` command will open up a new browser tab for you!

## Usage

How does someone use this application? Tell a user story here.

1. xxx
2. xxx
3. xxx
4. xxx
5. xxx
6. xxx

## Built With

List technologies and frameworks here

## License

[MIT](https://choosealicense.com/licenses/mit/)

_Note, include this only if you have a license file. GitHub will generate one for you if you want!_

## Acknowledgement

Thanks to [Prime Digital Academy](www.primeacademy.io) who equipped and helped me to make this application a reality. (Thank your people)

## Support

If you have suggestions or issues, please email me at [youremail@whatever.com](www.google.com)

## GitHub Repo

### Branching

- Branches are created from the `dev` branch of the repository
- Branch (story branch) names are based off of ticket id (i.e. `TTT-##`)
- To create a new branch: `git checkout -b <story branch>`

### Pull Request (PR)

- Pull requests are to be made after all feature development and testing scripts have been written
- **PR Title** is the title of the ticket (i.e. "TTT-##: Ticket Title")
- **PR Comment** should clearly outline the work performed on the branch
- An approver needs to be assigned and team pinged about new branch
- Branch needs to be assigned to requester

### Merging into `dev`

- Branches **ARE NOT** merged from GitHub
- Commits need to be "squashed" to keep `dev` clean
- Branches should be deleted after PR has been approved and branch merged into `dev`
- Once approved, branch owner commits the branch as follows:
  1. `git checkout dev`
  2. `git fetch --all`
  3. `git pull origin dev`
  4. `git merge --squash <story branch>` (Resolve any merge conflicts before continuing)
  5. `git commit -a -m "<story branch>: <story title>"`
  6. `git push origin dev`
  7. `git branch -D <story branch>`
  8. `git push origin :<story branch>`

### Deploying to `main`

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

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

### `yarn build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
