Hello everyone. 
My name is Mirjana Stamenkovic and I want to thank you for the opportunity you gave me by sending me this interesting task to solve. 

I developed a Windows Forms Application in C#.NET in Visual Studio 2019. 
The name of the application is SearchApp. 
The database I used is Microsoft SQL Server 2019. 
Credentials for connecting to SQL Server are:
Server name: DEV01 
Authentication: Windows authentication.
I created a new database and named it TechnicalTest2021.I created a new table dbo.results and filled it with data.
From this table user collects information while searching, and updates data accordingly.
Connecting the application to the database is done via the connection string, which is stored in file:Connections.xml. 
This file is located in the application path (SearchApp\SearchApp.UI\bin\Debug).

Windows Forms Applications in C#.NET:
This application-SearchApp is created as Solution that consists of only one Project(since the app is small), which is UserInterface (UI).
Typically, when larger applications are involved they would contain multiple layers(Projects) such as: 
-DB layer in which database-related information and transactions are stored. 
-BL layer where the business logic is, like Classes(Entities) used in the application.
Theese Projects would be created as Class Libraries,and built to dll-s.
-And, of course the main UI Layer for User Interface, which contains user forms and other relevant informations, and builds to an exe.
Additional Layer would be shared library with features used throughout the application.
This would ususaly be stored in static Classes and Methods.

Informations about C# SearchApp:
When the user starts the application, the Main-menu form opens. This form is of type-MdiContainer and it contains links to other forms. 
There are 2 options user can choose: 
The main option is -Search for results, in which the task is located. 
Second option is: Test scenario, and it's no less important then the main option.
In test scenario, user can preview original data from database, and filter it in several ways.
While opening this form, all data from the table: results are loaded immediately. 
It is possible for the user to enter a word (or part of word), to filter the data from the table. 
For example enter word: mic and press the refresh button. It is also possible to select the appropriate radio buttons to search by certain criteria. 
Then, user should click the button: Generate data for drop-down, where the main logic for the task is stored.
This generates data that should appear in the drop-down list (in the main option-Search for results).
In the main option- Search for results, user should type min 3 letters and select the word from drop-down list(combo-box). 
Each time a result is selected it is recorded in the database, by increasing the value of weight by 1 (in table results). 

Informations and instructions for creating a database, table and filling in the data, are stored in another file: Database.txt.

I wish you a nice day and successful testing. 
And that you like my application :)

