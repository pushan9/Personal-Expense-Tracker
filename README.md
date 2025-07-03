# Personal Expense Tracker 
Project Objectives 
• Enable users to record daily expenses with detailed metadata 
• Allow categorization of expenses and track them in a structured format 
• Provide functionality to set and monitor a monthly budget 
• Implement file handling for persistent storage using CSV 
• Provide a menu-driven interface for easy user interaction 

Core Features & Implementation 

1. Data Handling 
• Uses a global list (expenses) to store expense dictionaries 
• Each expense includes: date, category, amount, and description 
2. Expense Entry 
• The add_expense() function collects inputs from users and appends a validated expense 
record to the list 
• Input validation ensures the amount is a valid floating-point number 

3. Viewing Expenses 
• The view_expenses() function displays all stored entries in a readable format 
• Handles edge cases like no records or incomplete entries gracefully 

4. Budget Tracking 
• Users can set a monthly budget using set_budget() 
• track_budget() calculates total spending and compares it to the budget  
o If exceeded: warning is displayed 
o If within budget: remaining balance is shown


6. File Management
   
• Uses CSV format for saving/loading expenses via save_expenses() and load_expenses() 
• Automatically loads saved data on startup and persists it on exit

7. Interactive Menu 
• The display_menu() function creates a loop-driven menu 
• Users can select options for adding, viewing, budgeting, tracking, and exiting 

Technologies Used

• Python Standard Library: File I/O (csv), input/output handling 
• Data Structure: List of dictionaries 
• Console UI: Menu-driven logic using loops and conditionals 

Sample Run Snapshot 
=== Personal Expense Tracker Menu === 
1. Add Expense 
2. View Expenses 
3. Set Monthly Budget 
4. Track Budget 
5. Save and Exit 
Choose an option (1–5): 
