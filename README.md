READ ME
----------------------------------------------------------------------------------------------------
Target Framwork: .NET Framework 4.8
Visual Studio Version: 2022 Community
* This application makes use of MVC architecure

Welcome! This application is a prototype for the stock management of website of Farm Cental. 
The application will keep track all the famers, employees and products of the database.



CHANGES
----------------------------------------------------------------------------------------------------
The major problem of the code was that it was unable to load. This error did not happen on the original 
save of the project.

An error was found on the GitHub of the project. When pushing the application, GitHub ignores .mdf files.
This was changed by altering the .gitignore file. 

This same error happed with the dependency files. This resulted in an empty bin folder on the repository.
This must be fixed locally. 

Please run the following command in the package manafer console to solve this problem
Update-Package Microsoft.CodeDom.Providers.DotNetCompilerPlatform -r

A new GitHub link as been included with the updated files. If the application does not run from the local files,
please clone the code from the respository


RUNNING THE APPLICATION
----------------------------------------------------------------------------------------------------
Database:
If the database file is not working, update the database file by right clicking on it. 
If this does not work, run the following command in the package manager console: update-database
Please refer to the PopulateDatabase.cs file for the database data

Admin:
Username: Admin
Password: Password@123

Eployee1:
Username: Employee1
Password: Password@123

Farmer1:
Username: Farmer1
Password: Password@123


HOW TO USE
----------------------------------------------------------------------------------------------------
This is a navigation of the web application:
Home Page:
	In order to proceed use a premade account to login

If logged in with an admin or EMPLOYEE or ADMIN account:
	The home page contains 3 main areas: Farmers, Products and Product Types
	Each section can be either navigated by the home page or by navigation bar
Farmers:
	Here you can view all the current farmers in the database.
	There is a green button to add a new farmer.
		To add a new farmer fill in all the required user input, then press create
	To edit a farmer, click the edit link of the respective farmer account.
		Here some of the account information can be changed
		Once done, click the save button to save the changes
	To view the details of a farmer, click the detaisl link
		This shows additional information about the farmer
	To delete a farmer, click the delete link
		Deleting the farmer will also delete any assosiated products
		click the delete button to delete the farmer form the database
Types:
	Here you can view all the product types of the database.
	For a farmer to add a product, they need to specify the type, therefore it must be
	ensured that there is a sufficient number of product types
	This section works in the same way as the Farmer section (see above)
		Note: When deleting a product type, all the products in the database of 
		that type will be removed
Products:
	Here you can view all the products in the database that farmers have added.
	To select a specific farmer, use the drop down list to chose the farmer username.
	This will show the products of only the selected farmer.
	To filter products, click on the 'Type' or 'Date Added' headdings
	This will change the filtering system. 
	The current filter applied can be see under the page title
	The details of each product can be view, altough you cannot edit or delete any products
		

If logged in with a FARMER account:
	The home page contains 2 main sections and a quick link. To quickly add products, click
	the 'ADD PRODUCT' button
Product Types:
	Here is a list of all the types of products avaible in the database. When adding products
	to the database, a product type must be selected. The types will be from this list
Products:
	Here you can view all the products linked to the farmer profile. 
	To add a new product, click the grenn 'ADD NEW PRODUCT' button.
		To create the product, fill in all the user inputs and click the 'CREATE' button
		when done. 
		For the product type - see Product Types (above)
	To edit a product, click the edit link
	To delete a product, click the delete link
	To view the details of a product, click the details link.		












