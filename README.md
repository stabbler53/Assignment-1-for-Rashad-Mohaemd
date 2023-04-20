# Assignment: Simple Profile Page

Objective: Create a simple Flutter application that allows the user to enter their name, age, and upload a profile picture. The application should display the entered information on the same screen after the user presses a "Submit" button. Note that the code main.dart have been partially provided for you. Your job is too build the widget tree to create the following requirements.

Requirements:

1. Create a StatefulWidget called ProfilePage for the main screen of the application.
2. Inside the ProfilePage, use a Scaffold widget to create the basic layout structure.
3. Add an AppBar to the Scaffold with the title "Simple Profile Page".
In the Scaffold body, use a Column widget to align the input fields, button, and display widgets vertically.
4. Add a TextField widget for the user to input their name. Use a TextEditingController to capture the input value.
5. Add a second TextField widget for the user to input their age. Set the keyboardType to TextInputType.number and use another TextEditingController to capture the input value.
6. Add a button (e.g., ElevatedButton, FlatButton, or TextButton) to allow the user to upload a profile picture. When the button is pressed, use a package such as image_picker to open the device's image gallery and select an image. Store the selected image in the state.
7. Add a "Submit" button (e.g., ElevatedButton, FlatButton, or TextButton) below the input fields. When pressed, update the state to display the entered name, age, and profile picture below the button.
8. Use a Text widget to display the user's entered name and age.
9. Use an Image widget to display the selected profile picture. If no picture is selected, show a default placeholder image.

# Tips:

Use setState() to update the state of the ProfilePage whenever the user selects a profile picture or presses the "Submit" button.
Remember to dispose of the TextEditingControllers in the dispose() method of your ProfilePage StatefulWidget.
This assignment will help you gain experience with creating a simple user interface using Flutter, working with StatefulWidgets, handling user input, and displaying images.

If you are using ImagePicker, you may need to add the image_picker package to your pubspec.yaml file.

# Mohamed Amr Elsayed Rashad
# 2020355
#The code imports necessary libraries for the Flutter app, including 'dart:io' for file input/output operations, 'package:flutter/material.dart' for Flutter UI
components, and 'package:image_picker/image_picker.dart' for picking images from the device's gallery.
The app's entry point is the main() function, which calls the runApp() function with an instance of the MyApp class as its argument.
The MyApp class is a stateless widget that represents the root of the app. It returns a MaterialApp widget, which sets the app's title, theme, and home page to an
instance of the ProfilePage classThe ProfilePage class is a stateful widget that represents the profile page of the app. It contains various UI components, such as an
app bar, a column of widgets, and a form for submitting user's profile information.
The _ProfilePageState class is the state object associated with the ProfilePage widget. It manages the state for the profile page, including the user's name, age, and
profile image file.
The _pickImage() method is a private method that uses the ImagePicker plugin to open the device's gallery and allows the user to pick an image. The selected image file
is stored in the _image variable and triggers a UI update using the setState() method.
The _submitProfile() method is a private method that retrieves the user's name and age from the text input fields, and stores them in the _name and _age variables
respectively. It also triggers a UI update using the setState() method.
The _buildProfilePicture(), _buildNameTextField(), _buildAgeTextField(), and _buildSubmitButton() methods are private methods that define the UI components for the
profile picture, name text field, age text field, and submit button respectively. They use various Flutter UI components such as CircleAvatar, TextField, and
ElevatedButton to create the corresponding UI elements.
The _buildDisplayWidgets() method is a private method that defines the UI component for displaying the submitted profile information. It uses the _name and _age variables to conditionally display the user's name and age as text widgets.

Finally, the build() method of _ProfilePageState class returns a Scaffold widget that contains the various UI components created by the private methods, and defines the overall layout and structure of the profile page.


#It has beautiful interface and my name on it. 
