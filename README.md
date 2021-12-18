# Mark-my-Words
Lecture 7 Exercise 3
#include<iostream>
using namespace std;
int main()
{
	int marks;  //declaring variable with appropriate datatype int
	cout << "Please enter your marks : " << endl; //asking the user to enter the marks
	cin >> marks;   //marks will be stored in variable
	if (marks >= 0 && marks <= 100)   /*using nested if else to check if the marks are in the range of 0 to 100. If yes it will grade the marks, if not it will display
	the the default statement*/
	{

		if (marks > 70 && marks <= 100)  //using else if statement to grade the marks of user
		{
			cout << "Grade A " << endl;
		}
		else if (marks >= 60 && marks <= 69)
		{
			cout << "Grade B " << endl;
		}
		else if (marks >= 50 && marks <= 59)
		{
			cout << "Grade C " << endl;
		}
		else if (marks > 40 && marks <= 49)
		{
			cout << "Grade D" << endl;
		}
		else if (marks <= 40)
		{
			cout << "Grade F " << endl;
		}
	}
	else
	{
		cout << "Please enter the marks within the range of (0-100)." << endl; //the given message will be displayed if userenters marks greater than 100
	}
	return 0;
}
