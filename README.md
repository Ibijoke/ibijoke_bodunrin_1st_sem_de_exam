## THIS IS MY ALTSCHOOL FIRST SEMESTER EXAM PROJECT

### **Project description:**
This task was designed to test my comprehension of Object Oriented Programming in Python. 

The first part involved creating a Class called Expense where I needed to first create the class and initialize it, then list all the attributes that each instance (object) of the class must possess. 
In tracking each expense, the object must have: <br>
A. a unique ID which is auto-generated using UUID4(),<br> 
B. an expenses title (what the money was spent on),<br>
C. cost of the item (amount),<br>
D. date and time of expense- this is also auto-generated using the datetime module. <br>

Two additional methods were required to be created- the update and to_dict methods. 
A. Update method (I presume) is to allow editing of an already existing expense, the time of the update was required to be recorded. <br>
B. The to_dict is to accept and return all the attributes details of each expense in a dictionary datatype with the attributes as the key and the expense details as the values.<br>

The second part was to create a database for storing all the expenses. This required creation of another class called ExpenseDB. This will act as a collection and storage point for all the details of each expense using a list datatype. 
I was tasked to create five different methods, asides the initialization method, in this class- <br>
A. add_expense: to add an expense to the database, <br>
B. remove_expense: to remove an expense using the unique identifier, <br>
C. get_expense_by_id: retrieves an expense by using the expense ID, <br>
D. get_expense_by_title: this can be used to retrieved expenses by title, <br>
E. to_dict: returns a list of dictionaries representing expenses.<br>

### **How to clone this project**
Open your terminal, change directory to the folder you want to clone the file to. Enter the git clone command followed by the url for the file (this can be gotten from the github page, navigate to the clone or download button and copy the url). This command will clone this project to your computer locally. 

### **How to run the code**<br>
A. Open the python file in your preferred IDE- VSCode, PyCharm etc<br>
B. To create sample expenses for the Expense class, create expense variables eg expense1 and pass two values- the title (which has to be a string datatype) and amount (float datatype) the print the expense.<br>
expense1 = Expense("Ice-cream and Popsicle", 25.0)<br>
print(expense1.to_dict())<br>
output will be {'id': '0ea4f904-c835-411c-92fa-d0d781e680e6', 'title': 'Ice-cream and Popsicle', 'amount': 25.0, 'created_at': '2023-12-24 18:10:37 UTC', 'updated_at': '2023-12-24 18:10:37 UTC'}<br>
C. To create expenses that will be stored into the ExpenseDB, create a DB that will store your input, create sample expenses, use the .add_expense method to add them to the DB. To check if all your expenses have been added use:
print("All expenses in the database:", expense_db.to_dict())
Other methods can be used as follows: .remove_expense: to remove an expense using the unique identifier, .get_expense_by_id: to retrieve an expense by using the expense ID, .get_expense_by_title: this can be used to retrieved expenses by title, .to_dict: to return a list of dictionaries representing expenses.
