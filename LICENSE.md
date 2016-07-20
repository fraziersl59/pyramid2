//Assignment #2
// calculating the area of a 2 types of pyramids.

#include <iostream>
using namespace std;
 
double pyramid (double a, double b)
{
  double pyr_vol;
  pyr_vol=(4/3)*(b*a);
  return (pyr_vol);
}

int main ()
{
  char choice;
  double l,w,h,b;
  double pyr;
  cout<<"Choose a polygon: \na-Triangle Pyramid\nb-Square Pyramid"<<endl;
  cin>>choice;
  switch (choice)
  {
  case 'a':    //begining of triangle base pyramid
 cout<<"Enter length of base\n";
 cin>>l;
 cout<<"Enter width of base\n";
 cin>>w;
b=(l*w)/2;     //formula for triangle base
cout<<"the area of the triangie base is "<<b;
 cout<<"\nEnter height\n";
 cin>>h;
 pyr = (4/3)*(b*h);     //formula to calculate area***************
 cout << "The volume of the pyramid is "<<pyr;
 break;
 case 'b':     //beginning of square base pyramid
 cout<<"Enter length of base\n";
 cin>>l;
 cout<<"Enter width of base\n";
 cin>>w;
b=(l*w);
cout<<"The area of the square base is "<<b;
 cout<<"\nEnter height\n";
 cin>>h;
 pyr = (4/3)*(b*h);    //formula to calculate area*****************
 cout << "The volume of the pyramid is "<<pyr;

 break;
 default: 
 cout<<"Out of coverage"<<endl;
 }
  return 0;
}
