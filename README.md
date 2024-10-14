# Contact-Book-using-Python

This Python code is a Graphical User Interface (GUI) application for a Contact Management System. It uses the Tkinter library to create the GUI and SQLite3 to manage the database. Here's a detailed explanation of the code:

1.	**Importing Libraries:**
   
      •	tkinter: Used for creating the GUI.

      •	tkinter.ttk: Used for creating advanced Tkinter widgets.

      •	tkinter.messagebox: Used for displaying message boxes.

      •	sqlite3: Used for interacting with the SQLite database.

2.	**Database Function:**

      •	Database(): This function is responsible for creating the SQLite database and the "REGISTRATION" table if it doesn't already exist.

3.	**Display Form Function:**

      •	DisplayForm(): This function creates the main window of the application and sets up the GUI layout.
  	
      •	It creates several frames to organize the different components of the application, such as the top header, the left registration form, the left search form, and the middle area for displaying the records.

      •	The registration form includes fields for First Name, Last Name, Gender, Address, and Contact.

      •	The search form includes a search entry field and buttons for searching, viewing all records, resetting the form, deleting a record, and updating a record.

      •	The middle area displays the records in a Treeview widget, which is a table-like structure.

  	  •	The DisplayData() function is called to populate the Treeview with the initial data from the database.

4.	**Update Function:**

      •	Update(): This function is called when the "Update" button is clicked. It retrieves the selected record from the Treeview, updates the corresponding fields in the database, and refreshes the Treeview.

5.	**Register Function:**

      •	register(): This function is called when the "Submit" button is clicked. It retrieves the form data, inserts a new record into the database, and refreshes the Treeview.

6.	**Reset Function:**

      •	Reset(): This function is called when the "Reset" button is clicked. It clears the Treeview, resets the form fields, and clears the search text.

7.	**Delete Function:**

      •	Delete(): This function is called when the "Delete" button is clicked. It prompts the user for confirmation, deletes the selected record from the database, and refreshes the Treeview.

8.	**Search Function:**

      •	SearchRecord(): This function is called when the "Search" button is clicked. It retrieves the search text, clears the Treeview, and displays the records that match the search criteria.

9.	**Display Data Function:**

      •	DisplayData(): This function is responsible for populating the Treeview with all the records from the database.

10.	**Double-Click Event Handler:**

      •	OnDoubleClick(): This function is called when a record in the Treeview is double-clicked. It retrieves the selected record and sets the form fields accordingly.

11.	**Main Execution:**

      •	The DisplayForm() function is called to start the application, and the mainloop() function is called to run the Tkinter event loop.

Overall, this code provides a complete Contact Management System with a user-friendly GUI and the ability to perform CRUD (Create, Read, Update, Delete) operations on the contact records stored in a SQLite database.
