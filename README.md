//SWAP 2 NUMBERS
#include <iostream>
 using namespace std;

int main()
{
    int a = 5, b = 10, temp;

    cout << "Before swapping." << endl;
    cout << "a = " << a << ", b = " << b << endl;

    temp = a;
    a = b;
    b = temp;

    cout << "\nAfter swapping." << endl;
    cout << "a = " << a << ", b = " << b << endl;

    return 0;
}
//2.LARGEST OF THREE
  #include <iostream>
using namespace std;

int main() {    
    float n1, n2, n3;

    cout << "Enter three numbers: ";
    cin >> n1 >> n2 >> n3;

    if(n1 >= n2 && n1 >= n3)
        cout << "Largest number: " << n1;

    if(n2 >= n1 && n2 >= n3)
        cout << "Largest number: " << n2;
    
    if(n3 >= n1 && n3 >= n2)
        cout << "Largest number: " << n3;
  
    return 0;
}
  //3.LEAP YE#include <stdio.h>
int main() {
   int year;
   printf("Enter a year: ");
   scanf("%d", &year);

  
   if (year % 400 == 0) {
      printf("%d is a leap year.", year);
   }
  
   else if (year % 100 == 0) {
      printf("%d is not a leap year.", year);
   }
   
   else if (year % 4 == 0) {
      printf("%d is a leap year.", year);
   }
  
   else {
      printf("%d is not a leap year.", year);
   }

   return 0;
}
//4.FIBONACCI SERIES
  #include <iostream>
using namespace std;

int main() {
    int n, t1 = 0, t2 = 1, nextTerm = 0;

    cout << "Enter the number of terms: ";
    cin >> n;

    cout << "Fibonacci Series: ";

    for (int i = 1; i <= n; ++i) {
        // Prints the first two terms.
        if(i == 1) {
            cout << t1 << ", ";
            continue;
        }
        if(i == 2) {
            cout << t2 << ", ";
            continue;
        }
        nextTerm = t1 + t2;
        t1 = t2;
        t2 = nextTerm;
        
        cout << nextTerm << ", ";
    }
    return 0;
}
//5. PRIME OR NOT

#include <iostream>
using namespace std;

int main()
{
   
    int n, i, c = 0;
    
        cout << "Enter any number n: ";
  cin>>n;
    
        for (i = 1; i <= n; i++)
    {
        if (n % i == 0)
        {
           c++;
        }
    }
    if (c == 2)
    {
       cout << "n is a Prime number" << endl;
    }
    else
    {
         cout << "n is not a Prime number" << endl; 
    }
    return 0;    
}
 //6.PATTERN
                                                  

#include <stdio.h>

int main() {
   int n,i,j;

   n = 5;   // number of rows.

   for(i = 1; i <= n; i++) {
      for(j = 1; j <= n-i; j++)
         printf(" ");

      for(j = 1; j <= i; j++)
         printf("* ");

      printf("\n");
   }
   return 1;
}
 //7. FIND 2ND LARGEST ELEMENT IN ARRAY
 #include<iostream>
using namespace std;
int main ()
{
    int A[10], n, i, j, x;
    cout << "Enter size of array : ";
    cin >> n;
    cout << "Enter elements of array : ";
    for (i = 0; i < n; i++)
        cin >> A[i];    
    for (i = 0; i < n; i++)
    {
        for (j = i + 1; j < n; j++)
        {
            if (A[i] < A[j])
            {
                x = A[i];
                A[i] = A[j];
                A[j] = x;
            }
        }
    }
    cout << "Second largest number : " << A[1];
    cout << "\nSecond smallest number : " << A[n - 2];
    return 0;
}
                      
                                               
