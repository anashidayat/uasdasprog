# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Annasrulloh Hidayat
<br>NIM		:	12227050024
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Dalam Tugas Ulangan Akhir Semester ini kita diberikan soal yang sudah dipelajari sebelumnya, sebelum mengerjakan soal ini, kita harus memahami konsep array 2 dimensi dan matriks terlebih dahulu,kemudian kita ditugaskan untuk membuat kolom serta baris dan harus membagi habis nilai yang diinputkan yang dibagi oleh bilangan prima yaitu 3,5,7.
## Source Code

Tugas 1

      #include<iostream>
      #include<iomanip>
      using namespace std;

      int main(){

        int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

        cout<< "Tugas Program Mencetak Matrix Transpos\n";
        cout<< "=======================================\n";
        cout<< "Nama  : Annasrulloh Hidayat\n";
        cout<< "Nim   : 1227050024\n";
          cout<< "                          \n";

          cout<<"Input jumlah baris: "; cin>>jumlahBaris;
          cout<<"Input jumlah kolom: "; cin>>jumlahKolom;
          cout << endl;

          for(i = 0; i < jumlahBaris; i++){
        for(j = 0; j < jumlahKolom; j++){
            cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
            cin >> arr[i][j];
        }
        cout << endl;
          }
          cout << "Hasil matriks: " << endl;

          for(i = 0; i < jumlahBaris ; i++){
          for(j = 0; j < jumlahKolom; j++){
        cout << setw(3) << arr[i][j] << " ";
          }
          cout << endl;
          }

        baris = jumlahBaris;
        kolom = jumlahKolom;

        jumlahKolom = baris;
        jumlahBaris = kolom;

        cout << "\nUbah kolom jadi baris dan baris jadi kolom: " << endl;

        for(i = 0; i < jumlahBaris ; i++){
      for(j = 0; j < jumlahKolom; j++){
      cout << setw(3) << arr[j][i] << " ";
        }
        cout << endl;
        }
      return 0;
    }

 Tugas 2

       #include <iostream>
      #include <iomanip>
      using namespace std;
      int main(){

        int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

        cout<< "Tugas Program Bilangan Yang Habis Dibagi 3,5,7\n";
        cout<< "==============================================\n";
        cout<< "Nama  : Annasrulloh\n";
        cout<< "Nim   : 1227050024\n";
        cout<< "                                               \n";

          cout<<"Input jumlah baris: "; cin>>jumlahBaris;
          cout<<"Input jumlah kolom: "; cin>>jumlahKolom;
          cout << endl;

          for(i = 0; i < jumlahBaris; i++){
        for(j = 0; j < jumlahKolom; j++){
            cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
            cin >> arr[i][j];
        }
        cout << endl;
          }

          cout << "Hasil input nilai : " << endl;

          for(i = 0; i < jumlahBaris ; i++){
          for(j = 0; j < jumlahKolom; j++){
        cout << setw(3) << arr[i][j] << " ";
          }
          cout << endl;
          }

          cout << "\nHasil bilangan yang habis dibagi 3,5,7 : " << endl;

          for(i = 0; i < jumlahBaris ; i++){
          for(j = 0; j < jumlahKolom; j++){
        if(arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0){
        cout << setw(3) << arr[i][j] << " ";
        }
          }
          cout << endl;
          }


          cout << endl;
          return 0;
      }
 
## Output
Tugas 1

Tugas Program Mencetak Matrix Transpos
Nama  : Annasrulloh Hidayat
Nim   : 1227050024

Input jumlah baris: 2
Input jumlah kolom: 3

Baris 1, kolom 1 = 3
Baris 1, kolom 2 = 5
Baris 1, kolom 3 = 7

Baris 2, kolom 1 = 9
Baris 2, kolom 2 = 7
Baris 2, kolom 3 = 6

Hasil matriks:
  3   5   7
  9   7   6

Ubah kolom jadi baris dan baris jadi kolom:
  3   9
  5   7
  7   6

Tugas 2

Tugas Program Bilangan Yang Habis Dibagi 3,5,7
Nama  : Annasrulloh
Nim   : 1227050024

Input jumlah baris: 2
Input jumlah kolom: 3

Baris 1, kolom 1 = 1
Baris 1, kolom 2 = 2
Baris 1, kolom 3 = 3

Baris 2, kolom 1 = 4
Baris 2, kolom 2 = 5
Baris 2, kolom 3 = 6

Hasil input nilai :
  1   2   3
  4   5   6

Hasil bilangan yang habis dibagi 3,5,7 :
  3
  5   6
