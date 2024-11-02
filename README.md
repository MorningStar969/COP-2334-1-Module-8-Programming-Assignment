# COP-2334-1-Module-8-Programming-Assignment
This is a GitHub repository link for Programming Exercise of Module 8.

// This program is used to determine if the number from the user's charge account is valid or not.

// Include the header file.
#include <iostream>
using namespace std; // Using standard namespace.

// Declare the function prototypes.
int main() { // Start of the main function.
  int accountNumber; // Declare the variable to store the account number.
  int accountNumbers[] = {5658845, 4520125, 7895122, 8777541, 8451277, 1302850, 8080152, 4562555, 5552012, 5050552, 7825877, 1250255, 1005231, 6545231, 3852085, 7576651, 7881200, 4581002}; // Declare the array to store the account numbers.
  cout << "Enter a charge account number: "; // Prompt the user to enter the account number.
  cin >> accountNumber; // Read the account number from the user.
  bool found = false; // Declare a boolean variable to check if the account number is valid or not.
  for (int i = 0; i < 18; i++) { // Start of the for loop.
    if (accountNumber == accountNumbers[i]) { // Check if the account number is valid.
      found = true; // Set the found variable to true.
      break; // Break the loop.
    } 
  }
  if (found) { // Check if the account number is valid.
    cout << "The number is valid." << endl; // Display a message if the account number is valid.
  }
  else { // If the account number is not valid.
    cout << "The number is invalid." << endl; // Display a message if the account number is invalid.
  }
  return 0; // Return 0 to indicate successful termination.
}
