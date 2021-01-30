# Online-Offline-Budget-Tracker

## Table of Contents
[Description](https://github.com/dhfoss/Online-Offline-Budget-Tracker/#description)  
[Functionality](https://github.com/dhfoss/Online-Offline-Budget-Tracker/#functionality)   
[Usage](https://github.com/dhfoss/Online-Offline-Budget-Tracker/#usage)  
[Questions](https://github.com/dhfoss/Online-Offline-Budget-Tracker/#questions)

### Description
https://polar-depths-96609.herokuapp.com/  
Think this is a normal budget app that merely keeps track of your funds? Think again! This website is made for a modern day on-the-go user who might not have internet service at every single second. That's right, update your transactions anywhere, anyhow, and as soon as you get in range of some sweet sweet pulp-free fresh squeezed internet juice, this will automatically update, without having to raise a finger. So make that dough and watch it rise baby!

### Functionality
When the website loads, a service worker is registered to the browser, as well as all the necessary files for the app to work offline.  
![Cache](/screen-shots/1-Cache.png?raw=true "Cache")

One of the files loaded is `db.js`, which initiates an indexedDB to the page.  This will save any transactions while the app is offline.  When the user re-establishes an internet connection, the data in the indexedDB will get saved to the MongoDB.  
![IndexedDB](/screen-shots/2-IndexedDB.png?raw=true "IndexedDb")

### Usage
Using the Website is a simple matter of typing in a monetary amount, then clicking add or subtract from total funds. If the network connection is cut before finishing the transaction, the browser will update thanks to the service workers. Upon reconnection, the site will send the data to MongoDB Atlas.  
![UI](/screen-shots/3-UI.png?raw=true "UI")

### Questions
For questions contact me at:  
Email: dhfoss89@gmail.com  
https://github.com/dhfoss

Thank you, and happy budgeting!  
-DHF
