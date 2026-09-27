
| Berkas | Jenis kesalahan | Pesan yang muncul (baris pertama) | Cara kamu mengetahuinya |
|---|---|---|---|
| `k1_sintaks.cpp` | Sintaks | `error: expected ',' or ';' before 'std'` | Build gagal pada tahap compile karena ada tanda titik koma (`;`) yang hilang setelah deklarasi `int nilai = 80`. |
| `k2_nama.cpp` | Nama/identifier | `error: 'Nilai' was not declared in this scope` | Compiler menunjukkan bahwa `Nilai` belum pernah dideklarasikan. C++ membedakan huruf besar dan kecil sehingga `Nilai` berbeda dari `nilai`. |
| `k3_runtime.cpp` | Runtime | Tidak ada pesan compiler/error saat build | Program berhasil di-build, tetapi ketika dijalankan dengan input `0`, terjadi masalah saat pembagian dengan nol. |
| `k4_logika.cpp` | Logika | Tidak ada pesan compiler/error | Program berhasil di-build dan berjalan, tetapi hasil rata-rata salah karena pembagian bilangan bulat. |

Menurut saya, kesalahan runtime paling berbahaya karena program dapat terlihat berhasil saat di-build, tetapi masalah baru muncul ketika program digunakan dengan kondisi tertentu.