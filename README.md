# Subgenre Analyzer
An artificial intelligence project to determine the subgenre of a song given a genre.

This is the GUI version of the project using Qt. To view the command line version, view the [CMD](https://github.com/ChrisTheEngineer/Subgenre_Analyzer/tree/CMD) branch.

libZPlay library - used for FFT audio analysis

#Project Description
Project originally created using Qt Creator 3.4.1 based on Qt 5.4.2 on Windows 8.1

**Initial Program:**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="/Documents/Images/Initial Program.PNG?raw=true" alt="Initial Program">

The user can select a genre from the avaliable [genres](/Subgenre_Analyzer/Genre_Finder_GUI/Genres). Additonally, the user can load audio from their computer. The 'Load Audio' button will open a prompt to select a song. The user must load audio, select a genre, and click the 'Update Genre Directory' before they can select the 'Analyze' button.

**Analyze Audio:**

<img src="/Documents/Images/Analyze Audio.PNG?raw=true" alt="Analyze Audio">

Once the user selects 'Analyze', the audio's information will be displayed in a seperate window. This includes the name, song length, peak tempo, autocorrection tempo, and the subgenre the program predicted. The predicted subgenre is determined using clustering. There is a visual representation of the feature vector, which shows all previous analyzed songs and the tempo ranges of each subgenre.

**Editing and Zoom:**

<img src="/Documents/Images/Edit and Zoom.png?raw=true" alt="Edit and Zoom">

The user can edit all parts of the song data excluding the song length by double clicking on the value of any piece of information. Additionally the user can zoom in and out of the visual feature vector. When the user is zoomed in, the image can be moved around.

**Adding Genres:**

To add a new genre, the user should create a text file in the [Genres](/Genre_Finder_GUI/Genres) folder. The file name should be the name of the genre. Below is an example of how each subgenre should be written (excluding the brackets):
```
[Subgenre name], [minimum tempo], [maximum tempo]
```

Files containing a more in-depth description and details of the project are located in the [Documents](/Documents) section. These documents correspond to the command line version of the project; however, are very similar in concept and should apply to this version.
