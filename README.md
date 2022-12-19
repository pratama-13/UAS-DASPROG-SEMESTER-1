# Ujian Akhir Semester 
<br>Mata Kuliah 	: [DASAR PEMROGRAMAN]
<br> Nama		: [MARVI YOGA PRATAMA]
<br>NIM		: [1227050070]	
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Pengertian Array 2 dimensi adalah array dengan lebih dari 2 bentuk index array. Jika pada array 1 dimensi hanya ada satu bentuk index saja, pada array 2 dimensi kita bisa menjumpai lebih dari satu bentuk index array.
Itulah mengapa array ini memiliki sebutan lain array multidimensi. Selain itu juga dapat diartikan sebagai array yang memiliki dua subskrip, yakni baris dan kolom. Sehingga bentuknya menyerupai matriks atau tabel, di mana indeks pertama merupakan baris dan indeks kedua adalah kolom.
Analogi lain adalah matriks . Dalam matematika, matriks terdiri dari kolom dan baris . Kembali, untuk menentukan nilai dari sebuah matriks, kita harus menyebutkan secara berpasangan seperti baris 1 kolom 1, atau baris 2 kolom 3, dst. Konsep seperti inilah yang menjadi dasar dari array 2 dimensi.Untuk membuat array 2 dimensi di dalam bahasa C++, caranya tulis 2 kali tanda kurung siku setelah nama variabel, seperti contoh berikut:
int arr[2][2];
Baris diatas akan membuat array 2 dimensi dengan nama variabel: arr . Variabel arr ini total berisi 4 elemen (2 x 2). Atau jika diibaratkan sebagai matriks, disini kita membuat matriks 2 x 2.

## Source Code
Soal No1:
  //Input banyaknya baris dan kolom array dimensi 2
   #include <iostream>

  using namespace std;

  int main()
  {
    cout << "Nama  : Marvi Yoga Pratama" << endl;
    cout << "NIM   : 1227050070 " << endl;
    cout << "Kelas : IF-B" << endl;
    cout << "==========================================" << endl;
    cout << "##  Program C++ Input Matriks 2 Dimensi ##" << endl;
    cout << "==========================================" << endl;
    cout << endl;

    int matriks[100][100];
    int jum_baris, jum_kolom, i, j;

    cout << "Input jumlah baris matriks: ";
    cin >> jum_baris;

    cout << "Input jumlah kolom matriks: ";
    cin >> jum_kolom;
    cout << endl;

    // proses input array
    for(i = 0; i < jum_baris ; i++){
      for(j = 0; j < jum_kolom; j++){
        cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
        cin >> matriks[i][j];
      }
      cout << endl;
    }
    for(i = 0; i < jum_baris ; i++){
      cout << endl;
      for(j = 0; j < jum_kolom; j++){
        cout << matriks[i][j];
      }
          cout << endl;
        }
        for(i = 0; i < jum_baris ; i++){
          cout << endl;
          for(j = 0; j < jum_kolom; j++){
            cout << matriks[j][i];
          }
          cout << endl;
        }
        return 0;
      }

      Soal No2:
      #include <iostream>
      #include <iomanip>
      using namespace std;
      int main(){
          int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

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

          cout << "\nHasil: " << endl;

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
![Screenshot (15)](https://user-images.githubusercontent.com/118746439/208374857-9d78059b-37b1-4249-a1d7-8c2d54bd1c9d.png)
![Screenshot (16)](https://user-images.githubusercontent.com/118746439/208374884-7d431d0b-79a3-40d0-9d54-85e2c69fd448.png)
