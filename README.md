# Lab-23.10-
#include <iostream>
using namespace std;

int main() {
  const int MAX_SIZE = 100;
  int grades[MAX_SIZE];// this is for the higest a grade can be.
  
  int numberOfGrades; // the number of grades read.
  
  cout << "Please input the number of grades to be read:\n";
  cin >> numberOfGrades; // the number of grades the user will input
  cout << "Please input grades from 1 to 100\n";
  for (int i = 0; i < numberOfGrades; i++)// this is for how many grades the user wants to input
  {
    cin >> grades[i];
  
  }
  int i, max, min;
  max = grades[0];
  min = grades[0];
  int sum = 0;
  cout << endl;
  for (int i = 0; i < numberOfGrades; i++) // this is for how many grades were entered are each labeled element 1, 2 etc.
  if (grades[i] > max) 
  max  = grades[i];
  if (grades[i] < min)
   min = grades[i];
  {
    cout << "Element " << i+1 << " is " << grades[i] << endl; // grades is for the grades the user entered 
    sum = sum + grades[i]; // total of the grades that the user inputed 
  
  
  }
  double average = sum/numberOfGrades;
  cout << "The average of the elements is " << average << endl;
  cout << "The sum of the " << numberOfGrades << " numbers is " << sum << endl;
  cout << "The lowest element is " << min << endl;
  cout << "The highest element is " << max << endl;
}
// this array is called a partcially filled array because it is unknown to how much data it will be holding. It all depends on what the user inputs.
