# Polymer + Firebase Q&A

A simple Q&A app built with Polymer and Firebase. Covers routing, authentication, material design, and CRUD operations.

- [Live Demo](http://polymer-qa.divshot.io/)
- [Video Walkthrough](https://www.youtube.com/watch?v=gErWcBdd-F8)

## Running Locally

Create a new app in Firebase. Set up a new GitHub application and [configure authentication](https://www.firebase.com/docs/web/guide/login/github.html) in Forge. Run the following command in your terminal:

    npm install && bower install

Edit `/app/elements/app.html` and change `<your-firebase>` to your Firebase URL:

```javascript
Polymer({
  ready: function() {
    this.globals.firebase = '<your-firebase>';
  },
```

Run the server locally with Grunt:

    grunt serve