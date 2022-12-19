# Ujian Akhir Semester 
Mata Kuliah 	: Dasar Pemrograman
Nama	      	: Ahmad Juaeni Yunus
NIM	        : 1227050011
Jurusan		: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Definisi Matriks, Matriks merupakan sekumpulan informasi yang setiap individu elemenya diacu dengan menggunakan dua buah indeks (baris dan kolom).
Walaupun berdimensi tapid alam penyimpanan matriks tetap tersusun secara terurut.Matriks merupakan kumpulan-kumpulan bilangan yang disusun secara baris(vertikal) dan kolom(horizontal) bisa disebut juga array dua dimensi (multi-dimensional).
Transpose Matriks adalah memperoleh sebuah matriks dengan cara menukar baris menjadi kolom dan kolom menjadi baris dari sebuah matriks.
## Source Code

#include <iostream>
using namespace std;
	
const string garis = "_________________________________________________________________\n";

int main() {
	int baris, kolom, b, k,i,j;
	int A[20][20];
	string nama = "Ahmad Juaeni Yunus";
	long nim = 1227050011;
	
	cout<< garis;
	cout<<" \t\tMEMBUAT PROGRAM BARIS DAN KOLOM\n NILAI DIINPUTKAN DAN DIBALIK BARIS KE KOLOM, KOLOM KE BARIS "<<endl<<garis;
	cout << "Nama :	" <<nama<<endl;
	cout << "Nim  :	"<<nim<<endl<<garis;
	
	
	cout<<"Masukan jumlah baris : ";
	cin>>baris;
	cout<<"Masukan jumlah kolom : ";
	cin>>kolom;
	cout<<endl;
	
	for (b=1;b<=baris;b++){
		for (k=1;k<=kolom;k++){
			  cout<<"Baris["<<b<<"]Kolom["<<k<<"] = ";
			  cin>>A[b][k];
		}
		cout<<endl;
	}
	cout<<"Hasil dari nilai yang di inputkan : "<<endl;
	for (b=1;b<=baris;b++){
		for (k=1;k<=kolom;k++){
			 cout<<A[b][k]<<" ";
		}
		cout<<endl;
	}
	cout<<endl<<"Nilai dibalik baris jadi kolom, kolom jadi baris : "<<endl;
	for (b=1;b<=kolom;b++){
		for (k=1;k<=baris;k++){
			 cout<<A[k][b]<<" ";
		}
		cout<<endl<<endl<<endl;
	}
	
	cout << garis;
	cout << "PROGRAM MENCARI BILANGAN YANG TIDAK HABIS DIBAGI DENGAN 3, 5, 7\n"<<garis;
	cout << "Nama :	" <<nama<<endl;
	cout << "Nim  :	"<<nim<<endl<< garis;
	
	cout << endl << "Masukkan banyak baris: "; cin >> baris;
	cout << endl << "Masukkan banyak kolom: "; cin >> kolom;
	
	int num[20][20];
	
	for (i = 1; i <= baris; i++) {
		for (j = 1; j <= kolom; j++) {
			cout << "Num(" << i << "," << j << ") : ";
			cin >> num[i][j];
		}
	}
	cout << "Bilangan yang tidak habis dibagi 3, 5, 7 : ";
	for (i = 1; i <= baris; i++) {
		for (j = 1; j <= kolom; j++) {
			if (num[i][j] % 3 != 0 && num[i][j] % 5 != 0 && num[i][j] % 7 != 0) {
				cout << " " << num[i][j];
			} 
		}
	}
	return 0;	
}

## Output

_________________________________________________________________
                MEMBUAT PROGRAM BARIS DAN KOLOM
 NILAI DIINPUTKAN DAN DIBALIK BARIS KE KOLOM, KOLOM KE BARIS
_________________________________________________________________
Nama :  Ahmad Juaeni Yunus
Nim  :  1227050011
_________________________________________________________________
Masukan jumlah baris : 2
Masukan jumlah kolom : 3

Baris[1]Kolom[1] = 1
Baris[1]Kolom[2] = 2
Baris[1]Kolom[3] = 3

Baris[2]Kolom[1] = 4
Baris[2]Kolom[2] = 5
Baris[2]Kolom[3] = 6

Hasil dari nilai yang di inputkan :
1 2 3
4 5 6

Nilai dibalik baris jadi kolom, kolom jadi baris :
1 4


2 5


3 6


_________________________________________________________________
PROGRAM MENCARI BILANGAN YANG TIDAK HABIS DIBAGI DENGAN 3, 5, 7
_________________________________________________________________
Nama :  Ahmad Juaeni Yunus
Nim  :  1227050011
_________________________________________________________________

Masukkan banyak baris: 2

Masukkan banyak kolom: 3
Num(1,1) : 1
Num(1,2) : 2
Num(1,3) : 3
Num(2,1) : 4
Num(2,2) : 5
Num(2,3) : 6
Bilangan yang tidak habis dibagi 3, 5, 7 :  1 2 4
--------------------------------
Process exited after 16.63 seconds with return value 0
Press any key to continue . . .
