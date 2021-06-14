# C++ Algorithm-LMN-s
C++ Last Minute Notes(LMN's) For Algorithm


## C++ Algorithms:
>[demystifying C++ Algo.]


# vector<int> arr = {1, 2, 3 ,8,1};
##  vector<int> ar = {1,5,9,1,22};

>Binary Search = [binary_search(arr.begin(),arr.end(),2);]                      => 1

>Is vector Sorted? =[is_sorted(arr.begin(),arr.end());]                         => 0
  
>Get Lower Bound = [*lower_bound(arr.begin(),arr.end(),2);]                     =>2
  
>Get Upper Bound = [*upper_bound(arr.begin(),arr.end(),2);]                     =>3
  
 >Check Sort For Certain Range = [is_sorted_until(arr.begin(),arr.end());]      =>[1, 2, 3 ,8,5}-?or)3arg(cmp)5
  
 >FindAdjacent=[*adjacent_find(arr.begin(),arr.end(),cmp);^above ex:if fails]   =>8
  
 >Count Elements = [count(arr.begin(),arr.end(),1); {1, 2, 3 ,8,1};]            =>2
 
 >Find Elements = [find(arr.begin(),arr.end(),12)!=arr.end());]                 =>0
  
 >Replace Elemenents = [replace(arr.begin(),arr.end(),1,21);]                  =>arr[0]//21

 >Swap Elements = [swap(arr[0],arr[1]);]                                       =>2,1
  
 >Move To Another Array = [move(arr.begin(),arr.end(),a.begin());]            =>arr+ar=a
  
 >Fill Elements = [fill(arr.begin(),arr.end(),3);	]                           => arr=3,3,3,3,3	
  
 >Merge vect = [merge(arr.begin(),arr.end(),ar.begin(),ar.end(),a.begin());]  =>merge2_ar into 1
  
 >Intersection =[set_intersection(arr.begin(),arr.end(),ar.begin(),ar.end(),a.begin());]  =>//    indexWiseInteractionCheck
	 
>Union = [set_union(arr.begin(),arr.end(),ar.begin(),ar.end(),a.begin());]    => indexWiseUnionCheck
  
  
 # Code
  
  ```
#include<bits/stdc++.h>
using namespace std;
bool cmp(int a,int b){return a>b;}
int main(){
	 vector<int> arr = {1, 2, 3 ,8,1};
	 vector<int> ar = {1,5,9,1,22};
	 vector<int> a(arr.size()+ar.size());
	 //cout<<binary_search(arr.begin(),arr.end(),2);							
	 //cout<<is_sorted(arr.begin(),arr.end());  							   	 
	 //cout<<*lower_bound(arr.begin(),arr.end(),2); 							 
	 //cout<<*upper_bound(arr.begin(),arr.end(),2); 							 
	 //cout<<*is_sorted_until(arr.begin(),arr.end());{1, 2, 3 ,8,5}-?or)3arg(cmp)
	 //cout<<*adjacent_find(arr.begin(),arr.end(),cmp);^above ex:if fails		 
	 //cout<<count(arr.begin(),arr.end(),1); {1, 2, 3 ,8,1};					 
	 //cout<<(find(arr.begin(),arr.end(),12)!=arr.end());=>if u srch fr ele		 
	 //replace(arr.begin(),arr.end(),1,21); needs two xtra args(s,e,act,alt)All  arr[0]=21
	 //swap(arr[0],arr[1]);   swapin => 1,2								     	 
	 //move(arr.begin(),arr.end(),a.begin()); vector<int> a(5);move all ele to	
	 //fill(arr.begin(),arr.end(),3);								
	 //merge(arr.begin(),arr.end(),ar.begin(),ar.end(),a.begin());				
	 //set_intersection(arr.begin(),arr.end(),ar.begin(),ar.end(),a.begin());   
	 //set_union(arr.begin(),arr.end(),ar.begin(),ar.end(),a.begin());          
	 
	 for(auto it:a)cout<<it<<" "; 
	 
}
```
  
 ## Thank You
  
