# Tugas-adp-soal-2
#include <iostream>
#include <cmath>

using namespace std;

// Fungsi untuk menghitung tinggi segitiga tegak
double hitungTinggiSegitiga(double sisiAlas, double tinggiLimas) {
    return sqrt(pow(sisiAlas / 2, 2) + pow(tinggiLimas, 2));
}

int main() {
    double sisiAlas, tinggiLimas;

    // Input panjang sisi alas dan tinggi limas
    cout << "Masukkan panjang sisi alas limas: ";
    cin >> sisiAlas;
    cout << "Masukkan tinggi limas: ";
    cin >> tinggiLimas;

    // Hitung tinggi segitiga tegak
    double tinggiSegitiga = hitungTinggiSegitiga(sisiAlas, tinggiLimas);

    // Hitung volume limas
    double volume = (1.0/3) * pow(sisiAlas, 2) * tinggiLimas;

    // Hitung luas permukaan limas
    double luasPermukaan = pow(sisiAlas, 2) + 4 * (0.5 * sisiAlas * tinggiSegitiga);

    // Output hasil
    cout << "Volume limas: " << volume << endl;
    cout << "Luas permukaan limas: " << luasPermukaan << endl;

    return 0;
}
