# iTravel
Authors:
1. Daniel Yoshida (dtyoshid@csu.fullerton.edu)
2. Parth Sharma (parthsharma@csu.fullerton.edu)
3. Marco Gabriel (marcog10@csu.fullerton.edu)
4. Diego Barrales (diego.barrales@csu.fullerton.edu)

## Background and motivation
This project is aimed at solving a problem that comes with traveling and being able to find all of the necessary information without having to walk around the entire airport and asking someone for help in another country, if necessary. Our application is attempt to address how to make traveling simpler and stress-free without the constant need to be worried about a missed flight or being over-weighed on a luggage.

### Summary
This project is trying to create an application that can help travelers be stress-free, allow travelers to focus more on enjoying their traveling experience, rather than being stressed out over paperwork and passports, and allowing travelers to have all of their information in one application.

## Features
1. Location and Time to Departure Gate (Daniel Yoshida) - Allows the user to find their departing gate based on their location and gives the estimated time of arrival to their departing gate. This will display the estimated time and provide a map of the airport and where the gate is located after the security gate is passed.
2. Currency (Marco Gabriel) - Allows the user to calculate from their currency to the traveler’s desired destination currency.
3. Covid Requirements (Parth Sharma) - Allowing users to find the Covid-19 test resources at the airport before their flight. The reason behind adding this feature comes from a problem with making covid test appointments within the 3 day period before the international flight. Most airports have covid testings but finding those options is challenging.
4. Seating Map of Plane (Diego Barrales) - Allows the user to check the number of seats taken on their given flight. The user could input their flight number and the output would be a map of the airplane with boxes representing the seats taken/or available.
5. Number of Carry-On and Dimension of the Carry-On (Developer Name) - Allows the user to check the number of carry-on possible and the dimensions of the carry-on.
6. Flight Time (Developer Name) - Allows the user to input their flight number and the software will show how long the flight will take.
7. Number of Luggages and Overweight Cost (Developer Name) - Allows the user to check how many luggages they can carry before additional costs are required and the overweight cost.
8. Local Time of the Destination (Developer Name) - Allows the user to add the local time of the destination that they are traveling to.
9. Link Passport and Other Travel Documents (Developer Name) - Allows the user to add their passport and other information (visa, etc…).

## Progress
### Check-in 1
#### Daniel Yoshida:
For my code, I have created a single class that inherits the airline and airport library that we are creating. Also, I have an array that associates the flight number with the gate number, created an initializer, a function that finds the departing gate number, created an array of terminals that contains sample gate numbers, and a function that displays the departing terminal image. I had some issues at the beginning with how to set things up and as a group, we were trying to figure out how to create this project and we realized that using a library might help all of our group members with what we might need for this project. We originally had the idea of creating a database, but we ended up deciding on create a library because it might be too difficult to accomplish.

#### Todo list:
1. I hope to be able to use the library that our group creates so that I would be able to link the library to the code that I write. Also, I hope to be able to have written enough code so that I would have an idea of how to create the UI because I currently only have an idea for the back end of the user experience and not the front end of the user experience.

#### Marco Gabriel:
For my part of the code I created simple class that has properties that will be used later on but things can change and they wont be used. For the mean time they are a placeholder. The purpose of this class is to get information from real time data. Most importantly getting the rates of the currency from different countries. 

#### Todo list:
1. I am hoping that I am able to get the real time data to work and from their just build on to it. As well getting a user interface that the user can scroll selecting their preference of the type of conversion they would like to make.

#### Parth Sharma:
Describe the changes made to your code since the last check-in. List any issues you encountered while you were building your application and solutions if you already solved them. Document any design changes or modifications in the features of your project and provide the reasons behind the change. 

#### Todo list:
1. Describe what you plan to accomplish by the next code checkin. You can check the milestone list for reference.

#### Diego Barrales:
For this check-in, I created a struct call seatMap that only contained a String variable. I also worked a lot on the dummy library for my group to use as an example database. This dummy library is where I spend most of the time before check-in 1; It went through many iterations, of review and discussion about what functions.
#### Todo list:
1. Finish the dummy library AirportManger class and all related items. 
2. Brainstorm ideas on how to implement my feature. 

### Check-in 2:
#### Daniel Yoshida:
For my code, I was able to utilize the library that our group created to develop my feature. I had to restructure my entire code from the previous check in because I noticed that the previous idea would not work properly and that it would be very difficult for me to be able to develop more efficient code. I created several functions that would get the gate numbers and created a unit test to check to make sure that I am able to get the gate numbers from the library.  Also, I created 8 arrays that have the gate numbers associated with the terminal number and 8 functions that checks to see if the gate number is in the array of gate numbers associated with the terminal number. If the function return true, then the function will return the terminal number. Furthermore, I created 8 arrays that have the airline code associated with each terminal that they are departing and arriving from and created 8 functions that checks to see if the airline code is associated with a specific terminal that the airline is departing and arriving from. I am using the return value from the previously mentioned functions to check for the specific terminal. If the function return true, then the function will return a string statement of the terminal map at LAX. Lastly, I created unit tests for all of the functions that I have created and all of them are working. I had some issues with how to design the functions and how to write it because I wanted to be able to understand what I was trying to do. I also had some technical issues with my branches, being able to build my code, and even find code that I had not pushed yet. I was able to get this resolved during office hours and I currently do not have any issues in regards to building, testing, or finding my code.

#### Todo list:
1. I hope to be able to develop a more cleaner UI and being able to actually link the UI with the code that I have created to see if the code that I wrote and the UI would work. I currently have not linked the two, so I do not know if they will work.

#### Marco Gabriel:
For my part I was able to run a suitable interface but was sadly turned down because I was building it onto main. No harm done so instead I just created the code to get real time data. Using a website that helps you get real time data from the current currency rates. I also created another file that will handle the exchange rates getting the data from the website. The exchange rates is a dictionary that will hold the abbreviation of the country and the currency rates of the country. I also updated my currency file to have the code to get the website info and properties that will hold a string and a double. As well created unit tests that will hopefully run if not then I will update them later on.

#### Todo list:
1. I am hoping that I am able to connect everything together to run the code with the interface and will probably update it as we go. As of right now the interface is a maybe. I may change the design down the road to make it a little bit more usable. As well to update on the unit tests. 

#### Parth Sharma:
For my part, I started on structuring and designing my feature. Since the purpose of my function is to show the Covid test requirement and options based on traveler's origin and destination, I have to first find credible resources. Therefore, I had focused doing that from end this week.  

#### Todo list:
1. I want to implement or find a way to showcase the results. I might even be done for this feature by next week, so I want to see what more I could add to this feature.

#### Diego Barrales:
Firstly, my group and I completed the dummy library and all related items for it. In addition to this, I updated seatMap, based on some of my brainstorming. Some of the more important changes were creating serval different private functions and variables for my struct. First one is an enum, call PlaneType which has 2 cases, eDomestic/ eInternational. This will/is used to determine what plane size will we be dealing with. In addition, I decided to create an array of seats, which are strings only. With this I was thinking that maybe I use this array in the UI side of things, by iterating through it to display the seats. Finally created a few tests functions to make sure the correct size array was being made and also created a storyboard reference a placeholder design. 
#### Todo list:
1. Work on the UI side of things more. Specifically get the user input to work. 
2. Figure out how to make a drop-down menu/pop up menu since it doesn't work right now. 
3. Potentially change seatList from an array of strings to an array of Seats, meaning create a Seat class or struct. My idea for this is that the Seat class or struct could contain a ton of boolean value to determine what type of seat I should display. For example, var isEconomy: Bool = true, would mean that this seat instance is a Economy(basic ticket) verse var isFirstClass = true. 

### Check-in 3
#### Daniel Yoshida:
For this check-in, I originally created a pickerView that I learned from Marco, but I noticed that looking through 156 different flight numbers would not be fun. So, what I did is I created two search bars, one for the airline names and one for the flight numbers. I was able to create it using UITableViewControllers and I was also able to create a navigation controller, so that the UI looks nice. Creating a cleaner UI was one of my objectives for this check-in and I think I have done a good job of it, but I would like to make improvements to it to make it more easier for the user to use. I had a tough time with the search bar because I didn't know how I was going to link the data and being able to move to the next view controller. I was able to do it by creating a button that will allow the screen to move to the next screen. I did not make any changes to my unit tests because I primarily wanted the user interface to work and figuring out how to improve my algorithm to search for the terminal map. Also, I was able to display the airline name data and the flight number data that I got from the library, but I still need to find a way to display the correct terminal map associated with the gate number. We still are not 100% sure on how the data will be shared among our group members, but I think we will get to that point in the very near future.

#### Todo list:
1. I hope to be able to have an algorithm that will allow me to get the correct gate number so that I can display the correct terminal map.
2. I will try and attempt to be able to create the pinch gesture recognizer so that the user can zoom in or out of the terminal map.

#### Marco Gabriel:
For this check-in I managed to output the JSON file. Doing this I was able to get the code to work properly. As well connecting back to the controller viewer that displays the data. The interesting thing about it was the picker view because it made a nice ticking noise when the user scrolls through it. As well I added some code that will make the code run if it ever went offline. The issue I have now is getting it to work. I also created another file that will hold constant values. Meaning that these values will remain unchanged. Another issue I have is getting the unit test to work. That is a flaw that I am currently having. 

#### Todo list:
1. Try to make reasonable unit tests.
2. Have a better interface. 
3. Hoping to finish the offline version.

#### Parth Sharma:
For this my original plan was to finish my part, however, I am honestly behind and plan to work on it over the break.
#### Todo list:
1. Plan what I have to implement and communicate with group members if I need help.
2. Learn how to use HTML link or file in the swift playground and implement it. 

#### Diego Barrales:
For this check-in, I made a lot of changes. Following my own Todo list, I did work on the UI side of the project a lot, so much that I got the picker view to work thanks to Daniel's help. This picker view replaced my drop-down menu idea and works a lot better. For the third item, a seat class, I ended up changing it after realizing how inefficient it was going to be since I could not make a general seat map for a bunch of different type of planes. So I commented that out and got started on working on an airplane database, where I created a plane struct and plane manager to do determine what plane is being used based on the distance between 2 airports, and what airline the user is flying with. Finally made unit tests to ensure that everything I implemented works as intended. 

#### Todo list:
1. Continue working on creating the image assets for all the different plane maps that exist. 
2. Work on a better UI design.
3. figure out a better way to pass information between view controllers, right now I set the navigation item's title to the name of the asset that is retrieved from .getSeatMap() which causes it shows on the title on the next page.

### Check-in 4
#### Daniel Yoshida:
For this check-in, I was able to complete the todo list that I wanted to do. I worked over spring break to get my feature to work using the algorithm that I created and being able to zoom in and out of the terminal map. I had some difficulty with the algorithm as well as linking all of the view controllers because I have three table view controllers and one normal view controller and I didn't know at the time of how to pass the data between the different view controllers. I was able to pass the data from one view controller to another view controller by passing the value using a variable and animating to the next view controller when it is true. I also created a pop up that rejects the user if they select an incorrect airline for a particular airport and a pop up that displays the estimated time of arrival to the gate number. Lastly, I added multiple unit tests to check for the various variables such as the gate numbers, the airport name, the airline name, the flight number, the estimated time of arrival to the gate number, and the terminal map.

#### Todo list:
1. I hope to be able to create a pop up menu that displays the user's recently searched terminal map.

#### Marco Gabriel:
The changed that I made is I got the offline part to work. I had an issue where my view controller turned everything dark and I couldn't seem to fix. So I decided to update Xcode and it finally updated after 3 days. As well I added an image to indicate that its a currency converter. I also added a button that will go to the offline version. Overall I am satisfied with what I have accomplished.

#### Todo list:
1. For next check in Im planning to add a pop error that will indicate the user is not connected to the internet or if the API is not working. This will change the user to go to the offline calculator. 

#### Developer 3 name:
Describe the changes made to your code since the last check-in. List any issues you encountered while you were building your application and solutions if you already solved them. Document any design changes or modifications in the features of your project and provide the reasons behind the change. 

#### Todo list:
1. Describe what you plan to accomplish by the next code checkin. You can check the milestone list for reference.

#### Diego Barrales:
I believe that I completed the to do list I created for last check-in. I made a better UI, and found a better way to pass information between view controllers. My UI consists of 4 UItextfields and 3 tableviews, that can open and close when clicked and information is entered. This make the UI look better than the picker view from last check-in since the user will be able to see the full string instead a partial string. The way I passed information between view controllers was using the tracker class that you showed us, call seatMapTracker. this allowed me to remove the navigation item title that I wanted not to show. 
#### Todo list:
1. Create the final assets
2. Work on the user interaction with the image more 
3. Hopefully Be able to merge my code to main.

### Check-in 5
#### Daniel Yoshida:
For check-in 5, I was able to finish creating my feature and merging it with the main project. Saving data and deciding where to save the data on the UI was the most difficult part of this check-in. Another issue that I had struggled with was figuring out how to change the navigation prompt and navigation title when the saved terminal map was pressed. Instead of creating a pop up menu that would display the user's recently searched terminal map, I created a plus button to add the searched terminal map and a magnifying glass button that would allow the user to find the saved terminal map. In the beginning, it would only change the saved terminal map, but not the description that was associated with it. I was able to resolve this issue by getting the saved data from the plist and using it to display the descriptions once the saved terminal map was pressed. I also finished adding the unit tests for this check-in as well. Lastly, Diego created a nice opening page for our app by using an API to rotate the images of various cities around the world. 

#### Todo list:
1. Preparing to present the app in class.

#### Marco Gabriel:
For this last check in I worked on saving data as well adding some more unit tests for the saving data. I struggled doing this because I had no idea how to save an api so I switched it to an array instead. Doing this it made it simpler. Even so I still struggled but with the help of my teammates I got it working. The next part was the unit test and unfortunately this part was difficult for me but got it working in the end.  The last thing that was added was detecting if the internet is connected. If the internet is connected it will return true and if it is not it will return false. When it's false it will change view controller and go to the back up arrays that have the values.  

#### Todo list:
1. Present the project and hope it don't crash.

#### Developer 3 name:
Describe the changes made to your code since the last check-in. List any issues you encountered while you were building your application and solutions if you already solved them. Document any design changes or modifications in the features of your project and provide the reasons behind the change. 

#### Todo list:
1. Describe what you plan to accomplish by the next code checkin. You can check the milestone list for reference.

#### Diego Barrales:
For check-in 5, I was able to work on two things, my feature and the main Home Screen. For my feature I was able to finish it and fix all of the bugs / unexpected errors I was given when running the app. For the home screen, I was able to create a tab view controller to switch between my team’s different storyboards. In addition, I added a feature to it that presents images retrieved from an api called teleport. I created code to animate this cycle. Finally, I was able to merge both features to main and replace the placeholder storyboard with my teams’ storyboard.

#### Todo list:
1. present our app!

*Design document template is based on [Chromium’s Design document template.](https://docs.google.com/document/d/14YBYKgk-uSfjfwpKFlp_omgUq5hwMVazy_M965s_1KA/edit)*
