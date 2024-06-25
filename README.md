Payroll Application

Description
The Payroll Application is a Java-based program designed to compute and display detailed payroll information for employees. It supports multiple languages, specifically English and Hindi, providing a user-friendly interface for input and output. The application formats dates and currency according to the selected locale, ensuring that all displayed information is relevant to the user's region. The program calculates various components of the salary, including allowances, deductions, gross salary, and net salary, and properly formats the employee's name.

Key Features
Locale Support: Users can choose between English and Hindi for input prompts and output messages, ensuring accessibility for a wider audience.
Proper Case Conversion: Employee names are converted to proper case (e.g., "john doe" to "John Doe") to maintain a professional and consistent format.
Currency Formatting: All monetary values are formatted according to the selected locale, enhancing readability and relevance.
Date Formatting: The current date is displayed in a format appropriate to the chosen locale, providing contextual information.
Comprehensive Payroll Calculation: The application calculates House Rent Allowance (HRA), Travel Allowance (TA), Medical Allowance (MA), Dearness Allowance (DA), Provident Fund (PF), gross salary, applicable tax, and net salary based on the employee's basic salary.
Tax Computation: Taxes are computed based on predefined annual salary slabs, ensuring accurate deductions.
Detailed Explanation of Code
Imports and Class Declaration: The program begins by importing necessary packages for formatting, locale support, date handling, and user input. The PayrollApplication class contains all the methods and logic for the payroll system.
Static Variables:
rb (ResourceBundle): Used for fetching localized messages.
locale (Locale): Represents the selected locale for language-specific formatting.
loadBundle Method: Loads the appropriate resource bundle based on the selected locale, allowing the application to display messages in the correct language.
properCase Method: Converts a name to proper case by capitalizing the first letter of each word, ensuring names are displayed professionally.
currencyFormat Method: Formats a double value into a currency string based on the locale, ensuring monetary values are displayed correctly for the user's region.
dateFormat Method: Gets the current date formatted as a string based on the locale, providing context-specific information.
input Method: Handles user input for language selection and employee details. It prompts the user for the employee ID, name, and basic salary, and calls the compute method to process payroll details.
compute Method: Computes various payroll components like HRA, TA, MA, DA, PF, gross salary, tax, and net salary. Calls the print method to display the payroll details.
computeTax Method: Computes the tax based on annual gross salary using predefined tax slabs, ensuring accurate deductions.
print Method: Prints the payroll details, including allowances, deductions, gross salary, and net salary, in a formatted manner.
Main Method: The entry point of the application that calls the input method to start the process.

