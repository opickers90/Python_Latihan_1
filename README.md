# Python_Latihan_1

1)	Kebalikan dari Sepuluh:
Buatlah sebuah fungsi `bukan_sepuluh(num1, num2)` yang menerima dua angka. Fungsi ini harus mengembalikan `True` jika penjumlahan dari `num1` dan `num2` bukan sepuluh, dan `False` jika hasilnya sepuluh.
```python
# Tulis fungsi bukan_sepuluh di sini
def bukan_sepuluh(num1, num2):
    return num1 + num2 != 10

# Uncomment untuk menguji fungsi bukan_sepuluh
# print(bukan_sepuluh(9, 1))  # harus mencetak False
# print(bukan_sepuluh(9, -1))  # harus mencetak True
```

2)	Di Atas Anggaran:
Definisikan sebuah fungsi `atas_anggaran(anggaran, *pengeluaran)` yang menerima sejumlah anggaran bulanan dan sebuah daftar pengeluaran. Fungsi ini harus mengembalikan `True` jika total pengeluaran lebih dari anggaran, dan `False` jika tidak.
```python
# Tulis fungsi atas_anggaran di sini
def atas_anggaran(anggaran, *pengeluaran):
    return sum(pengeluaran) > anggaran

# Uncomment untuk menguji fungsi atas_anggaran
# print(atas_anggaran(100, 20, 30, 10, 40))  # harus mencetak False
# print(atas_anggaran(100, 50, 30, 20, 10))  # harus mencetak True
```

3)	Daya Besar:
Buatlah fungsi `daya_besar(base, eksponen)` yang mengembalikan `True` jika `base` pangkat `eksponen` lebih dari 5000, dan `False` jika tidak.
```python
# Tulis fungsi daya_besar di sini
def daya_besar(base, eksponen):
    return base ** eksponen > 5000
# Uncomment untuk menguji fungsi daya_besar
# print(daya_besar(2, 13))  # harus mencetak True
# print(daya_besar(2, 12))  # harus mencetak False
```

4)	Faktorial:
Tuliskan fungsi `faktorial(n)` yang menghitung nilai faktorial dari sebuah angka `n`. Faktorial dari `n` adalah hasil kali semua bilangan bulat positif hingga `n`.
```python
# Tulis fungsi faktorial di sini
def faktorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * faktorial(n - 1)

# Uncomment untuk menguji fungsi faktorial
# print(faktorial(5))  # harus mencetak 120
# print(faktorial(4))  # harus mencetak 24
```

5)	Cari Karakter:
Definisikan sebuah fungsi `cari_karakter(kalimat, karakter)` yang mengembalikan jumlah kemunculan `karakter` dalam sebuah `kalimat`.
```python
# Tulis fungsi cari_karakter di sini
def cari_karakter(kalimat, karakter):
    return kalimat.count(karakter)

# Uncomment untuk menguji fungsi cari_karakter
# print(cari_karakter("hello world", "o"))  # harus mencetak 2
# print(cari_karakter("hello world", "l"))  # harus mencetak 3
```

6)	Konversi Suhu:
Buatlah fungsi `konversi_suhu(dari, ke, suhu)` yang mengubah suhu dari Celsius ke Fahrenheit atau sebaliknya. Parameter `dari` dan `ke` adalah string yang bisa bernilai `"C"` atau `"F"`.
```python
# Tulis fungsi konversi_suhu di sini
def konversi_suhu(dari, ke, suhu):
    if dari == "C" and ke == "F":
        return suhu * 9/5 + 32
    elif dari == "F" and ke == "C":
        return (suhu - 32) * 5/9
    else:
        return "Konversi tidak valid"

# Uncomment untuk menguji fungsi konversi_suhu
# print(konversi_suhu("C", "F", 0))  # harus mencetak 32
# print(konversi_suhu("F", "C", 32))  # harus mencetak 0
```

7)	Cek Bilangan Prima:
Tuliskan sebuah fungsi `apakah_prima(n)` yang mengembalikan `True` jika `n` adalah bilangan prima, dan `False` jika bukan.
```python
# Tulis fungsi apakah_prima di sini
def apakah_prima(n):
    if n <= 1:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True

# Uncomment untuk menguji fungsi apakah_prima
# print(apakah_prima(11))  # harus mencetak True
# print(apakah_prima(10))  # harus mencetak False
```

8)	Bilangan Genap Ganjil dalam List:
Definisikan fungsi `hitung_genap_ganjil(daftar_angka)` yang menerima sebuah list dan mengembalikan tuple yang berisi jumlah bilangan genap dan ganjil dalam list tersebut.
```python
# Tulis fungsi hitung_genap_ganjil di sini
def hitung_genap_ganjil(daftar_angka):
    genap = sum(1 for x in daftar_angka if x % 2 == 0)
    ganjil = sum(1 for x in daftar_angka if x % 2 != 0)
    return (genap, ganjil)

# Uncomment untuk menguji fungsi hitung_genap_ganjil
# print(hitung_genap_ganjil([1, 2, 3, 4, 5]))  # harus mencetak (2, 3)
# print(hitung_genap_ganjil([10, 20, 30]))  # harus mencetak (3, 0)
```

9)	Balik Kata:
Buatlah fungsi `balik_kata(kata)` yang mengembalikan `kata` yang di-invers (dibalik).
```python
# Tulis fungsi balik_kata di sini
def balik_kata(kata):
    return kata[::-1]

# Uncomment untuk menguji fungsi balik_kata
# print(balik_kata("Python"))  # harus mencetak "nohtyP"
# print(balik_kata("Kata"))  # harus mencetak "ataK"
```

10)	Cari Terbesar dalam List:
Definisikan fungsi `cari_terbesar(daftar_angka)` yang mengembalikan angka terbesar dalam sebuah list.
```python
# Tulis fungsi cari_terbesar di sini
def cari_terbesar(daftar_angka):
    return max(daftar_angka)

# Uncomment untuk menguji fungsi cari_terbesar
# print(cari_terbesar([1, 2, 3, 4, 5]))  # harus mencetak 5
# print(cari_terbesar([10, 9, 8]))  # harus mencetak 10
```

11)	Pengurangan Rekursif:
Tulis fungsi `kurangi_rekursif(angka)` yang mengembalikan total pengurangan semua angka dari `angka` ke 0.
```python
# Tulis fungsi kurangi_rekursif di sini
def kurangi_rekursif(angka):
    if angka == 0:
        return 0
    else:
        return angka + kurangi_rekursif(angka - 1)

# Uncomment untuk menguji fungsi kurangi_rekursif
# print(kurangi_rekursif(10))  # harus mencetak 55
# print(kurangi_rekursif(5))  # harus mencetak 15
```

12)	Palindrome:
Buatlah fungsi `apakah_palindrome(kata)` yang memeriksa apakah sebuah `kata` adalah palindrome atau bukan.
```python
# Tulis fungsi apakah_palindrome di sini
def apakah_palindrome(kata):
    return kata == kata[::-1]

# Uncomment untuk menguji fungsi apakah_palindrome
# print(apakah_palindrome("kayak"))  # harus mencetak True
# print(apakah_palindrome("python"))  # harus mencetak False
```

13)	Cari Rata-Rata:
Definisikan sebuah fungsi `cari_rata_rata(daftar_angka)` yang menghitung dan mengembalikan rata-rata dari angka-angka dalam list.
```python
# Tulis fungsi cari_rata_rata di sini
def cari_rata_rata(daftar_angka):
    return sum(daftar_angka) / len(daftar_angka)

# Uncomment untuk menguji fungsi cari_rata_rata
# print(cari_rata_rata([1, 2, 3, 4, 5]))  # harus mencetak 3.0
# print(cari_rata_rata([10, 20, 30]))  # harus mencetak 20.0
```

14)	Tambahkan Border:
Tuliskan sebuah fungsi `tambahkan_border(kata, simbol)` yang mengembalikan `kata` dengan `simbol` yang ditambahkan di awal dan di akhir kata.
```python
# Tulis fungsi tambahkan_border di sini
def tambahkan_border(kata, simbol):
    return simbol + kata + simbol

# Uncomment untuk menguji fungsi tambahkan_border
# print(tambahkan_border("kata", "*"))  # harus mencetak "*kata*"
# print(tambahkan_border("hello", "-"))  # harus mencetak "-hello-"
```

15)	Cek Kelipatan:
Definisikan fungsi `cek_kelipatan(bilangan, kelipatan)` yang mengembalikan `True` jika `bilangan` adalah kelipatan dari `kelipatan`.
```python
# Tulis fungsi cek_kelipatan di sini
def cek_kelipatan(bilangan, kelipatan):
    return bilangan % kelipatan == 0

# Uncomment untuk menguji fungsi cek_kelipatan
# print(cek_kelipatan(10, 2))  # harus mencetak True
# print(cek_kelipatan(10, 3))  # harus mencetak False
```

16)	List ke String:
Buatlah fungsi `list_ke_string(daftar_kata)` yang menggabungkan elemen-elemen dalam list `daftar_kata` menjadi sebuah string dengan spasi sebagai pemisah.
```python
# Tulis fungsi list_ke_string di sini
def list_ke_string(daftar_kata):
    return ' '.join(daftar_kata)

# Uncomment untuk menguji fungsi list_ke_string
# print(list_ke_string(["Python", "adalah", "menyenangkan"]))  # harus mencetak "Python adalah menyenangkan"
# print(list_ke_string(["satu", "dua", "tiga"]))  # harus mencetak "satu dua tiga"
```

17)	Hapus Duplikat:
Tuliskan fungsi `hapus_duplikat(daftar)` yang menerima sebuah list dan mengembalikan list baru tanpa elemen yang duplikat.
```python
# Tulis fungsi hapus_duplikat di sini
def hapus_duplikat(daftar):
    return list(set(daftar))

# Uncomment untuk menguji fungsi hapus_duplikat
# print(hapus_duplikat([1, 2, 2, 3, 3, 3]))  # harus mencetak [1, 2, 3]
# print(hapus_duplikat(["apple", "banana", "apple"]))  # harus mencetak ["apple", "banana"]
```

18)	Pencarian Binari:
Definisikan sebuah fungsi `pencarian_binari(daftar_terurut, target)` yang menerapkan pencarian binari pada list terurut `daftar_terurut` untuk menemukan `target`.
```python
# Tulis fungsi pencarian_binari di sini
def pencarian_binari(daftar_terurut, target):
    low = 0
    high = len(daftar_terurut) - 1
    while low <= high:
        mid = (low + high) // 2
        if daftar_terurut[mid] == target:
            return mid
        elif daftar_terurut[mid] < target:
            low = mid + 1
        else:
            high = mid - 1
    return None

# Uncomment untuk menguji fungsi pencarian_binari
# print(pencarian_binari([1, 2, 3, 4, 5], 3))  # harus mencetak posisi index dari 3, misalnya 2
# print(pencarian_binari([1, 2, 3, 4, 5], 6))  # harus mencetak None
```

19)	Jumlahkan Prima:
Buatlah fungsi `jumlahkan_prima(n)` yang menghitung dan mengembalikan jumlah dari semua bilangan prima hingga `n`.
```python
# Tulis fungsi jumlahkan_prima di sini
def jumlahkan_prima(n):
    total = 0
    for num in range(2, n + 1):
        if all(num % i != 0 for i in range(2, int(num**0.5) + 1)):
            total += num
    return total

# Uncomment untuk menguji fungsi jumlahkan_prima
# print(jumlahkan_prima(10))  # harus mencetak jumlah dari semua bilangan prima hingga 10
# print(jumlahkan_prima(20))  # harus mencetak jumlah dari semua bilangan prima hingga 20
```

20)	Gabungan List Tanpa Duplikat:
Definisikan sebuah fungsi `gabung_list(list1, list2)` yang menggabungkan dua list menjadi satu tanpa elemen yang duplikat.
```python
# Tulis fungsi gabung_list di sini
def gabung_list(list1, list2):
    return list(set(list1 + list2))

# Uncomment untuk menguji fungsi gabung_list
# print(gabung_list([1, 2, 3], [2, 3, 4]))  # harus mencetak [1, 2, 3, 4]
# print(gabung_list(["a", "b", "c"], ["d", "e", "f"]))  # harus mencetak ["a", "b", "c", "d", "e", "f"]
```
