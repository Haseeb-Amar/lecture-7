# lecture-7


Earthquake
#include<iostream>
using namespace std;
int main()
{
	double mag;
	cout << "please enter the mangitude of the earthquake in numbers 0 input is not accepted : ";
	cin >> mag;

	

		if (mag < 2.0 && mag >0) {
			cout << " earthquake is considered to be a micro earthquake.";
		}
		else if (mag >= 2.0 && mag < 3)
		{
			cout << mag << " earthquake is considered to be a very minor earthquake.";
		}
		else if (mag >= 3.0 && mag < 4)
		{
			cout << mag << " earthquake is considered to be a minor earthquake.";
		}
		else if (mag >= 4.0 && mag < 5.0)
		{
			cout << mag << " earthquake is considered to be a light earthquake.";
		}
		else if (mag >= 5.0 && mag < 6.0)
		{
			cout << mag << " earthquake is considered to be a moderate earthquake." << endl;
		}
		else if (mag >= 6.0 && mag < 7)
		{
			cout << mag << " earthquake is considered to be a strong earthquake." << endl;
		}
		else if (mag >= 7.0 && mag < 8)
		{
			cout << mag << " earthquake is considered to be a major earthquake." << endl;
		}
		else if (mag >= 8.0 && mag <= 10)
		{
			cout << mag << " earthquake is considered to be a great earthquake." << endl;
		}
		else if (mag > 10.0)
		{
			cout << mag << " earthquake is considered to be a meteoric earthquake." << endl;
		}
	
		else {
			cout << "You entered an invalid value" << endl;
		}
		return 0;
		}
  
  
  
  timekilling
  
  #include<iostream>
using namespace std;
int main()
{
	int t, m;
	cout << "Until what time your friend will come? (Enter the time in minutes)\n";
	cin >> t;
	if (t >= 15)
	{
		cout << "Your friend will take more or equal to 15 minutes to come,\n enter the money amount to see if you can drink something";
		cin >> m;
		if (m > 5)
		{
			cout << "You have more than 5 AED, now you will buy a drink and wait for him" << endl;
		}
		else
		{
			cout << "You don't have enough money,\n Let's just walk around";
		}
	}
	else
	{
		cout << "Your friend will be here within 15 minutes, \n so you're just going to wait for him." << endl;
	}
	return 0;
}
  
  
  Starting a Band
  #include<iostream>
#include<string>
using namespace std;
int main()
{
	bool musician;
	string reply;
	string instrument;
	cout << "Do you play any musical instrument? \n type 'y' for yes \n and 'n' for no \n ";
	cin >> reply;
	if (reply == "y" || reply == "Y")
	{
		musician = true;
		if (musician == true)
		{
			cout << "What kind of insturment you can play \n type d if you're a drummer \n type g if you're a guitarist\n type o for other\n" << endl;
			cin >> instrument;
			if (instrument == "g" || instrument == "G")
			{
				cout << "That's great! I really needed a guitarist." << endl;
			}
			else if (instrument == "d" || instrument == "D")
			{
				cout << "That's great! I really needed a drummer." << endl;
			}
			else if(instrument =="o" || instrument == "O")
			{
				cout << "Ah I see, actually I'm looking for guitarist or a drummer.\n Let me know if you someone who plays them\n Thank you :)" << endl;
			}
			else
			{
				cout << "Incorrect input" << endl;
			}

		}
	}
		else if (reply == "N" || reply == "n")
		{
			musician = false;
			cout << "Oh! so you don't know how to play any instrument\n it's alright, let me know if you know someone who does \n Thanks" << endl;
		}
		else
		{

			cout << "Incorrect input" << endl;
		}

	
		return 0;
	}
  
  
  Mark my words Grade
  #include <iostream>
using namespace std;

int main()
{
   cout << "Enter the marks from 1-100 to see the grade, 0 input is not accepted\n";
   double m;
   cin >> m;
   if (m>70)
   {
  cout << "You have a A Grade";
   }
   else if (m >= 60 && m < 70)
   {
  cout << "You have a B Grade";
   }
   else if (m >= 50 && m < 60)
   {
  cout << "You have a C Grade";
   }
   else if (m>40 && m<50)
   {
  cout << "You have a D Grade";
   }
   else if (m == 40 )
   {
  cout << "You have a JUST PASSED Grade";
   }
   else if(m<40 && m!=0)
   {
  cout << "You have a Fail Grade";
   }
   else 
   {
  cout << "Wrong input";
   }
}
  
  
  
  Letter checker Vowels Consonant
  #include <iostream>
using namespace std;

int main()
{
	cout << "Enter a letter to see whether its a vowel or consonant\n";
	char c;
	cin >> c;
	//isalpha is a built in function to check for alphabet values in c++
	if (!isalpha(c))
	{
		cout << "you entered an incorrect value";
	}
	else if (c == 'a' || c == 'e' || c == 'i' || c == 'o' || c == 'u' || c == 'A' || c == 'E' || c == 'I' || c == 'O' || c == 'U')
	{
		cout << "you entered a vowel";

	}


	else
	{
		cout << "you entered a consonant";
	}
}
  
  
  France
  #include <iostream>
using namespace std;
int main()
{
    cout << "What is the capital of France?\n";
    string capital;
    cin >> capital;
   
    if (capital == "Paris" || capital == "paris" || capital == "PARIS")
    {
        cout << "You enter the correct answer";
    }
    else 
    {
        cout << "Sorry wrong answer";
    }
    
    return 0;
}
  
  
  
  
  theme park
  #include <iostream>
using namespace std;
int main()
{
    cout << "Please enter your height in meters to check whether you can ride or not\n";
    double h, age;
    cin >> h;
    cout << "Please enter your age to check whether you can ride or not\n";
    cin >> age;
    if (age >= 5 && h >= 0.6)
    {
        cout << "You can ride";
    }
    else if (age < 5 && h < 0.5)
    {
        cout << "Sorry you cannot ride";
    }
    else
    {
        cout << "Incorrect input";
    }
    return 0;
}

