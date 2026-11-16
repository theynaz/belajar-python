# Python Programming Fundamentals & OOP

Repositori ini berisi kumpulan kode latihan pemrograman Python terstruktur yang mencakup sintaks dasar, struktur data, pemrograman berorientasi objek (OOP), penanganan *exception*, operasi *file* (I/O), hingga modularisasi menggunakan *module* dan *package*. Setiap modul dilengkapi dengan tangkapan layar (*screenshot*) hasil eksekusi terminal di dalam direktori `assets/`.

---

## Daftar Materi & Berkas Kode

### 1. Dasar-Dasar Python (*Python Basics*)
- **Hello World & Output Dasar**: Menampilkan teks ke terminal menggunakan `print()`.
- **Variabel, Tipe Data & Konstanta**: Deklarasi variabel dinamis, tipe data primitif (`str`, `int`, `float`, `bool`), serta konvensi konstanta huruf kapital.
- **Operator & Alur Kontrol (*Control Flow*)**: Operasi aritmatika, perbandingan, logika, percabangan (`if-elif-else`), serta perulangan (`for` dan `while`).

### 2. Function (`functions`)
| Berkas | Deskripsi |
| :--- | :--- |
| `func_basic.py` | Definisi dan pemanggilan fungsi sederhana (`sapa`) menggunakan kata kunci `def`. |
| `func_parameters.py` | Pengiriman argumen ke dalam parameter fungsi (`sapa_nama`). |
| `func_return.py` | Pengembalian nilai hasil komputasi fungsi (`tambah`) menggunakan `return`. |
| `func_default_param.py` | Penggunaan nilai parameter opsional (*default value*) pada fungsi `sapa_orang`. |
| `func_args_kwargs.py` | Penanganan argumen dinamis tak terbatas menggunakan `*args` (`jumlahkan`) dan `**kwargs` (`biodata`). |

### 3. Struktur Data Koleksi (`collections` & `dicts`)
| Berkas | Deskripsi |
| :--- | :--- |
| `list_operations.py` | Operasi koleksi *mutable* `List`: *indexing*, `append()`, pembaruan elemen, dan `remove()`. |
| `tuple_operations.py` | Operasi koleksi *immutable* `Tuple`: akses indeks dan iterasi menggunakan `for`. |
| `set_operations.py` | Deduplikasi elemen unik otomatis, `add()`, `remove()`, serta operasi himpunan (`\|`, `&`, `-`). |
| `dict_create_access.py` | Pembuatan `Dictionary` (`mahasiswa`) dan pengambilan nilai aman dengan `.get()`. |
| `dict_update_delete.py` | Penambahan *key* baru, pembaruan nilai, serta penghapusan data via `.pop()` dan `del`. |
| `dict_iteration.py` | Perulangan pasangan *key-value* menggunakan metode `.items()`. |
| `dict_nested.py` | Struktur dan pengaksesan *nested dictionary* bertingkat (`kampus`). |

### 4. Pemrograman Berorientasi Objek (`oop`)
| Topik | Berkas | Deskripsi |
| :--- | :--- | :--- |
| **Class & Object** | `oop_class_object.py` | Pembuatan *blueprint* `class Mahasiswa`, konstruktor `__init__`, dan instansiasi objek. |
| **Atribut & Method** | `oop_attributes_methods.py` | Implementasi atribut instance dan *method* kalkulasi (`luas`, `keliling`) pada `PersegiPanjang`. |
| **Encapsulation** | `oop_encapsulation.py` | Penyembunyian atribut internal dasar (`__saldo`) pada `BankAccount`. |
| **Access Modifiers** | `access_modifiers.py` | Konvensi visibilitas atribut `public`, `_protected`, dan `__private`. |
| **Private Encapsulation** | `bank_account_encapsulation.py` | Implementasi lengkap *getter* (`lihat_saldo`) dan *setter* bervalidasi (`setor`, `tarik`). |
| **Inheritance Dasar** | `inheritance_basic.py` | Pewarisan *parent class* `Hewan` oleh *child class* `Kucing` dan `Anjing`. |
| **Subclass Extension** | `inheritance_subclass_method.py` | Penambahan *method* spesifik `terbang()` pada *subclass* `Burung(Hewan)`. |
| **Super Access** | `inheritance_super.py` | Penggunaan `super()` untuk memperluas konstruktor dan *method* induk pada `MahasiswaBaru`. |
| **Polymorphism (Method)** | `polymorphism_method.py` | Antarmuka *method* `suara()` yang sama pada kelas berbeda (`Kucing` & `Anjing`). |
| **Polymorphism (Inheritance)** | `polymorphism_inheritance.py` | Penimpaan (*method overriding*) `suara()` pada hierarki kelas `Hewan`. |
| **Polymorphism (Function)** | `polymorphism_function.py` | Penerapan *duck typing* melalui fungsi `cetak_suara(hewan)`. |
| **Polymorphism (Built-in)** | `polymorphism_builtin.py` | Perilaku polimorfik fungsi bawaan `len()` pada `str`, `list`, dan `dict`. |
| **Abstraction (ABC)** | `abstraction_basic.py` | Pembuatan *abstract base class* `Hewan(ABC)` menggunakan modul `abc` dan `@abstractmethod`. |
| **Abstraction (Studi Kasus)** | `abstraction_payment.py` | Simulasi antarmuka pembayaran `Pembayaran(ABC)` untuk kelas `Gopay` dan `Dana`. |

### 5. Exception Handling (`exceptions`)
| Berkas | Deskripsi |
| :--- | :--- |
| `exception_try_except.py` | Penanganan `ZeroDivisionError` secara terkendali menggunakan blok `try-except`. |
| `exception_multiple.py` | Penanganan berurutan untuk beberapa tipe *error* (`ValueError` dan `ZeroDivisionError`). |
| `exception_else_finally.py` | Alur lengkap `try-except-else-finally` untuk eksekusi sukses dan pembersihan akhir. |
| `exception_raise.py` | Pemicuan *exception* manual (`raise ValueError`) pada validasi fungsi `cek_umur()`. |

### 6. File Handling (`file-io`)
| Berkas | Deskripsi |
| :--- | :--- |
| `file_read.py` | Membaca seluruh isi berkas (`read()`) dan iterasi baris per baris (`strip()`) pada `data.txt`. |
| `file_write_append.py` | Menulis/menimpa berkas dengan mode `"w"` serta menambah baris di akhir dengan mode `"a"`. |
| `file_with_context.py` | Pengelolaan berkas aman menggunakan *context manager* `with open()` tanpa `close()` manual. |
| `file_handling_full.py` | Alur lengkap tulis (`"w"`), tambah (`"a"`), dan baca (`"r"`) pada berkas `contoh.txt`. |

### 7. Modules & Packages (`modules` & `packages`)
| Berkas / Direktori | Deskripsi |
| :--- | :--- |
| `matematika.py` & `main.py` | Pembuatan modul kustom (`tambah`, `kali`) dan pemanggilan dasar menggunakan `import`. |
| `module_alias.py` | Mengimpor modul dengan nama alias singkat (`import matematika as m`). |
| `module_from_import.py` | Mengimpor fungsi spesifik secara langsung (`from matematika import tambah`). |
| `module_builtin_math.py` | Pemanfaatan modul bawaan Python `math` (`math.sqrt` dan `math.pi`). |
| `my_package/` | Direktori paket berisi `__init__.py`, modul `operasi.py` (`kurang`), dan `geometri.py` (`luas_persegi`). |
| `package_import_modules.py` | Mengimpor modul `operasi` dan `geometri` dari dalam `my_package`. |
| `package_import_functions.py` | Mengimpor fungsi spesifik langsung dari submodul di dalam `my_package`. |
| `package_stdlib.py` | Penggunaan paket *Python Standard Library* (`os.getcwd()` dan `datetime.date.today()`). |

---

## Struktur Direktori

```text
.
├── assets/                          # Kumpulan screenshot output eksekusi terminal
├── my_package/                      # Contoh struktur Python package
│   ├── __init__.py
│   ├── operasi.py
│   └── geometri.py
├── func_*.py                        # Latihan Python Functions
├── list_operations.py               # Latihan struktur data List, Tuple, Set
├── tuple_operations.py
├── set_operations.py
├── dict_*.py                        # Latihan struktur data Dictionary
├── oop_*.py                         # Latihan dasar OOP & Encapsulation
├── access_modifiers.py
├── bank_account_encapsulation.py
├── inheritance_*.py                 # Latihan Inheritance & super()
├── polymorphism_*.py                # Latihan Polymorphism
├── abstraction_*.py                 # Latihan Abstraction (abc)
├── exception_*.py                   # Latihan Exception Handling
├── file_*.py                        # Latihan File Handling (I/O)
├── matematika.py                    # Modul kustom & latihan import
├── main.py
├── module_*.py
├── package_*.py                     # Latihan penggunaan Package & Standard Library
└── README.md