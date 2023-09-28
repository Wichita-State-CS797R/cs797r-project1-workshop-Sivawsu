[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/2sgFLH94)

Clone the project from the repositiry: https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-Sivawsu.git to the local machine.


Part1 - Displaying Data 

Added basic MonkeyFinder project along with all empty xaml page files into the git local repository.

The part Part-0 is showing the basic overview of .NET MAUI and projetc folder structure. Also explained how to set basic propeties of application like images, logo, icons..etc. Explained about CreateMauiApp method which is a static MauiProgram class that creates and return a MauiApp. This is entry point of the application. This MauiProgam class is must to run an app.
	
After Successfull run of Part0 basic code with all basic folders on VS code editor using Emulator, The app shown like this below.



In the Part1:

- In the Monkey Class, defined the features of monkey like Name, Location, Details, Image, Population, Latitute, Longitute
- Additionally, Using System.Text.Json to deserialize the data, we will want to add a MonkeyContext that will dynamically generate code for better performance.					# Internal sealed partial class MonkeyContext : JsonSerializerContext
- For displayong the list of Monkeys in a collected manner, The MainPage.xml has been updated here.
- Executed the code on Emulator and below is the run snap of app
 ${Part1-Run.png}

In the Part2:

- Introduced the full data binding with MVVM(Model-View-ViewModel) and retriving the monkeys from an internet data source.
	# INotifyPropertyChanged is important for data binding in MVVM Frameworks 
- For Implementing Title, IsBusy, IsNotBusy Given detailed code. Later given about how the CommunityToolkit.Mvvm library replaces the all above methods.
- Created the Monkey Service and implemented monkeylist in MonkeyService.cs. Added the imgaes link from web.
- Next step, Need to call the Monkey Service from ViewModel.
	# Updated the MonkeysViewModel to call our new monkey service and expose the list of monkeys to our user interface. 
	# Used "ObservableCollection<Monkey>" that will be cleared and then loaded with Monkey objects
- Before Running the app, update the register with all dependecies.
- Next, Builded the Monkeys User Interface and updated the View/MainPage.xaml
- Executed the Part2 code on Emulator and below is the run snap of app
 ${Part2-1-Run.png}   ${Part2-2-Run.png}   ${Part2-2-Run.png}





