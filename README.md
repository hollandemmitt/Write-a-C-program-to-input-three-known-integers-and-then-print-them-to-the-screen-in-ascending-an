# Write-a-C-program-to-input-three-known-integers-and-then-print-them-to-the-screen-in-ascending-an
Write a C++ program to input three known integers, and then print them to the screen in ascending and descending order.
#include <iostream>

void Sort(int &a, int &b, int &c){
     if(a>b){
        int tmp = a;
        a = b;
        b = tmp;
     }
     if(a>c){
        int tmp = a;
        a=c;
        c = tmp;
     }
     if(b>c){
        int tmp = b;
        b=c;
        c=tmp;
     }
     return;
}

int main(){
     std::cout << "Draw 3 so nguyen: " << std::endl;
     int num1;
     int num2;
     int num3;
     std::cin >> num1 >> num2 >> num3;

     int output1 = num1;
     int output2 = num2;
     int output3 = num3;

     Sort(output1,output2,output3);

     std::cout << num1 << " " << num2 << " " << num3 << " "
          << " when you try to see the next page: ";
     std::cout << output1 << " " << output2 << " " << output3 << std::endl;

     return 0;
}
