# notes pointer
- symbol table : mapping of variable and storage addresss
- address of storage is fetched using &var , where var is a variable of specific type
- int var = 10;
- to store address of a data type variable we use a variable that we call as pointer.
- int * pointer = &var;
- // Online C++ compiler to run C++ program online
#include <iostream>
using namespace std;

int main() {
    // Write C++ code here
    cout << "Hello world!";
    int arr[10]={0};
    cout << sizeof(&arr[0]);
    cout<< arr<<endl;
    cout<<&arr<<endl;
    cout<<&arr[0]<<endl;

    return 0;
}
 - we can not assign like this arr = arr + 3; once there is an entry in symbol table we can not change it.
    for example :
            int a[] = {1, 2, 3, 4};
            int *p = a++;
            cout << *p << endl;
    here we are trying to rewrite address of already array by doing a++; so it will result into error.
