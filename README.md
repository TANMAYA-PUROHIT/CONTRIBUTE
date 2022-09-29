# CONTRIBUTE
CODE HELP
#include<iostream>
#include<iostream>
#include<vector>
using namespace std;
void getmaxelement(int arr[],int size,int index,int& maxi){
    //base case
    if (index==size)
    return ;
    maxi=max(maxi,arr[index]);
    //RR
    getmaxelement(arr,size,index+1,maxi);

}
int main()
{
    int arr[]={8,4,97,8,5,};
    int size=5;
    int maxi=INT8_MIN;
    getmaxelement(arr,size,0,maxi);
    cout<<maxi<<endl;
    return 0;

}
