/*Використовуючи покажчики та оператор розіменування, визначити найбільше з двох чисел.
*/
//рішення
#include <iostream>
using namespace std;
int main() {
 int a;
 cout << "Enter the number: ";
 cin >> a;
 int* ptr = &a;
 int c;
 cout << "Enter the second number: ";
 cin >> c;
 int* ptr2 = &c;
 if (*ptr > *ptr2) {
  cout << "a > c" << endl;
 }
 else {
  cout << "c > a" << endl;
 }
 return 0;
}

/*Використовуючи покажчики та оператор розіменування, обміняти місцями значення двох змінних.*/
//рішення

void Masiv(int*, int one, int second) {
 int* ptr = &one;
 int* prt4 = &second;
 int replacement = *ptr;
 *ptr = *ptr4;
 *ptr4 = replacement;
}
return 0;
}

int main() {
 int one = 7;
 int second = 8;
 int* ptr = &one;
 int* ptr4 = &second;
 Masiv(int*, int one, int second);

}

/*Використовуючи покажчики та оператор розіменування, визначити знак числа, введеного з клавіатури.*/
//рішення

#include <iostream>

int main() {
 int number;
 cout << "Enter a number: ";
 cin >> number;

 int* ptr_number = &number;

 if (*ptr_number > 0) {
  cout << "The number " << *ptr_number << " is positive." << endl;
 }
 else if (*ptr_number < 0) {
  cout << "The number " << *ptr_number << " is negative." << endl;
 }
 else {
  cout << "The number " << *ptr_number << " is zero." << endl;
 }

 return 0;
}

/*Написати примітивний калькулятор, користуючись тільки покажчиками.*/
//рішення

#include <iostream>
using namespace std;
int main() {
 double number1, number2;
 char operation;

 double* ptrOne = &number1;
 double* ptrTwo = &number2;

 cout << "Enter the first number: ";
 cin >> *ptrOne;
 
 cout << "Enter an operation(+,-,*,/)" << endl;
 cin >> operation;
 
 cout << "Enter the second number: ";
 cin >> *ptrTwo;

 double result;
 double* pResult = &result;

 switch(operation){
 case '+':
  *pResult = *ptrOne + *ptrTwo;
  cout << "Result: " << *ptrOne << '+' << *ptrTwo;
 }
 case '-':
  *pResult = *ptrOne - *ptrTwo;
  cout << "Result: " << *ptrOne << '-' << *ptrTwo;
 }
 case '*'{
  *pResult = *ptrOne * *ptrTwo;
  cout << "Result:" << *ptrOne << '*' << *ptrTwo;

 }
 case '/'{
  if (*ptrTwo != 0) {
   *pResult = *ptrOne / *ptrTwo;
   cout << "Result: " << *ptrOne << '/' << *ptrTwo;

  }
  else {
   cout << "Error" << endl;
  }
  break;
 }
}


 


/*5. Даны два массива: А[M] и B[N] (M и  N вводятся с клавиатуры). Необходимо создать третий массив минимально возможного 
размера, в котором нужно собрать элементы массива A, которые не включаются в массив B.*/
//рішення

#include <iostream>
using namespace std;

 int main() {
  const int n1 = 8;
  int A[m] = { 56, 73, 67, 24, 67, 54, 98, 12 };
  const int m1 = 4;
  int B[n] = { 73, 91, 86, 34 };
  const int totalSize = n + m;
  int C[totalSize];

  int* ptr6 = A;
  int* ptr7 = B;
  int* ptr5 = C;

  for (int i = 0; i < n; i++) {
   *ptr5 = *ptr6;
   ptr5++;
   ptr6++;
  }
  for (int i = 0; i < m; i++) {
   *ptr5 = *ptr7;
   ptr5++;
   ptr7++;
  }

  cout << "Елементи обох масивів:" << endl;
  for (int i = 0; i < totalSize; i++) {
   cout << C[i] << " ";
  }
  cout << "\n\n";


  int sizeCommon;
  if (n < m) {
   sizeCommon = n;
  }
  else {
   sizeCommon = m;
  }
  int common[sizeCommon];
  int countCommon = 0;
  for (int i = 0; i < n; i++) {
   for (int j = 0; j < m; j++) {
    if (A[i] == B[j]) {

     int alreadyAdded = 0;
     for (int k = 0; k < countCommon; k++) {
      if (common[k] == A[i]) {
       alreadyAdded = 1;
       break;
      }
     }
     if (!alreadyAdded) {
      common[countCommon] = A[i];
      countCommon++;
     }
    }
   }
  }
  cout << "Загальні елементи двох масивів:" << endl;
  for (int i = 0; i < countCommon; i++) {
   cout << common[i] << " ";
  }
  cout << "\n";
