[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/2sgFLH94)

Clone the project from the repositiry: https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu.git to the local machine.

**
Name: Sivaprasad Reddy Bogireddy, mywsuId: K966S589
Course: CS797R 		Term: Fall-2023    Instructor: Huabo Lu**

# Part0: Initial

	Added basic MonkeyFinder project along with all empty xaml page files into the git local repository.
The part Part-0 is showing the basic overview of .NET MAUI and projetc folder structure. Also explained how to set basic propeties of application like images, logo, icons..etc. Explained about CreateMauiApp method which is a static MauiProgram class that creates and return a MauiApp. This is entry point of the application. This MauiProgam class is must to run an app.
After Successfull run of Part0 basic code with all basic folders on VS code editor using Emulator, The app shown like this below.

 Part0: Execution:![Part0-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part0-Run.png)


# Part1: Displaying Data

- In the Monkey Class, defined the features of monkey like Name, Location, Details, Image, Population, Latitute, Longitute
- Additionally, Using System.Text.Json to deserialize the data, we will want to add a MonkeyContext that will dynamically generate code for better performance.				
	* Internal sealed partial class MonkeyContext : JsonSerializerContext
- For displayong the list of Monkeys in a collected manner, The MainPage.xml has been updated here.
- Executed the code on Emulator and below is the run snap of app
- Part1: Execution:  ![Part1-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part1-Run.png)


# Part2: MVVM

- Introduced the full data binding with MVVM(Model-View-ViewModel) and retriving the monkeys from an internet data source.
	"INotifyPropertyChanged is important for data binding in MVVM Frameworks" 
- For Implementing Title, IsBusy, IsNotBusy Given detailed code. Later given about how the CommunityToolkit.Mvvm library replaces the all above methods.
- Created the Monkey Service and implemented monkeylist in MonkeyService.cs. Added the imgaes link from web.
- Next step, Need to call the Monkey Service from ViewModel.		
  * Updated the MonkeysViewModel to call our new monkey service and expose the list of monkeys to our user interface."
	* Used "ObservableCollection<Monkey>" that will be cleared and then loaded with Monkey objects
- Before Running the app, update the register with all dependecies.
- Next, Builded the Monkeys User Interface and updated the View/MainPage.xaml
- Executed the Part2 code on Emulator and below is the run snap of app
- Part2: Execution1: ![Part2-1-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part2-1-Run.png)
- Part2: Execution2:![Part2-2-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part2-2-Run.png)
- Part2: Execution3:  ![Part2-3-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part2-3-Run.png)
 

# Part3: Navigation

- In this part, they just added navigation to push a new page onto the stack to display details about the monkey.
- Used the built-in Shell navigation of .Net MAUI. This is powerful navigation system based on the URLs. It allows to pass any additional information while navigating query parameter such as string or object
- Expanded ViewModel for Details of each monkey on to the newly created DetailsPage.xaml UI
- Executed the Part3 code on Emulator and below is the run snap of app
- Part3: Execution1: ![Part3-1-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part3-1-Run.png))
- Part3: Execution2:![Part3-2-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part3-2-Run.png))
- Part3: Execution3: ![Part3-3-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part3-3-Run.png)

# Part4: Platform Features

- In this part, they tried to access the plotform features. By using .NET MAUI to find the closest monkey to us and also open a map with the Monkey location
- In the First step, they explained how to check if a device is connected to internet or not by simply using built in IConnectivity of .NET MAUI
	 * IConnectivity connectivity;
- Later steps, they added more functionalities to this application using the GPS of the device.
	* get access to the IGeolocator found inside of .NET MAUI
- In the steps, Implemented the opening default map application with built in .NET MAUI API
- Update the Monkey detailspage.xaml UI for adding option to map.
- Executed the Part4 code on Emulator and below is the run snap of app		
- Part4: Execution1:  ![Part4-1-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part4-1-Run.png))
- Part4: Execution2: ![Part4-2-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part4-2-Run.png))
- Part4: Execution3: ![Part4-3-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part4-3-Run.png))
- Part4: Execution4: ![Part4-4-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part4-4-Run.png)

# Part5: CollectionView

- Added Pull-to-Refresh feature to the application by using .NET MAUI ListView
- Played around the different Layout like LinearItemsLayout, GridItemsLayout and EmptyView.
- Changed the xaml code in MainPage.xaml as per different layouts.
- Below are the run-time screenshots.
- Part5: Execution1: ![Part5-1-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part5-1-Run.png))
- Part5: Execution2:![Part5-2-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part5-2-Run.png))
- Part5: Execution3:![Part5-3-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part5-3-Run.png))
- Part5: Execution4:![Part5-4-Run](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu/blob/main/Images/Part5-4-Run.png))

# Part6: AppThemes

- In this part, they shown how to change the background theme Light/Dark.
- Updated all the Resources in the App.xml.


