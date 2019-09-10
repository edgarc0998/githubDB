1.  My first step was to set up my database. I just needed to keep track of sessions to make sure users dont vote from the same browser more than once, and also a way to store a vote. A vote stored the name of the framework a user voted for, their email, and a session id.
2.  I set up my back end routes. I made one route for posting a new vote, and a route to get all the current votes for each framewoke (all in one route). In the post route, this either returned an error, or a success. If it was an error, that means a user voted with that email already. In the other route(get all votes), I checked the user's session Id. If it was already in the database, I sent a message to the front end to notify users of this. 
3.  I set up my front end. I needed a simple home page with containers for the three charts, and the 4 buttons. The only other challenge was using the Github API to get information from the four repositories.
4.  After the front end was made, I had to hook it up the vote buttons to call the routes I made.  
5. Deployment was my final step. Here is the link. https://github-framework-poll.herokuapp.com/
6. I used fullstack academy's boilermaker code. This set up the basic express server with some logging middleware and some of the folder structure for the app. All the code I wrote is in the folders client, server, and public. 



To run code follow these steps:

1. git clone
2. npm install
3. npm run seed
4. then npm run start-dev
