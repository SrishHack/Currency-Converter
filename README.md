Python Command-Line Currency Converter

Project Title

Simple Python Command-Line Currency Converter

Overview of the Project

This project is a simple, command-line application built purely in Python that allows a user to convert an amount from a source currency to a target currency. It is designed to be highly portable and run instantly in any standard Python environment without external dependencies (other than standard Python libraries).

The application uses a set of hardcoded mock exchange rates relative to the US Dollar (USD) as the base currency. It calculates the conversion amount and displays the direct exchange rate used for transparency.

Features

Instant Command-Line Conversion: Allows users to input an amount and specify the source and target currency codes interactively.

Input Validation: Ensures the entered amount is a positive number and verifies that the currency codes are supported by the system.

Dynamic Rate Calculation: Calculates the direct exchange rate between any two supported currencies based on their relationship to the base currency (USD).

Clear Output: Displays the converted amount and the precise exchange rate used in a clean, formatted manner.

Graceful Exit: Supports 'exit' or 'quit' commands to terminate the application.

Technologies/Tools Used

Category

Technology/Tool

Purpose

Language

Python 3.x

Core application logic and execution environment.

Libraries

sys, typing (Standard Library)

System interaction and type hinting for code clarity.

Data

Python Dictionary

Storing mock exchange rate data for conversion calculations.

Steps to Install & Run the Project

Prerequisite: Ensure you have Python 3.x installed on your system.

Save the File: Save the provided code as currency_converter.py.

Run the Script: Open your terminal or command prompt, navigate to the directory where you saved the file, and execute the following command:

python currency_converter.py


Interaction: The application will prompt you sequentially for:

The amount to convert.

The source currency code (e.g., USD).

The target currency code (e.g., EUR).

Exit: Type exit or quit at any prompt to close the program.

Instructions for Testing

Since the exchange rates are hardcoded, testing involves verifying the mathematical correctness of the conversion logic.

Positive Case (Known Conversion):

Test: Convert 10 USD to EUR.

Expected Result: Since the mock rate is 1 USD = 0.93 EUR, the result should be exactly 0.93 EUR.

Cross-Currency Conversion:

Test: Convert 10 GBP to CAD.

Expected Logic: Rate (GBP to CAD) = Rate (USD to CAD) / Rate (USD to GBP) = 1.37 / 0.81 ≈ 1.6914. Converted Amount ≈ 10 * 1.6914 ≈ 16.91 CAD.

Input Validation Test (Amount):

Test: Enter -50 or 0 for the amount.

Expected Result: The program should print "Amount must be a positive number." and ask for the amount again.

Input Validation Test (Currency Code):

Test: Enter XYZ for the currency code.

Expected Result: The program should print an error like "Error: Currency 'XYZ' not supported." and ask for the code again.

Exit Test:

Test: Type quit or exit when prompted for an input.

Expected Result: The program should terminate cleanly with a thank you message.
