# LiveProjectC-Sharp

This file contains Screenshots of every section of code I worked on during the C# Live Project that I worked organized by The Tech Academy.

About The Program:
https://hollywoodtheatre.org/
Software designed for a theater company to manage its website content without needing any technical knowledge. 
It will have multiple areas to manage admin needs, subscriber needs, and general public needs. 
The site will include information on the current season, past productions, the current cast members.
It will allow the acting company to easily upload content. It will allow subscribers to easily manage their subscriptions.

Some Project's I was Responsible for and the Requirements:
1. SignIn (Just had to pull origin/master, create a branch, and check out a story, then the find SignIn sheet, write our name down and commit/push to Azure)

2. Create Model For Productions (Properties should include Title, Description, StartDate (the day on the calendar when the production begins), EndDate (the final day of the production run), RunTime, Status (this property will be an enum with three items. Past, Current, and Upcoming), and a primary key.) 
![ProductionModel(CMS_B1)](https://user-images.githubusercontent.com/62126116/97636171-eedbdb80-19f5-11eb-90cc-9cf03481c0a7.PNG)
![Configuration(CMS_B1)](https://user-images.githubusercontent.com/62126116/97636883-f94aa500-19f6-11eb-861b-38bbad406939.PNG)
![IdentityModels(CMS_B1)](https://user-images.githubusercontent.com/62126116/97636890-fcde2c00-19f6-11eb-8f23-2dc97eb0e175.PNG)

3.Replace IsCurrentProperty (Create a method in the Production model called IsCurrentlyShowing that returns a bool.  The method should return true if the current date is between the opening and closing dates of the Production and should return false otherwise.  Once the method is created, find all instances of IsCurrent and replace them with the method calls to IsCurrentlyShowing.  In the startup file, you can remove the IsCurrent properties from the productions.) 
![CreateViewPageIsCurrentProperty](https://user-images.githubusercontent.com/62126116/97636341-36fafe00-19f6-11eb-94e8-5785f07dfc5d.PNG)
![DetailsViewPageIdCurrentProperty](https://user-images.githubusercontent.com/62126116/97636351-395d5800-19f6-11eb-9dc2-a968393ba7e6.PNG)
![EditViewPageIsCurrentProperty](https://user-images.githubusercontent.com/62126116/97636359-3ebaa280-19f6-11eb-8eb7-e9a702c80ac7.PNG)
![IndexViewPageIsCurrentProperty](https://user-images.githubusercontent.com/62126116/97636399-4da15500-19f6-11eb-86ed-b5f666bb83b7.PNG)
![HomeControllerIsCurrentProperty1](https://user-images.githubusercontent.com/62126116/97636365-40846600-19f6-11eb-91e5-6bf4dd45c434.PNG)
![HomeControllerIsCurrentProperty2](https://user-images.githubusercontent.com/62126116/97636372-437f5680-19f6-11eb-90d8-e0fc76057441.PNG)
![AdminControllerIsCurrentProperty](https://user-images.githubusercontent.com/62126116/97636634-a7098400-19f6-11eb-8fb0-38e493f4bb72.PNG)
![AdminControllerIsCurrentProperty1](https://user-images.githubusercontent.com/62126116/97636640-a83ab100-19f6-11eb-836d-98ab3ec6b45b.PNG)
![ProductionControllerIsCurrentProperty1](https://user-images.githubusercontent.com/62126116/97636428-55f99000-19f6-11eb-9d9e-732f14d8f3d8.PNG)
![ProductionControllerIsCurrentProperty2](https://user-images.githubusercontent.com/62126116/97636431-58f48080-19f6-11eb-9292-e8eb5e06e132.PNG)
![ProductionCSIsCurrentProperty](https://user-images.githubusercontent.com/62126116/97636451-5f82f800-19f6-11eb-8bf9-c51643710e5e.PNG)
![StartUpCSIsCurrentProperty1](https://user-images.githubusercontent.com/62126116/97636460-63af1580-19f6-11eb-8180-24f66ac60036.PNG)
![StartUpCSIsCurrentProperty2](https://user-images.githubusercontent.com/62126116/97636468-6578d900-19f6-11eb-8a98-4026ac0a2c2f.PNG)
![StartUpCSIsCurrentProperty3](https://user-images.githubusercontent.com/62126116/97636474-67429c80-19f6-11eb-8710-a44ea592c5ed.PNG)
![StartUpCSIsCurrentProperty4](https://user-images.githubusercontent.com/62126116/97636478-6873c980-19f6-11eb-86b0-9ab3bcc7b2d4.PNG)
![StartUpCSIsCurrentProperty5](https://user-images.githubusercontent.com/62126116/97636484-6a3d8d00-19f6-11eb-8542-a71041db3b37.PNG)
![StartUpCSIsCurrentProperty6](https://user-images.githubusercontent.com/62126116/97636487-6b6eba00-19f6-11eb-821f-965f6b1a53ef.PNG)
![StartUpCSIsCurrentProperty7](https://user-images.githubusercontent.com/62126116/97636493-6dd11400-19f6-11eb-93fe-0060058e0fc8.PNG)
![StartUpCSIsCurrentProperty8](https://user-images.githubusercontent.com/62126116/97636498-70336e00-19f6-11eb-8625-70be0612eb91.PNG)

4.Bulk Add Fixes and Features (I had to fix the sizing of the bootstrap, I removed the checkbox function when the matinee or evening time was invalid. I removed the text Invalid Date that would pop up when a Invalid Matinee or Evening time on a production was called. I added a function that reset the form when the Production N/A was chosen as well as automatically to automatically fill the form when a production is called (in the dropdown)).
![CalenderBulkAddFunction](https://user-images.githubusercontent.com/62126116/97636683-b557a000-19f6-11eb-88f7-2769b73cc28a.PNG)
![CalenderBulkAddHtml1](https://user-images.githubusercontent.com/62126116/97636689-b8529080-19f6-11eb-9967-9c3f2c1d2668.PNG)
![CalenderBulkAddHtml2](https://user-images.githubusercontent.com/62126116/97636695-b983bd80-19f6-11eb-96fe-0824f8bcd011.PNG)

5. Create Production Event Model: (I had to create a model that would be in a one to many relation ship to the Productions model I made earlier during the two week sprint.)
![ProductionEventModel(CMS_B2)](https://user-images.githubusercontent.com/62126116/97636765-d4563200-19f6-11eb-8636-cdddaf48f932.PNG)
![IdentityModels(CMS_B2)](https://user-images.githubusercontent.com/62126116/97636928-0d8ea200-19f7-11eb-87fe-6255c7c91f90.PNG)

6. Sponsors Search Bar: (I added a function to the search bar that let the user only see the sponsor they were searching for and hiding all the others. I also removed the search button since the function is always being called as soon as you interact with the search bar, it can also reset the page and the search bar by simply clicking a light blue x that'd pop up next to what you had typed/searched. Removing the need to constantly refresh and reload the page.)
![SponsorSearchBarFunction](https://user-images.githubusercontent.com/62126116/97636860-f059d380-19f6-11eb-9c88-d12c62f70982.png)
![SponsorSearchBarIndexTable](https://user-images.githubusercontent.com/62126116/97636867-f2239700-19f6-11eb-9e7b-16b075e649ad.png)
![SponsorSearchBarModel](https://user-images.githubusercontent.com/62126116/97636874-f485f100-19f6-11eb-99ea-3142b445c6c8.png)
