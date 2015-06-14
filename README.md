Lab_1
the firest lab

#include <iostream>
#include <cstdlib>
#include <string>

using namespace std;


int main (){
	
	int mas [7];
	int i;
	int temp;
	
	for (i = 0; i < 7; i++){
		cout << "[ " << i + 1 << " ]" << ":";
		cin >> mas [i];
	}
	cout << "Imeem massiv: ";
	
	for (i = 0; i < 7; ++i){
		cout << mas [i] << " ";
	}
 
	for (i = 0; i < 7 - 1; i++){
		for (int j = 0; j < 7 - i -1; j++){
			if (mas[j] > mas [j + 1]) {
				temp = mas [j];
				mas[j] = mas [j + 1];
				mas [j + 1] = temp; 
			}
		}
	}
 	cout << "Otsortirovany massiv: " << endl;
 	
 	for (i=0; i < 7; i++){
 		cout << mas [i] << " ";
 	}
	cout << endl;
	
	system ("pause");
	return 0;
}
