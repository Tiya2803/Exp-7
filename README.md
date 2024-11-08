# Experiment 7
# Aim:
To study and implement C++ Arrays and Strings

# Theory:
C++ arrays are collections of elements with mutually inclusive types which stay together in one contiguous memory space. They can be declared by presenting the type of these elements followed by square brackets that hold their numbers. In other words, arrays begin counting from zero; thus for instance character zero on array becomes the first one while second one becomes character one and so forth. C++ arrays have fixed sizes that must be determined at compile time.
In C++, strings are managed through either C-style string or by utilizing the string class which is included in the Standard Library. In this programming language, strings are made up of groups of characters terminated by a null character (‘\0’). Actions on C-styled strings are done by functions from C standard library like strlen, strcpy and strcat.

# Code:
a.
```
#include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int a[n];
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i <<" of  the array: ";
        cin>>a[i];

    }
    cout<<endl;
    cout<<"The array defined by the user: "<<endl;
    cout<<"{";
    for(i = 0; i < n;i++)
    {
        cout<<a[i]<<" ";

    }
    cout<<"}";
    cout<<endl;

    return 0;
}
```
b.
```
#include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int a[n];
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i+1 <<" of  the array: ";
        cin>>a[i];

    }
    cout<<endl;
    cout<<"The array defined by the user: "<<endl;
    for(i = 0; i < n;i++)
    {
        cout<<a[i]<<" ";

    }
    cout<<endl;

    cout<<"The array reversed: "<<endl;
    cout<<"{ ";
    for(i = n-1 ; i > -1 ;i--)
    {
        cout<<a[i]<<" ";

    }
    cout<<"}";
    cout<<endl;

    return 0;
}
```
c.
```
#include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int num = 0, co = 0, flag = 0;
    int a[n];
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i+1 <<" of  the array: ";
        cin>>a[i];
    }
    cout<<endl;
    cout<<"Enter the number you want to check: ";
    cin>>num;
    for(i = 0; i < n;i++)
    {
        if(a[i] == num)
        {
            co++;
            flag++;

        }
    }
    if (flag == 0)
    {
        cout<<"Element was not found.";
    }
    else
    {
        cout<<"The element was found "<<co<<" times.";
    }

}
```
d.
```
#include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int a[n];
    int num = 0, maxi = 0, mini = a[0];
    
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i+1 <<" of  the array: ";
        cin>>a[i];
    }
    cout<<endl;
    for(i = 0; i < n;i++)
    {
        if(a[i] > maxi)
        {
            maxi = a[i];
        }
        if(a[i] < mini)
        {
            mini = a[i];
        }
    }
    cout<<"Maximum value amongst the elements are: "<<maxi<<endl;
    cout<<"Minimum value amongst the elements are: "<<mini<<endl;


}
```
e.
```
#include <iostream>
using namespace std;
int main()
{
    int n = 0,i = 0;
    int num = 0, sum = 0, avg = 0;
    int a[n];
    cout<<"Enter size of array: ";
    cin>>n;
    for(i = 0; i < n;i++)
    {
        cout<<"Enter element no. "<< i+1 <<" of  the array: ";
        cin>>a[i];
    }
    cout<<endl;
    for(i = 0; i < n;i++)
    {
        sum = sum + a[i];
    }
    avg = sum/n;
    cout<<"Sum of elements: "<<sum<<endl;
    cout<<"Average of elements: "<<avg<<endl;


}
```
f.
```
#include <iostream>
#include <string>
using namespace std; 

int main()
{
    //printing a string
    string s;
    cout<<"Enter a word: ";
    cin>>s;
    cout<<"Word entered by user is: "<<s<<endl;
    cout<<endl;

    //concatenation of a string
    string s1,s2;
    cout<<"Enter a word: ";
    cin>>s1;
    cout<<"Enter another word: ";
    cin>>s2;
    cout<<"Concatenated word is: "<<s1+s2<<endl;
    cout<<endl;

    //printing string in reverse
    string s3;
    int i = 0;
    cout<<"Enter a word: ";
    cin>>s3;
    cout<<"Reverse String: ";
    for (i = s3.length()-1; i>=0; i-- )
    {
        cout<<s3[i];
    }
    cout<<endl;
    cout<<endl;

    //checking if a string is a palindrome.
    string s4,rs;
    int j = 0;
    cout<<"Enter a word: ";
    cin>>s4;
    for (j = s4.length()-1; j>=0; j-- )
    {
        rs = rs + s4[j];
    }
    if (rs == s4)
    {
        cout<<"It is a palindrome."<<endl;
    }
    else
    {
        cout<<"It is not a palindrome."<<endl;   
    }
    cout<<endl;
}
```

# Output:

a.<BR>![image](https://github.com/user-attachments/assets/a3e5ad8c-c35f-4c4f-870f-0bf4c06f000f)

b.<br>![image](https://github.com/user-attachments/assets/aff92238-19b1-4fee-a117-c384b77cdc6d)

c.<br>![image](https://github.com/user-attachments/assets/680bb4ed-3567-419b-aa81-cf01a4d7118e)

d.<br>![image](https://github.com/user-attachments/assets/40498290-390e-4efd-95c9-3bbf4f7d0f8b)

e.<br>![image](https://github.com/user-attachments/assets/634f8fc6-05f5-4893-b2a9-d3227d458a82)

f.<br>![image](https://github.com/user-attachments/assets/9cf8b90c-e0ec-4f15-aec4-f43fca77cd98)


# Conclusion:

→ We learnt the use case of arrays in C++.

→ We learnt how to perform basic string manipulations in C++.
