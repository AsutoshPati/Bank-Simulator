# Bank Simulator
----------------

This project simulates workflow of a bank. Where some functionalities like creating account,
deposit money, withdrwal money, transfer money and displaying transactions.

How to use
----------
As the code is made with python and written in jupyter notebook so it is possible to directly run 
the code and check the output over there.


As this program is written with concepts of OOPs. So first of all you have to create an object of 
bank class.<br>
<kbd>b = Bank()</kbd><br>

Then you can start using the functionalities with the created object.

Creating Account
-------------------
You can create 2 type of accounts.
1. Operator        - only operator can do the deposit process and all other functionalities
2. Account Holder  - all functionalities except deposit can be done
<br>
For creating account you have to call the method from the created object <br>
<kbd>b.register_user()</kbd> which will create an account holder's account<br>
for creating operator account just pass 'O' <kbd>b.register_user('O')</kbd><br>
<br>
Here you can select 3 different type of accounts like
1. Current (C) - By selecting current account 500 rupees will be credited in account.
2. Savings (S) - By selecting savings account 2000 rupees will be credited in account.
3. Loan (L)    - By selecting loan account you will be asked to enter the value of amount. And that much will be credited.
4. Quit registration (Q) - To quit from the registration process you can use Q.
<br>
It will ask for some other details you can provide them or you can use Q as input to quit the ongoing registration process.<br>
<br>
After completing the process account number will be generated. Remember the account number and 
the given password for further transactions.

Log in
-------------------
You can login with your phone number and password which was provided during the time of registration 
and the functionalities will be available only if any user has been logged in at the time. <br>
login method can be used for logging into account which can be called using the same bank object 
created before. <kbd>b.login()</kbd>

Log out
-------------------
After completing the job for which you have logged in; you can log out of the account using logout 
method which can be called using the same bank object created before <kbd>b.logout()</kbd>.

Changing the Password
---------------------
For changing the password you can call for the change_password method <kbd>b.change_password()</kbd> 
here you will be asked for the current password and the new password.

Deposit
--------
*Note: Only operators can deposit into an account
For making a deposit you can call the deposit function <kbd>b.deposit()</kbd>; where the operator 
will be asked to enter the account number of payer's and the amount to be deposited.

Withdrawl
----------
For doing an withdrawl process you will be asked to enter amount you want to withdraw; to use this 
function you have to call withdrawl method <kbd>b.withdrawl()</kbd>.

Money Transfer
--------------
For completing money transfer process you have to call the moneyTransfer method 
<kbd>b.moneyTransfer()</kbd>. Where you will be asked to enter the payee's account number and the 
amount you want to transfer.

Display Transaction Report
--------------------------
To see your transaction details you can call the method my_transactions 
<kbd>b.my_transactions()</kbd>; where you will be asked for some filter options like
1. All               - show all transactions till now
2. By year           - show transactions made in a specific year
3. By year and month - show transactions made in a specific year and specific month
4. Cancel            - cancel the process

Display Info
--------------------------
If you ever wanted to see account info that can displayed using the method my_details 
<kbd>b.my_details()</kbd>.