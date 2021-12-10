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
11:43- Corrected default reference @model ParitaBookStore.Models.ViewModels.ErrorViewModel
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
	"my migration folder name is :- 20211115021125_AddDefaultIdentityMigration"
9:20 - to update the database run the command - update-database
9:20 - successfully build 
9:21 - checked the updated table in SQL server object explorer
9:21 - run the project

run successfully.

9:25 - created the new class file in .Models project.
9:26 - modified the code.
9:30 - added the migration via console by command - add-migration AddCategoryToDb
	"my migration folder name is :- 20211115022846_AddCategoryToDb"
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
11:10 - push commits to github


15\11\2021

deleted and recreated github repo modified 
12:02 - commits all the changes and push it to the github
9:28 - Closed all the open tabs.
9:29 - Inside Areas/Admin/Controllers - added a new MVC empty controller named CategoryController.cs
9:34 - modifed the code of CategoryController.cs file4
00:25 - Created new folder named Category
00:25 - Added a view named Index into the Area/Admin/Views/Category.
00:30 - modified Index.cshtml file.
00:35 - modified the code of _Layout.cshtml file 
00: 36 - run the project.

And yehhhhhhh project run successfully with all the modified changes.

00:47 - in _layout.cshtml file, added code for the edit and delete icon
00:51 - Added new js file named category.js
00:53 - added code to the category.js file from the given file in assignment2 folder.

took a break

1:03 - In index.cshtml file added the @section for category.js script
1:06 - run the project.
1:06 - it ran successfully but is saying cannot find the database due to login error.

oh we are back 

5:43 - editing categorycontroller file to to activate edit and delete buttons.
5:43 - using upsert action, activate create new category button.
5:45 - added a view named Upsert
5:50 - modified the Upsert.cshtml view with the Category Upsert View.txt file from the assignment2 folder.
5:55 - created partial view for create.
5:56 - added the asp-action to the _CreateAndBackToListButton.cshtml file 
6:05 - created another partial view for the edit.
6:13 - modified the _EditAndBackToListButton.cshtml file with @model razor statement.
6:27 - modifed the Upsert.cshtml file
6:28 - added asp-action to the Index.cshtml file.

5:25 - created the new class file in .Models project.
5:26 - modified the code.
5:35 - modify the applicationDbContext.cs file
5:38 - re-run the command - add-migration AddCoverTypeToDb
5:40 - edited the migrated file 20211206153228_addCoverTypeToDb and checked the updated database 

and yeahhhh database is updated successfully......

6:00 - In ParitaBooks.DataAccess, created new folder name Repository
6:00 - In Repository folder, created new IRepository folder for interface
6:02 - In  IRepository folder, created the new interface and named it as  IRepository.cs
6:04 - Modified  IRepository.cs to perfoem CRUD operations.
6:06 - In Repository folder, created new class named  Repository.cs
6:06 - modified it but got some errors 
6:08 - by implementing interface in potential error fixes my error got solved.
6:10 - modifiedn the code to create the constructors and depedency injection
6:12 - created the class CoverTypeRepository.cs in  Repository
6:13 - created the interface ICoverTypeRepository in IRepository
6:15 - modified the CoverTypeRepository.cs
6:30 - modified the CoverTypeRepository.cs
6:32 - got some error but fixed it by using statement
6:33 - pushed all the changes to github

13:30 - create cover type repository
13:40 - Change in UnitofWork.cs 
13:55 - create migration and update database
13:10 - migration successfully created
13:25 - create controller and view for cover type
13:50 - Faced some errors and try to resolve it
14:10 - resolved errors and checked 

oh it ran successfully.
took a break

14:30 - create cover type Products
14:40 - Change in UnitofWork.cs 
14:56 - create migration and update database
15:20 -  migration successfully created
15:38 - create controller and view for cover type
15:45 - Faced some errors and try to resolve it
16:00 - resolved errors and checked




