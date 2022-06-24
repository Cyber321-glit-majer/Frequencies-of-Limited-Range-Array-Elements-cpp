# Frequencies-of-Limited-Range-Array-Elements-cpp
**PROBLEM STATEMENT**
Given an array A[] of N positive integers which can contain integers from 1 to P where elements can be repeated or can be absent from the array. Your task is to count the frequency of all elements from 1 to N.
Note: The elements greater than N in the array can be ignored for counting and please read your task section of the problem carefully to understand how to output the array.


Example 1:

Input:
N = 5
arr[] = {2, 3, 2, 3, 5}
P = 5
Output:
0 2 2 0 1
Explanation: 
Counting frequencies of each array element
We have:
1 occurring 0 times.
2 occurring 2 times.
3 occurring 2 times.
4 occurring 0 times.
5 occurring 1 time.

**CODE**
```
#include<bits/stdc++.h>
using namespace std ;
int main()
{
    int a[]={2, 3, 2, 3, 5};
    int n=sizeof(a)/sizeof(a[0]);
    int p=5;
    std::vector<int>v(n,0);
    for(int i=0;i<n;i++)
    {
        v[a[i]-1]++;
      
    }
    for(auto i:v)
    {
        cout<<i<<" ";
    }
   
      return 0;
}
