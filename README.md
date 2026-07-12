## Library-management-system

## About the Project
This Library Management System is a Python-based application developed to simplify the process of managing books in a library. The project allows users to add, update, search, issue, and return books while storing all the information in an SQLite database.
The main objective of this project is to reduce manual work and make library operations faster, more organized, and easier to manage.

## Features
- Add new books to the library
- View all available books
- Search books by title or author
- Update book information
- Delete books from the database
- Register students
- Issue books to students
- Return issued books
- Calculate overdue fines (optional)
- Store all records using SQLite

## Technologies Used
- Python 3
- SQLite
- Tkinter (for the graphical interface)
- Object-Oriented Programming (OOP)

## Project Structure
```
Library-Management-System/
│── main.py
│── database.py
│── books.py
│── students.py
│── issue_return.py
│── library.db
│── requirements.txt
│── README.md
│── screenshots/
```
## How to Run the Project
1. Clone this repository.
```bash
git clone https://github.com/yourusername/Library-Management-System.git
```
2. Open the project folder.
```bash
cd Library-Management-System
```
3. Install the required packages.
```bash
pip install -r requirements.txt
```
4. Run the application.
```bash
python main.py
```
##Code

Import tkinter as tk
students = []
def add_student():
    name = entry.get()
    if name:
        students.append(name)
        listbox.insert(END, name + " - Present")
        entry.delete(0, END)
def delete_student():
    selected = listbox.curselection()
    if selected:
        listbox.delete(selected)
        students.pop(selected[0])
def clear_attendance():
    listbox.delete(0, END)
    students.clear()
root = tk.Tk()
root.title("Attendance Management System")
root.geometry("600x600")
Label(root, text="Student Name").pack(pady=5)
entry = Entry(root, width=25)
entry.pack(pady=5)
Button(root, text="Add Student", command=add_student).pack(pady=5)
listbox = Listbox(root, width=40, height=10)
listbox.pack(pady=10)
Button(root, text="Delete Student", command=delete_student).pack(pady=5)
Button(root, text="Clear Attendance", command=clear_attendance).pack(pady=5)
root.mainloop()

## Screenshots
You can add screenshots of the application here.
- Home Page
- Add Book
- Search Book
- Issue Book
- Return Book
  
## Future Improvements
Some features that can be added in the future include:
- User login for Admin and Librarian
- Barcode or QR code support
- Email reminders for due dates
- Export reports to Excel or PDF
- Online book reservation
- Better dashboard with statistics

## What I Learned
While working on this project, I improved my understanding of:
- Python programming
- Database management using SQLite
- GUI development with Tkinter
- CRUD operations
- File organization and project structure
- Git and GitHub for version control

## Conclusion
This project helped me understand how a real-world library management system works. It also gave me hands-on experience in building a complete application using Python and a database. The project can be further enhanced by adding more advanced features and improving the user interface.

## Author
**Deepthisri Nimmagadda**
B.Tech Student

