# CovidPass
The project will create an universal Covid passport (being a single point of truth for Covid tests results) containing bar code for quick check at the borders of foreign countries and places like restaurants, airports, embassies, hotels, etc. 

## Problem to solve
Many countries including mine are being banned from travelling to other countries to stop Covid contagion. The main reason why my country was banned from travelling to Singapore, UEA and other countries is because travelers 
from my country were allowed to travel while they were positive to Covid-19. This because in my country, when you are tested, the care provider print a simple paper where it is stated wether you are positive or negative to COVID. 
This kind of certificate is not secure because, using paint of photoshop, the individual can alter their result from positive to negative in order to get the travelling VISA. 


Actually,There's no way to check whether the COVID test result in the printed paper is genuine or fake: many other key partners countries have threatened to ban my country if the care authorities are not able to stop these bad practices. That's why this project was created. It will help everyone (the embassies all around the world, borders security agents, hotels, restaurants etc.) 
to have the correct test result that was registered by the care provider when the individual was tested. With this, no one will be able to cheat on the result. 
In addition, the project will maintain a dashboard of Covid statistics all around the country.

 ## Roadmap
 1. Create a brand new web API project
 2. Care providers registration 
 3. Care providers profiles validation
 4. Individual registration and COVID test results updates
 5. Bar code generation 
 6. Alert individual about their results availability 
 7. Create web clients for all roles (including care providers, security agents, care authorities, embassies)
 8. Scanning bar code and submiting to web api and get the result
 9. Create Covid statistics dashboard
 10.Publish in azure or other web hosting

 ## Next steps
  1. Create android client
  2. Create iOS client

 ## Want to contribute?
Create a branch and a pull request: I will commit once a day befaure 10 PM (GMT). Please follow but don't change the following architecture:

 - **CovidPass.API** is a net core 6 web API, MVC and Angular app for administrators, care providers, and other checkers (embassies, hotels, airports...): USE ROLE AUTHORIZE ATTRIBUTE
 - **CovidPass.Context** is the .net Standard 2.1 project for data access logic (dbContext, entities and repositories): YOU SHOULD PUT YOUR DATABASE ENTITIES HERE
 - **CovidPass.Models** is the project for all view models (targeting .net Framework 4.7 optionally): PUT YOUR VIEW MODELS HERE
 - **CovidPass.Mapping** is the automapper profiles project: PUT YOUR AUTOMAPPER PROFILES CLASSES HERE
