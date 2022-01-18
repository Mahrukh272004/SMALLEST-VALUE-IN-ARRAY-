# SMALLEST-VALUE-IN-ARRAY-#include <iostream>

using namespace std;
int main()
{
    cout << "Enter the size of array" << endl;
    int  a;
    cin >> a;
    int Array [a];
    for (int count=0; count<a; count++)
    {
        cout << "Enter num" << endl;
        cin >> Array[count];
    }
    
    for (int count1=0; count1<a; count1++)
    {
        for (int count2=0; count2<a; count2++)
        {
        if (Array[count2]>Array[count1])
        {
        int tempvalue = Array[count1];
        Array[count1]= Array[count2];
        Array[count2]=tempvalue;
        }
        }
    }
   
 cout << "The second smallest number is " << Array[1] ;  
 return 0;
}
