# Web-Worker
This demo shows how an ajax call can be made to fetch thousands of record without blocking UI

I think this technique should be adopted throughout the projects specially for mobile development projects.
Web worker runs the bulky script in the background thereby not blocking the UI and thus giving a smooth User Experience.

There are three files in this sample project. 
1. index.html file contains inline style and script to call web-worker.
2. worker.js is the main web-worker file that has the bulky logic for ajax request. It process json in the 
   background and returns the data with postMessage funtion.
3. test.json contains sample records with multiple entries for over 8000 records.

To run the sample, just open index.html with mozila firefox as chrome doesn't 
allow web worker to run when served from local file system due to security reasons.
See how animation runs smoothly even though the record is fetched from json.
