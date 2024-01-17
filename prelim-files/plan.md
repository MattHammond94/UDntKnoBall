# Plan/initial idea

### Stack/Technologies

> NEXT and Typescript.

> Having used MongoDB for my past 3 projects I want to get back to using SQL with a relational database. The data being used in the project is definintely relational but how I decide to create the database and query it is a matter of experimentation for now to find what works best for me and the project.

> Third party library/package for both input validation and log in: I spent a lot of time during my last full stack project working on secure log in functionality and also sanitising user inputs at each possible stage. As I'm comfortable with this now I'd like to explore and implement a package to handle all of this. Firebase is an option.

> API - I have not yet decided which api I will be using to provide the results data that the user inputs will be compared to. There are multiple Premier League API's but some seem overly vrbosed with the sheer amount of data they are able to provide. For now I only really need the score and winner of a fixture but this may well change in future versions depending on what I am allowing users to predict. 

> User emails! - I want some nicely designed reg emails along with general correspondence/updates so this is a nice change and something that I have not yet explored. 

> Taking payment! - for later versions (one I have completed the MVP) I want each league created to have a buy in. Each league would then have a prize pot which would be awarded to the winner of a league. This poses a lot of exciting new challenges when it comes to taking payments. The Stripe API is a good starting point.

### Potential Edgecases:

> Some things I will need to consider before implementing anything is what would happen in the instance of any of the below scenarios: 

* Blank GW's
* Double GW's 
* suspended/resheduled/abandonned matches
* A cut off time for when results can be submitted by for each gameweek. 
* A set time for when results are tallied (All data would need to be received for each GW before results can be tallied.)
* Will users be defaulted to inputting a result of 0 - 0 each week if they cease to be active? 
* What effects could this have if results do return 0 - 0 and the inactive user continues to accumulate scores.
* Year after year the premiership teams will change (Based on promotion and relegation) how will this be handled?

### V1 (MVP)

> V1 will only have one league/pot which users can CHOOSE to join or simply spectate the league results if they prefer.

> Users can log in and log out and join said league.

> users have a profile where they can view stats/results.

### V2 

> A user can create their own league table and invite others to join.

> A pot of money is incremented by each user who joins the league and this money will be awarded as prize money to the victor of each league. 

### Styling/theme 

> I'm still not a fan of bootstrap OR tailwind for handling styling so for now the use of good old vanilla CSS will continue to be my choice. I feel the more I use vanilla CSS the better my understanding of what is happening under the hood in a widely used CSS library gets. Where possible, it would be nice to add some Sass elements to differentiate my design but unfortunately this will be lowest on the list of priorities.

