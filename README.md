# Crystal Labeija's Salon

#### By: Ryan Broadsword

#### Application that allows the user to add/edit/view Stylists and add/edit/view Clients and assigns a client to a single stylist. 

## Technologies Used

* C#
* .Net 5
* REPL
* CSS
* HTML
* SQL
* MySQL Workbench 
* Entity


## Description 

Crystal Labeija's Salon
You've been referred by Pierre to his friend Crystal who is the owner of a hair salon called Crystal's Salon. She has contracted you out to create an MVC web application to help her manage her employees (stylists) and their clients. Crystal should be able to add a list of stylists working at the salon, and for each stylist, add clients who see that stylist. The stylists have specific specialties, so each client can only see (belong to) a single stylist.

User Stories
* As the salon owner, I need to be able to see a list of all stylists.
* As the salon owner, I need to be able to select a stylist, see their details, and see a list of all clients that belong to that stylist.
* As the salon owner, I need to add new stylists to our system when they are hired.
* As the salon owner, I need to be able to add new clients to a specific stylist. I should not be able to add a client if no stylists have been added.

## Setup/Installation Requirements

### Clone project
* clone repository
* open in vs code
* open terminal
* in terminal run "dotnet build" to make sure everything is up to date.
* in terminal run "dotnet test" to see test results for functionality. 
* in termianl run "dotnet run" to run the program and follow the prompts given in the console. 
* select localhost:5000/ to launch application in browser.

### Create your database schema and tables! 
* In MySQLWorkbench create a new schema named hair_salon
* Create a new table called clients
* In clients table add the following columns: 
  * ClientId with Datatype: INT, select boxes PK, NN, and AI
  * Name with Datatype: VARCHAR(255)
  * StylistId with Datatype: INT
* Create a new table called stylists
* In stylists table add the following columns: 
  * StylistId with Datatype: INT, select boxes PK, NN, and AI
  * Name with Datatype: VARCHAR(255)
  * Specialty with Datatype: VARCHAR(255)

### Create appsettings.json
* navigate to project folder in terminal "cd HairSalon"
* In termianl add "touch appsettings.json" 
* in the appsettings.json file add "{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=hair_salon;uid=root;pwd=[YOUR PASSWORD HERE];"
  }
}
* add your password for SQL where it says pwd=[YOUR PASSWORD HERE] 


## Known Bugs

* Should not be able to add client if no stylists are added


## License

Not currently licensed 

Copyright (c) July 30th 2022, by Ryan Broadsword rbroadsword@gmail.com 
