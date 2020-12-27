
### Write a program in C++ to ask the user to enter the temperature. It also asks if the temperature is
### in Celsius or Fahrenheit. If it is in Celsius then the program outputs the corresponding temperature
### in Fahrenheit, otherwise it converts to Celsius. Use appropriate formula F = C × 9/5 + 32.

```C++
#include <iostream>

using namespace std;

int main()
{
    int temp;
    char T_temp;
    float Celsius,Fahrenheit;
    cout<<"Enter the Tempertaure :";
    cin>>temp;
    cout<<"\nEnter the type of Temp Celsius=C OR Fahrenheit=F : ";
    cin>>T_temp;
    
    Fahrenheit = temp * (9.0/5.0) + 32;
    
    Celsius = (temp-32) * 5.0/9.0;
    
    switch(T_temp)
    {
    	case 'C':
    		cout<<"\n"<<temp <<" Celsius Tempertaure is equal to "<<Fahrenheit<< " Fahrenheit Tempertaure"<<endl;
    	break;
    	
    	case 'F':
    		cout<<"\n"<<temp <<" Fahrenheit Temperrtaure is equal to "<<Celsius<<" Celsius Tempertaure"<<endl;
    	break;
    	
    	default:
    		cout<<"Errer! chose given option :";
    	break;
	}
    
    return 0;
}
```
