# LiveProjectC-Sharp

This file contains Screenshots of every section of code I worked on during the C# Live Project that i worked organized by The Tech Academy.

About The Program:
Software designed for a theater company to manage its website content without needing any technical knowledge. 
It will have multiple areas to manage admin needs, subscriber needs, and general public needs. 
The site will include information on the current season, past productions, the current cast members.
It will allow the acting company to easily upload content. It will allow subscribers to easily manage their subscriptions.

Some Project's I was Responsible for and the Requirements:
1. SignIn (Just had to pull origin/master, create a branch, and check out a story, then the find SignIn sheet, write our name down and commit/push to Azure)
2. Create Model For Productions (Properties should include Title, Description, StartDate (the day on the calendar when the production begins), EndDate (the final day of the production run), RunTime, Status (this property will be an enum with three items. Past, Current, and Upcoming), and a primary key.)
3.Replace IsCurrentProperty (Create a method in the Production model called IsCurrentlyShowing that returns a bool.  The method should return true if the current date is between the opening and closing dates of the Production and should return false otherwise.  Once the method is created, find all instances of IsCurrent and replace them with the method calls to IsCurrentlyShowing.  In the startup file, you can remove the IsCurrent properties from the productions.)
4.Bulk Add Fixes and Features (I had to fix the sizing of the bootstrap, I removed the checkbox function when the matinee or evening time was invalid. I removed the text Invalid Date that would pop up when a Invalid Matinee or Evening time on a production was called. I added a function that reset the form when the Production N/A was chosen as well as automatically to automatically fill the form when a production is called (in the dropdown)).
5. Create Production Event Model: (I had to create a model that would be in a one to many relation ship to the Productions model I made earlier during the two week sprint.)
6. Sponsors Search Bar: (I added a function to the search bar that let the user only see the sponsor they were searching for and hiding all the others. I also removed the search button since the function is always being called as soon as you interact with the search bar, it can also reset the page and the search bar by simply clicking a light blue x that'd pop up next to what you had typed/searched. Removing the need to constantly refresh and reload the page.)
