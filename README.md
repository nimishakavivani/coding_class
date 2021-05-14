# coding_class
#include <iostream>
using namespace std;
bool isPrime(int n){
   for(int i = 2; i < n/2; i++){
      if(n%i == 0){
         return false;
      }
   }
   return true;
}
int findPrimeSum(int n){
   int sumVal = 0;
   for(float i = 2; i <= n; i++){
      if(isPrime(i))
         sumVal += i;
   }
   return sumVal;
}
int main(){
   int n = 15;
   cout<<"The sum of prime number between 1 to "<<n<<" is "<<findPrimeSum(n);
   return 0;
}
