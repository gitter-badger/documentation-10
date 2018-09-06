## Frontend

The front end of the C3S project is created using the Vue 2 framework and some key libraries for it. Most of the practise followed here is the same as most modern web apps, here are some key terms and their definitions:
* Vue - The framework used to create an modern web app
* Vuex - A package to enable `client side state` to be used within a Vue app
* State - A snapshot of the information held within a web app at any one time
    * Store - This is the object that holds keys and values. The store is **immutable**
    * Event - An event is `dispatched` on the store to carry out an `action`
    * Action - An action could be updating the store or retrieving data from a URL
    * Commit - This is a value to update the store with. For example, committing a `username` to the store
    * Subscribe - Components and/or views can subscribe to an item within the store to be told whenever it changes
* View - A page within a Vue web app (can also be thought of as a page)
* Component - A `view` can contain one or more components
* 