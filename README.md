# Pierre's Sweet & Savory Treats

#### _3/27/2020_

#### _By Jonathan Carlos_

## **Description**

_This C# codebase will build a user-friendly MVC Web application, allowing Pierre - as an authenticated and authorized user - to market his sweet and savory treats to the public._

## **Behavior Driven Development**

| Behavior | Input | Output |
|----------|:-----:|--------|
| Pierre enters treat name. | "Cake" | newTreat.name == "Cake" |
| Pierre enters treat description. | "Three-layered" | newTreat.description == "Three-layered" |
| Pierre enters a flavor name to a treat. | "Chocolate" | newTreat.flavor.name == "Chocolate" |
| Pierre enters a flavor description to a treat. | "Originates from organic mexican dark chocolate" | newTreat.flavor.description == "Originates from organic mexican chocolate" |
| Pierre enters the same flavor description to a different treat. | "Originates from organic mexican dark chocolate" | newTreatTwo.flavor.description == "Originates from organic mexican chocolate" |
| Pierre is greeted with a welcome splash page. | localhost:5000/ | route == "/" |
| Pierre clicks on a link that sends him to a form where he can add a treat. | "click" | HttpPost ActionResult' == Create(Treat treat) |
| Pierre clicks on a treat name and it goes to a page that displays all of that treat's flavors. | "click" | ActionResult ==  Details() |
| Pierre clicks on a link that presents a form for a new flavor for a particular treat. | "click" | HttPost ActionResult == Create (Flavor flavor) |
| Pierre enters an email and a password to create/register an account | Email: "Pierre@Bakery.com" Password: **** | CRUD functionality becomes available for Treats and Flavors |


## **Minimum Viable Product (MVP)**

The MVP of this project is to allow Pierre to create an account, log in successfully, and be granted access to CRUD functionality that is only available to users who are logged in.

Stretch goals include:

* Add feature that creates separate roles for admins and logged-in users, allowing only admins to add, update, and delte.
* Add an order form that only logged-in users can access, with the ability to create, read, update, and delete their own order.

## **Setup/Installation**

*Installing .NET Core* 

1. Download the .NET Core SDK [Software Development Kit](https://dotnet.microsoft.com/download).
2. Open the .Net Core SDK file and install.
3. Confirm the installation was successful by runnning the `$ dotnet --version` command in your terminal (You should see something like this in the response: `2.2.105`).
4. Install the dotnet script REPL tool by running the `$ dotnet tool install -g dotnet-script` command in your terminal.
5. Restart your terminal to complete the installation.

*Installing MySQL | MacOS:*

1. Download the MySQL Community Server DMG File from [MySQL Community Server](https://dev.mysql.com/downloads/file/?id=484914)
2. You can exit the mysql program by entering `exit`.
3. Download the MySQL Workbench DMG File from [MySQL Workbench](https://dev.mysql.com/downloads/file/?id=484391). (Use the No thanks, just start my download link.)
4. Install MySQL Workbench to Applications folder.
5. Open MySQL Workbench and select the `Local instance 3306 server`. You will need to enter the password you set. (We used `epicodus`.) If it connects, you're all set.

*Installing MySQL | Windows 10:*

1. Download the MySQL Web Installer from [MySQL Downloads](https://dev.mysql.com/downloads/file/?id=484919) (Use the No thanks, just start my download link.).
2. Choose `Custom` setup type.
3. When prompted to `Select Products and Features`, make sure you select both `MySQL Server` (Under MySQL Servers), and `MySQL Workbench` (Under applications).
4. When you reach `Configuration`:
  * Set `High Availability` to `Standalone`. 
  * Defaults are OK under `Type and Networking`. 
  * Set `Authentication Method` to `Use Legacy Authenticationn Method`.
  * Lastly, set your password and complete the installation process.
5. You can exit the mysql program by entering `exit`
6. Add the MySQL environment variable to the System PATH. We must include MySQL in the System Environment Path Variable. This is its own multi-step process. Instructions here are for Windows 10:
  * Open the Control Panel and visit System > Advanced System Settings > Environment Variables...
  * Then select PATH..., click Edit..., then Add.
  * Add the exact location of your MySQL installation, and click OK. (This location is likely `C:\Program Files\MySQL\MySQL Server 8.0\bin`, but may differ depending on your specific installation.)
7. Open MySQL Workbench and select the `Local instance 3306` server (it may have a different name). You will need to enter the password you set (We used `epicodus`). If it connects, you're all set.

*Cloning this repository:*

1. Open your terminal.
2. Navigate to the desired directory in which you want to clone this repository.
3. Use the command `git clone https://github.com/jamestlalocPDX/PierresTreats.Solution` to clone this repository.
4. Open this repository from within your terminal and navigate to the project folder: `PierresTreats/`.
5. Run the command `dotnet restore`.
6. Run the command `dotnet build`.
7. If build is successful, run the command `dotnet ef migrations add Initial`. If build failed, make necessary updates and repeat steps 5-7.
8. Run the command `dotnet ef database update`.
9. Use `dotnet run` to generate a local server.
10. Copy and paste the generated `localhost:5000` onto your URL.

*Downloading this repository:*

1. On the top right of this page, click the "Clone or download" button.
2. Click on "Download ZIP."
3. Click the downloaded file to unzip and extract this repository to your desired directory.
4. Open this repository from within your terminal and navigate to the project folder: `PierresTreats/`.
5. Run the command `dotnet restore`.
6. Run the command `dotnet build`.
7. If build is successful, run the command `dotnet ef migrations add Initial`. If build failed, make necessary updates and repeat steps 5-7.
8. Run the command `dotnet ef database update`.
8. Use `dotnet run` to generate a local server.
10. Copy and paste the generated `localhost:5000` onto your URL.

## **Known Bugs**

There are no known bugs at this time.

## **Support and contact details**

If you have any questions, comments, or concerns, please feel free to contact the content creator at examplemail@company.net 

## **Technologies used**

* _Git 2.23.0_

* _C# language_

* _.NET Core 2.2.106_

* _dotnet script 0.50.1_

* _Visual Studio Code 1.43.1_

* _Model-View-Controller(MVC) framework_

* _MySQL 8.0.15_

* _MySQL Workbench 8.0.15_

* _Entity Framework Core 2.2.4_

* _Language-Integrated Query (LINQ)_

* _ASP.NET Razor_

* GitBash

## **License**

Copyright (c) 2020 **_Pierre's Sweet & Savory Treats_**

This software is licensed under the MIT license.