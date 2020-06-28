# React Testing and Deployment

## React Testing

* Snapshots: Assertions on the exact rendered markup at any state of the application.

* Render testing: like snapshots but with inspection of virtual DOM tree.

* Shallow Testing: executes and renders the container component.

* Mounting: Executes full component and children.

## Deployment

* React in development mode uses node service to create live website, this is not what actually gets deployed if you want to deploy your website online.

* React uses index.html file that uses javascript to render components in the browser, node server exists only to help in development.

* After using `npm run build` it will output a website containing an index.html, .js and a .css files required to open the app.

* Steps to deploy to GitHub Pages:

1. Enable GitHub pages on your domain using gh-pages branch.
2. Create a personal access token in your GitHub account.
3. Add this token as secret called `PERSONAL_TOKEN` in the repository you are using.
4. Add react workflow.yml file to the repository.

* Doing this will initiate GitHub Action whenever you push or merge code into your repository.

* It will run the build command, create a new branch called gh-pages and deploy react static files.

## Deploying to AWS Amplify

* Create a new Amplify workflow
* Point the workflow to GitHub repo (master branch).
* Merge code to master on GitHub

## Deploying to Netlify

* Create a netlify.com account, then create a new application.
* Point the application to GitHub repo (master branch).
* Merge code to master on GitHub.
