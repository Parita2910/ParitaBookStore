Name: Amin Parita Vipulbhai
Id:- 0773902 
Assignment2:- Bookstore

11:00 - Create new ASP.NET core(MVC) web application of name ParitaBookStore
11:00 - configuired the project
11:03 - Run the project
11:04 - create the github repository named Assignment2 and push the assignment2 to my github.

Oh It successfully ran.

11:08 - Go the bootswatch.com
11:08 - and selected the theme "SLATE"
11:09 - replaced the bootstrap.css file of the theme to current css file located in wwwroot folder.
11:10 - also replaced the main site.css file to the site.css file in the assignment2 folder in blackboard.
11:11 - changed file name from bootstrap.min.css to bootstrap.css
11:11 - Changed the nav class from navbar-light to navbar dark and bg-white to bgprimary
11:12 - add extrea properties to footer class text-white-50 and bg primary
11:13 - run the project  

yeah theme is successfully applied.

11:15 - In _Layout.cshtml, added the additional stylesheets and scripts from the file CSS_JS.txt file.
11:17 - Adding dropdown in navbar 
11:18 - run the project
11:20 - Adding three new project in application
11:20 - three new projects - ParitaBooks.DataAccess, ParitaBooks.Models, ParitaBooks.Utility
11:21 - copied data folder and pasted into new project .DataAccess 
11:21 - deleted the original folder
11:23 - Installed the packages: Microsoft.EntityFrameworkCore.Relational and Microsoft.EntityFrameworkCore.Sqlserver
11:26 - Deleted the migration folder
11:27 - Installed the Identity.EntityFrameworkCore
11:28 - In ApplicationDbContext.cs, changed the namespace to ParitaBookStore.DataAccess.Data
11:29 - Deleted all the Class1.cs files from .DataAccess, .Models and .Utility project
11:35 - Moved the models folder into ParitaBooks.Models
11:36 - In main project, Added the two project references - .DataAccess and .Models
11:38 - Changed the model folder name to Viewmodel
11:39 - run the project

Oops! Got some error in startup.cs file

11:42 - solve the error by using.ParitaBookStore.DataAccess.Data
11:43 - removed the using.RajviBookStore.Data
11:43- Corrected default reference @model RajviBookStore.Models.ViewModels.ErrorViewModel
11:44 - run the project

Oh finally it successfully run!

11:50- Added new class file named SD.cs in utility project
11:52 - added project reference in the main project
11:54 - added Models and Utility reference to .DataAccess project.
11:57 - Add a new area named Customer
11:59 - Deleted data and models folder from Areas and moved the HomeController.cs file to the Area>Customer>Controller
12:08 - run the application

run successfully but different webpage loaded

12:09 - copied the _ViewStart and ViewImport to customer area
12:10 - added the new path to _ViewStart.cshtml
12:11 - run the application

Yeah after solving the error it  successfully run

12:15 - Added a new area named Admin
12:16 - Deleted data and models folder from Admin area and copied _ViewStart and ViewImport to admin area
12:19 - Deleted the controller folder
12:20 - run the application

Successfully build.

Date:- 13/11/2021

9:00 - build the application and it successfully build
9: 01 - open the Nuget package manager console and run the command add-migration AddDefaultIdentityMigration 
9:06 - default project is ParitaBookStore so it showing error 
9:06 - select the ParitaBooks.DataAccess
9:07 - run the command add-migration AddDefaultIdentityMigration
//my migration folder name is :- 20211115021125_AddDefaultIdentityMigration
9:20 - to update the database run the command - update-database
9:20 - successfully build 
9:21 - checked the updated table in SQL server object explorer
9:21 - run the project

run successfully.

9:25 - created the new class file in .Models project.
9:26 - modified the code.
9:30 - added the migration via console by command - add-migration AddCategoryToDb
//my migration folder name is :- 20211115022846_AddCategoryToDb
9:35 - modify the applicationDbContext.cs file
9:38 - re-run the command - add-migration AddCategoryToDb
9:40 - edited the migrated file 20211115022846_AddCategoryToDb and checked the updated database 

and yeahhhh database is updated successfully......

10:00 - In ParitaBooks.DataAccess, created new folder name Repository
10:00 - In Repository folder, created new IRepository folder for interface
10:02 - In  IRepository folder, created the new interface and named it as  IRepository.cs
10:04 - Modified  IRepository.cs to perfoem CRUD operations.
10:06 - In Repository folder, created new class named  Repository.cs
10:06 - modified it but got some errors 
10:08 - by implementing interface in potential error fixes my error got solved.
10:10 - modifiedn the code to create the constructors and depedency injection
10:11 - copied the Repository.cs file from assignment2 folder in blackboard
10:12 - created the class CategoryRepository.cs in  Repository
10:13 - created the interface ICategoryRepository in IRepository
10:15 - modified the CategoryRepository.cs
10:30 - modified the CategoryRepository.cs
10:32 - got some error but fixed it by using statement
10:33 - pushed all the changes to github
11:00 - added the new interface in IRepository folder named ISP_Call.cs
11:02 - included the code and installed the Dapper NuGet package
10:03 - got some errors but solved it using potential error fixes
10:10 - Added new class to Repository folder named SP_call
10:13 - modified the SP_call
11:05 - got some errors


15\11\2021

deleted and recreated github repo modified 
12:02 - 

