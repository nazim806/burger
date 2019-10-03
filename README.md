# burger

**Overview**
 
A Node, Express, Handlebars, and MySQL burger app that lets users input the names of burgers they'd like to eat and then devour them!  The site uses Node and MySQL to query and route data in the app, and Handlebars to generate HTML. Please check out the launched app on Heroku!

Burger is a restaurant app that lets users input the names of burgers they'd like to eat. Whenever a user submits a burger's name, app will display the burger on the left side of the page -- waiting to be devoured. Each burger in the waiting area also has a Devour it! button. When the user clicks it, the burger will move to the right side of the page. Burger app will store every burger in a database, whether devoured or not.



**Functionality**
Using an home-grown ORM, the app has 3 basic CRUD functions...

READ all entries from the MySQL database and display them to the DOM using Handlebars.
UPDATE a selected burger by clicking "Devour It", which... * hits an /burger/eat/:id route in Express to change its "devoured" status in the MySQL database * re-routes the webpage back to the index, where the burger is now in the devoured column (via Handlebars)
CREATE a new burger using the "Place Order" form, which... * hits a /burger/create route in Express to insert a new burger into the MySQL database * re-routes the webpage back to the index, where the burger is now ready to be eaten column (via Handlebars)


![burger image] (./assets/img/burger-page.png)
