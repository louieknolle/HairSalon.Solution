# Eau Cl-hair's Beauty Salon

#### By _**Louie Knolle**_

####_This is a web-based application to allow a beauty shop owner the ability to keep a log of employed stylists and their respective clients._

## Technologies Used

- _C#_
- _.NET 5_
- _ASP.NET Core MVC_
- _MySQL_
- _Entity Framework Core_
- _HTML_
- _CSS_

## Description

This application allows Claire of Eau Cl-hair's Beauty Salon to keep track of all employed stylists and link specific clients to one stylist.  It also keeps a record of their next appointment. The data is contained in an SQL database.

## Setup/Installation Requirements
* _Open the terminal on your computer_
* _If they do not currently exist in your system, install [C#](https://docs.microsoft.com/en-us/dotnet/csharp/) and [.NET]https://docs.microsoft.com/en-us/dotnet/). You can follow the instructions found in this [lesson](https://www.learnhowtoprogram.com/c-and-net-part-time-c-and-react-track/getting-started-with-c/installing-and-configuring-mysql)_
* _Clone this repository onto your computer by running this command in your terminal `https://github.com/louieknolle/HairSalon.Solution.git`_

* _Start the server on MySQL with this command `mysql -uroot -p[YOUR-PASSWORD-HERE]`_
* _Next open the MySQL Workbench application_
* _Choose the MySQL instance in the __MySQLConnections__ section._
* _Select the __Navigator>Administration__ tab and in this window select __Data Import/Resote__ and the Data Import Window will open._
* In the __Import Options__ section of the Data Import window, select __Import from Self-Contained File__.
* _Click the dots at the end of the __Import from Self-Contained__ file field (three dots for windows, two dots for Mac) and a pop up box will open. In the pop up box, navigate to the louieknolle.sql file in the root directory of the project (HairSalon.Solution/). Once correct file is selected, click open. The pop up box will close itself._
* _In the __Default Schema to be Imported To__ section of the Data Import window, there is a __Default Target Schema__ drop box. To the right of the drop box, select the __New__ button and a pop up box will appear. In the pop up box, name the schema (i.e the database structure) `louie_knolle`. Click __OK___.
* _Click __Start Import__ at the bottom right corner of the window (If on a Mac the __Start Import__ button will be in the same view. If on a Windows machine first change to the __Import Progress__ tab to access the __Start Import__ button)._
* _Once import is complete, navigate to the workbench's __Navigator>Schemas__ tab, right click within the Schemas window and select __Refresh All__; the new database will appear._ 
* _In your terminal, navigate to the production project directory with the command `$ cd HairSalon.Solution/HairSalon`_
* _In your terminal, create a file within the project in which to store your connection string for connecting the project to the database with the command `touch appsettings.json`_
* _In your text editor add the following code to the newly created appsettings.json file. *Note that uid and pwd may vary depending on your local MySql configurations._

```
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;database=louie_knolle;uid=root;pwd=[YOUR-PASSWORD-HERE];"
  }
}
```
* _Issue command `$dotnet restore` in the project folder to launch the developer environment and install required dependencies_
* _Next run the program with `$dotnet run` and _

## Known Bugs

_none_

## License

_MIT_

**Copyright (c) _July 2022_ _Louie Knolle_**
**Please contact me for any contribution or questions: [email](mailto:knollelw@gmail.com)**