# Ujian-Akhir-Semester
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Alya Nurul Lathifah
<br>NIM		:	1227050018
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Array adalah sebuah variabel yang menyimpan sekumpulan data yang memiliki tipe sama atau Array juga dapat disebut sebagai kumpulan dari nilai-nilai data bertipe sama dalam urutan tertentu yang memakai sebuah nama yang sama. Sedangkan Array dua dimensi adalah array yang terdiri dari n buah baris dan m buah kolom, atau array dua dimensi juga biasa disebut sebagai array yang mempunyai dua subskrip, yaitu baris dan kolom. dimana indeks pertama menunjukan baris dan indeks kedua menunjukan kolom. Untuk mendeklarasikan sebuah array dua dimensi dalam C++, kita harus menggunakan tanda [ ] (bracket). Adapun bentuk umum dari pendeklarasian array dua dimensi adalah sebagai berikut:

tipe_data nama_array [jumlah_elemen_baris] [jumlah_elemen_kolom];

Coding ini membahas deret matematika bilangan yang tidak habis dibagi 3, 5, dan 7.
Input baris pertama merupakan banyaknya baris dan baris kedua merupakan banyaknya kolom. Adapun output yang ditampilkan adalah bilangan yang tidak habis dibagi 3, 5, dan 7.

## Source Code

    #include <iostream>
    using namespace std;
    int main(){
    int input [100][100];
    int baris, kolom, a, k;
    cout <<"Masukan Jumlah Baris : ";
    cin >> baris;
    cout <<"Masukan Jumlah Kolom : ";
    cin >> kolom;
    cout << endl;
    for (a = 0; a < baris; a++){
    for (k = 0; k < kolom; k++){
    cout << " Baris " << a+1 << " kolom " << k+1 << " = ";
    cin >> input[a][k];
    }
    cout << endl;
    }
    cout << "Hasil : " << endl;
    for (a = 0; a < baris; a++){
    for (k = 0; k < kolom; k++){
    cout << " " << input[a][k];
    }
    cout << endl;
    }
    cout << "=================================" << endl;
    for (a = 0; a < kolom; a++){
    for (k = 0; k < baris; k++){
    cout << " " << input[k][a];
    }
    cout << endl;
    }
    }
    
    Source code 2
    
        #include <iostream>
    using namespace std;

    int main(){
      int A [20][20];
      int b, k, i, j;
      cout <<"Masukan Jumlah Baris : ";
      cin >> b;
      cout <<"Masukan Jumlah Kolom : ";
      cin >> k;

      for(i=0; i<=b-1;i++){
        for(j=0;j<=k-1;j++){
          cout <<"Masukan Nilai ("<<i<<"."<<j<<") : ";
          cin >> A[i][j];
        }
      }
      cout <<"Nilai yang diinputkan : \n";
      for(int i=0;i<b;i++){
        for(int j=0;j<k;j++){
          cout <<A[i][j]<<"\t";
        }
        cout<<endl;
      }
      int angka[20];
      int index = 0;
      for(i=0;i<b;i++){
        for(j=0;j<k;j++){
          if(A [i][j]%3 !=0 && A[i][j]%5 !=0 && A[i][j]%7 !=0){
            angka[index] = A[i][j];
            index++;
          }
        }
      }
      cout <<"Angka yang tidak bisa dibagi 3, 5, 7 adalah ";
      for(int i=0;i<index;i++){
        cout<<angka[i]<<";";
      }
    }
## Output

Code 1
<img width="71" alt="Screenshot_20221222_150931" src="https://user-images.githubusercontent.com/121221565/209099601-cc38735d-95d9-4c07-a2d5-2a906d6ef420.png">

code 2

<img width="306" alt="Screenshot_20221222_142812" src="https://user-images.githubusercontent.com/121221565/209100390-e28c8fbf-93be-411f-872a-f18fd4ba5ef5.png">


readme.md
Menampilkan readme.md.
