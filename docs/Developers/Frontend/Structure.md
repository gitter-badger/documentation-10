## App Structure

The structure of the app is all held within the `src` folder. Here is a breakdown of the core folders inside:

* assets/ 
    * img/ - This contains all static images used by the app
    * styles/ - This folder contains all `scss` files for every component or view within the app
* components/ - These are reusable components that can be used in views throughout the app
* localisation/ - This folder contains all of the languages that the website supports (currently German and English)
* router/ - Contains all of the routes within the app and the components they are linked to. It also handles authorisation and validation of users and protecting certain routes
* store/ - This contains the combined state for the entire application, the structure is primarily matching the views folder
* views/ - This holds all of the main pages within the app, split by the model that they are linked to in the API
* test/ - Run both of these with `npm run test`
    * e2e/ - This contains all end to end tests and can be run with `npm run e2e`
    * unit/ - This contains all unit tests and can be run with `npm run unit`
* `App.vue` - This is the main app file that is kind of like the `index.html`
* `main.js` - This is your main file that sets up the Vue app. In our case, it generates the SDK, handles translations and sets up the store before launching the app. Plugins are added to Vue here.