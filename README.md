```
作業
```
4/10
```
#include <iostream>
using namespace std;

int main()
{
  const int NUMBER_OF_ELEMENTS = 5;
  double numbers[NUMBER_OF_ELEMENTS];
  double numbers_squared[NUMBER_OF_ELEMENTS];
  double sum = 0;

  for (int i = 0; i < NUMBER_OF_ELEMENTS; i++)
  {
    cout << "輸入整數: ";
    cin >> numbers[i];
    sum += numbers[i];
    numbers_squared[i]=numbers[i]*numbers[i];
  }
  cout << "numbers[1] is " << numbers[1] << endl;
  cout << "numbers_squared[1] is " << numbers_squared[1] << endl;
  
  double average = sum / NUMBER_OF_ELEMENTS;

  int count = 0; // The number of elements above average
  for (int i = 0; i < NUMBER_OF_ELEMENTS; i++)
    if (numbers[i] > average)
      count++;

  cout << "平均: " << average << endl;
  cout << "超過平均的數字: " << count << endl;
  system("pause"); 
  return 0;
}
```

![result]()

4/17

4/24
```
#include <iostream> 
#define PI 3.14 

using namespace std; 
class Circle 
{ 
private: 
double mRadius; 
public: 
Circle():mRadius(1) 
{} 
~Circle(){} 
void setRadius(double rad) 
{ 
mRadius=rad;  
} 
void getRadius() 
{ 
cout<<"半徑="<<mRadius<<"\n";
} 
void getPerimeter() 
{ 
cout<<"體積="<<4/3*PI*mRadius*mRadius*mRadius<<"\n";
} 
void getArea() 
{ 
cout<<"面積="<<PI*mRadius*mRadius<<"\n";
} 
}; 

int main() 
{ 
int radius; 
Circle cir; 
cout<<"半徑:"; 
cin>>radius; 
cout<<"\n"; 
cir.setRadius(radius); 
cir.getRadius(); 
cir.getPerimeter(); 
cir.getArea(); 

system("pause"); 
return 0; 

} 

```
