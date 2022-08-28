# CPP-program-to-find-duplicate-numbers-and-their-position
#include <bits/stdc++.h>
using namespace std;  
int main()    
{    
    //Initialize array     
    int array[100],c,n;

 cout<<"Enter number of elements in array: ";
  cin>>n;

  cout<<"Enter "<<n<<" integers:"<<endl;

  for (c = 0; c < n; c++)
    cin>>array[c];
        
    cout<<"Duplicate elements and their position in given array: "<<endl;    
    //Searches for duplicate element    
    for(int i = 0; i < n; i++) {    
        for(int j = i + 1; j < n; j++) {    
            if(array[i] == array[j])    
                cout<<array[j]<<" "<<j<<endl;    
        }    
    }    
    return 0; 
}
