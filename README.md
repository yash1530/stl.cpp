# stl.cpp
#include<bits/stdc++.h>
using namespace std;

int main() {
	vector<int>v;
	v.push_back(10);
	v.push_back(20);
	v.push_back(30);
	v.emplace_back(40);
	//faster then pushback (time complexity is less)
	/*for(int i=0;i<v.size();i++)cout<<v[i]<<" ";
	v.pop_back();
	cout<<endl;
	for(auto it:v)
	{
	    cout<<it<<" ";
	}*/
	//last value -1 will print
	auto it1=v.begin();
	auto it2=v.end()-1;
	cout<<*it2;
	

	return 0;
}
****************************************************************************
             #include<bits/stdc++.h>

using namespace std;

int main() {
    vector<int>v;
	v.push_back(10);
	v.push_back(20);
	v.push_back(30);
	v.emplace_back(40);
//	for(<int>::iterator it=v.begin();it!=v.end;i++)
//	cout<<*it<<" ";
for(auto it=v.rbegin();it!=rend();it++)
cout<<*it<<" ";

	return 0;
}
**********************************************************************************
  #include<bits/stdc++.h>
using namespace std;

int main() {
/*	vector<int>v;
	v.push_back(20);
	v.push_back(10);
	v.push_back(30);
	v.emplace_back(40);

	sort(v.begin(),v.end());
	for(auto it:v)
	{
	    cout<<it<<" ";
	}*/
	int arr[]={5,4,3,2,1,10,6,18};
	int n = sizeof(arr) / sizeof(arr[0]);
	 

	sort(arr,arr+n);
	for (int i = 0; i < n; ++i)
        cout << arr[i] << " ";
 
	return 0;
}
***********************************************************************************************
 #include<bits/stdc++.h>
using namespace std;

int main() {
    
     vector<int>vet;
     vector<int>vet1;
	vet.push_back(10);
	vet.push_back(20);
	vet.push_back(30);
	vet.emplace_back(40);
	vet1.push_back(50);
	vet1.push_back(60);
	vet1.push_back(70);
	vet1.emplace_back(80);
	
	for(auto it:vet)
	{
	    cout<<it<<" ";
	}
	
cout<<endl;
for(auto it:vet1)
	{
	    cout<<it<<" ";
	}
	cout<<endl;
	
	//vet.erase(vet.begin());//remove first element
	//vet.erase(vet.begin()+1);//remove second ele
   // vet.erase(vet.begin()+1,vet.begin()+4);//1st element to 4 element
   //vet.insert(vet.begin(),10);
   
   vet.swap(vet1);
    for(auto it:vet)
	{
	    cout<<it<<" ";
	}
	cout<<endl;
	for(auto it:vet1)
	{
	    cout<<it<<" ";
	}
	//v1.swap(v2);

	return 0;
}
*************************************************************************
  #include <bits/stdc++.h>
using namespace std;

int main() {
	// your code goes here
	vector<vector<int>>mat={{1,2,3},{4,5,6},{7,8,9}};
	for(int i=0;i<mat.size();i++)
	{
	    for(int j=0;j<mat[i].size();j++)
	    {
  
	        cout<<mat[i][j]<<" ";
	    }
	    cout<<endl;

	    
	}
	return 0;
}
**********************************************************************************
  #include <bits/stdc++.h>
using namespace std;

int main() {
	// your code goes here
	/*pair<int,int>p={1,2};
	{
	    cout<<p.first<<" "<<p.second<<endl;
	    cout<<p.second<<" "<<p.first;
	    
	}*/
	/*pair<int,char>p={1,'y'};
	{
	    cout<<p.first<<" "<<p.second<<endl;
	    cout<<p.second<<" "<<p.first;
	    
	}*/
	    /*pair<string, double> p("yash", 1.23);
	    {
	        cout<<p.first<<" "<<p.second<<endl;
	    }*/

	
	
	//pair<int,char>;
	//pair<str,str>;
/*	vector<pair<int,int>>p;
	p.push_back({10,20});
	p.push_back({30,40});
	for(auto it:p)
	{
	    cout<<it.first<<" "<<it.second<<endl;
	    
	    
	}*/
	vector<pair<int,pair<int,int>>>p={{1,{0,4}},{2,{1,3}}};//pair in a pair
	for(auto it:p)
	cout<<it.first<<" "<<it.second.first<<" "<<it.second.second<<endl;
	return 0;
}
