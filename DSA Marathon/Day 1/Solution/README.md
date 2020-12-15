//code by suman276 ..submission for DSC DSA marathon by gaurav verma 
#include <iostream>
#include <set>
#include <iterator>
using namespace std;

int main() {
	int cases; 
	cin>>cases;
	while(cases>0){
	    int num;
	    cin>>num;
	    int arr[num];
	    set<int> comp;
	    
	    for(int i=0; i<=num; i++){
	        int s;
	        cin>>s;
	        comp.insert(s);
	        arr[i]=s;
	    }
	    int sum1=0;
	    int sum2=0;
	    
	   for (auto const &i: comp) {
        sum1 += i;
    }
	    for(int i=0; i<=num; i++){
	        sum2+=arr[i];
	    }
	    cout<<sum2-sum1<<endl;
	    cases--;
	}
	return 0;
}
