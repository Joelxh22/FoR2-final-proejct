Online Bank Management System

My project is a small online bank system, where a customer creates accounts and makes transactions based upon his own preferences. 
As soon as you run it you are given a window with 6 buttons, Create Account, Transfer, Withdraw, Deposit, Display record and exit. These buttons all run a specific method from the classes i have created which have the same name or similar name as the clicked button(except for the exit button). I will explain each button:
Create Account: calls the CreateAccount() method of the BankAccount class. It asks for user input for your name, account number, pin, account type balance and salary(only if you have specified that you want to create a checkings account). After all these inputs the method saves the information provided in a vector which I have used to save all the information provided by all users that create a new account.
Transfer: calls the Transfer() method which asks for four inputs, your account number, your pin, the recipient's account number, and the amount you want to transfer. After checking if the account numbers exist the program will make the transaction.
Withdraw: calls the WithdrawMoney() method which asks for user's account number and their pin in order to withdraw money from their account
Deposit: calls the DepositMoney() method which does the opposite of the WithdrawMoney() method
Display record: Calls the DisplayRecord function which asks for the user's account number and pin to display their entire account information
it must be made clear that to make sure that the entire application  runs properly, try catch statements have been implemented in almost every method of the child classes. These handle exceptions that might occurr during the running of the application such as the user might make writing errors etc.

Some technologies that I have used include:
Java Swing for GUI
I have used this so there is a better interaction between the user and the program using user friendly interface
JOptionPane 
I have used it for the user to input information and display to him messages regarding those inputs
Vector
I have used a vector to save the information that the user gives to the program when he wants to create an account and later use it to find the account number whenever the user wants to make transactions.
Abstract Class and methods
I have used them since they define common behavior and structure, while the account type is the one that makes the difference between each child class
java.awt.*,
java.awt.event.ActionEvent, and
java.awt.event.ActionListener,
i have used all of these to create and work on buttons and event handling in the main method's class. these imported libraries allow the application to respond to user input and trigger appropriate actions.


Challenges I faced was creating a method to save the transaction history which I unfortunately erased from my project. I could not find an answer anywhere on the internet and working on it for a while I gave up on it later on. Also a challenge for me was that I could not create a universal try catch statement and implement it on a method so i could use it for each type of variable, which later on I also gave up on. In the future I hope to implement a template type to work on a method and not matter the type of variable.


To install and run the project, we need to follow these steps:

Step 1: Compile the Java source files

Open a command prompt or terminal window.
Compile all the Java source files by executing the following command:
javac src/*.java

Step 2: Run the project

After successfully compiling the Java source files, you can run the project by executing the following command:
java BankAccountDemo

This command will execute the `main` method in the `BankAccountDemo` class and launch the application.

Step 3: Interact with the application

The application window will appear with its buttons for managing a bank account.
Click on the "Create Account" button to create a new bank account (checking or savings). Follow the prompts in the dialog box that appears.
Once an account is created, you can manage your account or to perform transactions like transferring money, withdrawing money, depositing money, displaying account records, or just exiting the application.

Using the project is very simple. After you compile and run the classes and after the application window appears you can: 

Create an account
Enter the account type (SAVINGS or CHECKINGS) when prompted.
Follow the subsequent prompts to input account details such as name, account number, PIN, initial balance, and additional information specific to the chosen account type (monthly salary for CheckingsAccount or none for SavingsAccount).

Perform different transactions
After creating an account, you can perform various transactions:
Transfer: Click the "Transfer" button and follow the prompts to transfer money between accounts.
Withdraw: Click the "Withdraw" button and follow the prompts to withdraw money from the account.
Deposit: Click the "Deposit" button and follow the prompts to deposit money into the account.

Display your account's information
Click the "Display Record" button to view information about the currently selected account, such as account type, name, account number, and balance.

Or just exit the application
Click the "Exit" button to close the application. You'll then be prompted to confirm the exit.

Credits: 
Stack Overflow
https://stackoverflow.com/questions/571026/java-gui-layout-problems
GitHub 
https://github.com/ssoad/BankingSystem/tree/master/bin/Bank
Geeks for Geeks
https://www.geeksforgeeks.org/java-util-vector-class-java/
