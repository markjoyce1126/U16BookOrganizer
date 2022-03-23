# U16BookOrganizer

## Bugs, missing features, poor implementation etc

### Bugs

- Button to create Temp folder does nothing
  - Intended use is to create a temp folder to output the .json file, even if the user doesn't have such a folder on their device
- The 'Output' and 'Go' buttons are effectively worthless; all work being done by the 'Input' button

### Missing Features

- No ability to remove the selected directory - the user will have to kill the program and start again

### Poor Implementation

- Usage of MessageBox.Show() is messy - it's a pop up dialogue that may frustrate users.
  - Would have been cleaner to utilize a method that would show on the XAML interface, rather than popping up randomly after a task has been completed.

## What is This?

The U16BookOrganizer is a XAML/C# program that takes a .csv file and outputs it to a .json file with an added cataloguing system in order to make the...well...the cataloguing of books easier. Its intended use is for a college library.

- Example (pre output):
  Orwell, George	England your England	London	Penguin	2017
- Example (post output):
  "Cat": "8583951a80",
    "Name": "Orwell, George",
    "Title": "England your England",
    "PublishedIn": "London",
    "Publisher": "Penguin",
    "Date": "2017"



