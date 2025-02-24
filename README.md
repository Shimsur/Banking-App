# Banking-App

Welcome to the AwesomeGIC Bank Console Application. This is a simple banking system that handles account transactions, calculates interest based on defined rules, and allows users to print account statements.

Features
Transaction Input: Users can add deposits or withdrawals to a bank account.
Interest Rules: Users can define interest rates for specific periods.
Account Statement: Users can view account transactions and earned interest for a specific month.
Interest Calculation: The system calculates interest based on the end-of-day balances for each day of the month.
Requirements
.NET 8.0 or later.
A console terminal for interacting with the app.

Usage
Upon running the application, you'll be prompted to choose one of the following options:

[T] Input transactions: Enter transaction details (deposit or withdrawal).
[I] Define interest rules: Define interest rates for specific periods.
[P] Print statement: Generate an account statement for a specific month.
[Q] Quit: Exit the application.

Sample Input
Input Transactions

Enter transaction details (YYYYMMDD Account Type Amount): 
20230626 AC001 W 100.00
Define Interest Rule

Enter interest rule details (YYYYMMDD RuleId Rate): 
20230615 RULE03 2.20
Print Statement

Enter account and month (Account YYYYMM): 
AC001 202306
Interest Calculation
Interest is calculated based on the end-of-day balance for each day within the month. Interest is credited to the account on the last day of the month.

Example:

For AC001, for June 2023, with the following transactions:

Deposit of 150 on 20230601
Withdrawal of 20 on 20230626
Withdrawal of 100 on 20230626
If the interest rate is defined as 2.20% for the month, the system calculates the interest and credits it to the account on 20230630.



Testing
I have implemented unit tests for various parts of the application, including transaction handling and interest calculations.

Running Tests
To run the tests using the .NET CLI:

dotnet test

Test Coverage
Transaction Tests: Tests for valid transactions, including deposits and withdrawals.
BankService Tests: Tests for adding transactions, defining interest rules, and calculating interest.

Thank You
