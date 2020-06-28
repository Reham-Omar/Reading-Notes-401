#  React Testing and Deployment

## React Testing

- You can test React components similar to testing other JavaScript code.
- There are a few ways to test React components. 

* Snapshots - Make assertions on the exact rendered markup (with content) at any state of the application.
* Render Testing - Similar to snapshots, but allows for jQuery-like inspection of the virtual DOM tree
* Shallow Testing - Executes and renders the called/container component, but does not compose children.
* Mounting - Executes the full component and children. Allows for inspection of rendered Virtual DOM as well as the current state

- Jest is a JavaScript test runner that lets you access the DOM via `jsdom`.

## Deployment

- React in development mode uses a node service to create a live website that refreshes as you write code. 
- This is NOT what actually gets deployed when you want your React website to go live. 
- React, remember is an index.html file that uses Javascript to render components in the browser.
- The node server is only there to aid in your development.

### Deploying to GitHub Pages

- Enable GitHub Pages on your domain, using the gh-pages branch
- Create a Personal Access Token in your GitHub account
- Add this token as a “Secret” called PERSONAL_TOKEN in the repository housing your react app
- Add the react workflow .yml file to your repository (in .github/workflows)