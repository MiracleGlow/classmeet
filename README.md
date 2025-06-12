
---

## 1. Tantangan Utama

* **Eliminasi otomatis tanpa finish time**: Pemain yang gagal menjadi finisher di ronde 1 dan ronde 2 tidak memiliki finish time untuk diurut; mereka dieliminasi bersamaan oleh sistem game saat quota finishers terpenuhi.
* **Keinginan memberi poin sama**: Karena mereka dieliminasi bersamaan, wajar mempertimbangkan memberi poin identik kepada semua yang tereliminasi di ronde yang sama.
* **Risiko tie**: Jika semua eliminasi di ronde 1 mendapat poin sama, dan di ronde 2 pula sama, maka akumulasi poin tim berpotensi sama lebih sering. Kita perlu mekanisme tiebreak yang adil dan praktis supaya penentuan pemenang match tetap lancar.

---

## 2. Struktur Ronde dan Grup Eliminasi

* **Ronde 1 (Cannonball Chaos)**: Hanya 4 pemain tercepat finish dianggap “survivors”; sisanya (2 pemain peserta + spectator) dieliminasi otomatis tanpa finish time.

  * Survivor: 4 pemain yang berhasil finish.
  * Eliminated: 2 pemain yang tidak sempat finish karena quota 4 sudah terpenuhi + spectator (otomatis).
* **Ronde 2 (Super Slide)**: Hanya 2 pemain tercepat finish dianggap survivors; sisanya (2 pemain peserta tersisa) dieliminasi otomatis.

  * Survivor: 2 pemain yang berhasil finish.
  * Eliminated: 2 yang tidak sempat finish.
* **Ronde 3 (Block Dash Endless)**: Survival head-to-head antara 2 pemain; urutan jelas: pemenang (= bertahan lebih lama) dan runner-up.

Kita kelompokkan pemain berdasarkan ronde eliminasi:

* **Group E1**: Tereliminasi di ronde 1 (tidak finish).
* **Group E2**: Tereliminasi di ronde 2 (tidak finish).
* **Group R2**: Runner-up ronde 3.
* **Group R1**: Pemenang match (last man standing ronde 3).
* **Spectator** selalu dieliminasi di ronde 1 → termasuk Group E1 atau bisa diberi grup khusus dengan poin 0 (biasa dimasukkan ke E1 dengan poin 0 bila diinginkan).

---

## 3. Opsi Skema Poin dengan Grup yang Sama

Karena semua di E1 dieliminasi bersamaan tanpa urutan internal, dan sama di E2, kita bisa memberi poin **sama** untuk anggota grup yang sama. Contoh tabel poin (skema dasar):

| Grup Eliminasi / Status | Deskripsi                         | Poin Individu |
| ----------------------- | --------------------------------- | ------------: |
| R1 (Pemenang match)     | Last man standing di Ronde 3      |            10 |
| R2 (Runner-up match)    | Kalah di Ronde 3                  |             7 |
| E2 (elim ronde 2)       | Tidak finish di ronde 2           |             3 |
| E1 (elim ronde 1)       | Tidak finish di ronde 1           |             1 |
| Spectator               | (otomatis dieliminasi di ronde 1) |           0\* |

> Keterangan:
>
> * Angka 10, 7, 3, 1 hanyalah contoh. Yang penting:
>
>   * Jarak poin antara grup besar (pemenang vs runner-up) lebih besar untuk memberi insentif kuat menang ronde akhir.
>   * Jarak antara E2 vs E1 cukup jelas (misal 3 vs 1) supaya tim dengan anggota yang sampai ronde 2 tetap diunggulkan.
>   * Spectator biasanya tidak ikut penilaian tim, tapi jika perlu dimasukkan, beri 0 sehingga tidak menambah poin tim mana pun.
> * Skema angka lain bisa: 8-5-2-0, atau 7-5-2-0; intinya R1 > R2 > E2 > E1. Pastikan spread (selisih) meminimalkan tie, tapi tidak terlalu besar sehingga tim dengan satu pemenang match tidak otomatis menang mutlak jika anggota lain gagal total—meski seringnya pemenang match kuat.

---

## 4. Mekanisme Penghitungan dan Risiko Tie

1. **Hitung total poin tim**: Setelah match selesai, kita tahu siapa yang masuk grup mana (R1, R2, E2, E1). Untuk tiap anggota tim, ambil poin sesuai tabel, jumlahkan → Total Poin Tim A vs Tim B.

2. **Kemungkinan tie**:

   * Misal Tim A anggotanya: satu sampai R2 (runner-up), dua di E1 → total = 7 + 1 + 1 = 9.
     Tim B: satu sampai R1, dua di E2 → total = 10 + 3 + 3 = 16. Tidak tie.
   * Namun mungkin: Tim A: satu R1 + dua E1 = 10 + 1 + 1 = 12; Tim B: tiga di E2 = 3+3+3 = 9. Tidak tie.
   * Contoh tie: Tim A: satu R2 + dua E2 = 7 + 3 + 3 = 13; Tim B: satu R1 + dua E1 = 10 + 1 + 1 = 12. (bukan tie).
   * Namun kombinasi skema angka tertentu bisa mengakibatkan tie. Misal skema 7-5-2-0: Tim A satu R2 + dua E2 = 5+2+2 = 9; Tim B satu R1 + dua E1 = 7+0+0 = 7. Tidak tie. Sulit tie? Mungkin jarang, tapi bisa jika skema angka kurang cermat.
   * Jika skema: 7-5-2-1: Tim A: satu R2 + dua E1 = 5+1+1 = 7; Tim B: tiga E2? Tidak mungkin karena hanya 2 slot sampai ronde 2 survive. Umumnya tie lebih mungkin jika paduan anggota terdistribusi.
   * **Namun**: walau grup poin sama untuk E1/E2, masih ada variasi jumlah anggota yang masuk ke grup di tiap tim, sehingga seringnya total berbeda. Tie mungkin jarang tapi bisa terjadi jika misalnya:

     * Skema angka memungkinkan kombinasi: (R2 + E1 + E1) vs (E2 + E2 + R1) menghasilkan angka sama? Bisa terhindar dengan memilih selisih angka yang tepat.

3. **Tips memilih angka untuk meminimalkan tie**:

   * Pilih jarak yang tidak mudah dijumlah sama dengan kombinasi lain. Contoh: R1=10, R2=7, E2=3, E1=1.

     * Kombinasi Tim A: R2 + 2×E2 = 7 + 3 + 3 = 13.
       Kombinasi Tim B: R1 + 2×E1 = 10 + 1 + 1 = 12. Bukan tie.
     * Cek kombinasi lain: 2×R2 + E1 = 2×7 + 1 = 15; R1 + E2 + E1 = 10 + 3 + 1 = 14. Selisih.
     * Sulit cari kombinasi yang exact sama. Dengan angka ini, tie jarang bahkan nyaris tidak terjadi karena E1 poin 1 (bukan 0), E2 3 (bukan 2), R2 7 (bukan 5), R1 10 (bukan 8).
   * Anda bisa mencoba beberapa skema sederhana di spreadsheet untuk memastikan tidak ada kombinasi “jumlah poin sama” antar distribusi (misal: satu tim: satu sampai R2 + dua E2 vs tim lain: satu sampai R1 + dua E1).

4. **Tie-breaker**
   Walaupun skema angka baik, tetap siapkan prosedur tie-break cepat:

   * **Tie-break utama**: Lihat siapa tim yang punya anggota di R1 atau R2:

     * Jika salah satu tim memiliki pemenang match (R1) sementara tim lain tidak, pemenang match diprioritaskan (meski total poin sama, namun skema angka idealnya menghindari tie kalau R1 vs kombinasi lain).
     * Jika kedua tim sama-sama tidak punya R1, tapi satu tim punya runner-up (R2) sementara tim lain tidak, runner-up diunggulkan.
   * **Tie-break sekunder** (jika misalnya kedua tim punya status anggota identik, misal sama-sama satu anggota di R2 dan sisanya di E1/E2 sehingga poin benar-benar sama):

     * Lihat jumlah “survivors” di ronde 1: di ronde 1 ada 4 survivors. Cek berapa anggota masing-masing tim masuk ke ronde 2. Tim dengan lebih banyak anggota di ronde 2 dianggap unggul.
     * Jika sama, lihat jumlah anggota yang masuk ke ronde 3 (idealnya kalau ada 2 survivors ronde 2, tapi mungkin kedua survivors berasal dari tim yang sama? Maka tim lainnya tak punya; namun kombinasi ini jarang tie jika skema poin benar).
     * Jika masih sama (misalnya satu anggota tiap tim ke ronde 2, sisanya tereliminasi di ronde 1), bisa adakan mini-match tie-breaker 1 vs 1 di map singkat (misal survival kecil atau race singkat).
   * Dengan memilih skema angka yang baik, kemungkinan tie sangat kecil. Namun prosedur tie-break tetap disiapkan agar match tidak terhenti lama.

---

## 5. Contoh Skema Poin dan Ilustrasi

### 5.1. Pilih Skema

Misal kita pilih:

* **R1 (pemenang match)**: 10 poin
* **R2 (runner-up match)**: 7 poin
* **E2 (elim ronde 2)**: 3 poin
* **E1 (elim ronde 1)**: 1 poin
* **Spectator**: 0 poin (tidak menambah tim).
  (Catatan: Anda juga bisa set spectator 1 poin, tetapi bila spectator dianggap bukan bagian tim, biasanya diabaikan.)

### 5.2. Ilustrasi Hasil Match

Misal Tim A: A1, A2, A3; Tim B: B1, B2, B3.

* Setelah ronde 1: 4 survivors; misalnya survivors adalah A1, B1, B2, A2. Jadi A3 & B3 dieliminasi ronde 1.

  * A3, B3 → E1 → masing-masing 1 poin.
* Ronde 2: 2 survivors finish: misal finishers: B1, A2. Jadi B2 & A1 dieliminasi ronde 2.

  * B2, A1 → E2 → masing-masing 3 poin.
* Ronde 3: head-to-head antara B1 vs A2: misal B1 menang, A2 runner-up.

  * B1 → R1 → 10 poin; A2 → R2 → 7 poin.

Hitung total:

* **Tim A**: anggota A1(E2)=3 + A2(R2)=7 + A3(E1)=1 → total = 11.
* **Tim B**: anggota B1(R1)=10 + B2(E2)=3 + B3(E1)=1 → total = 14.
  Tim B menang match.

Cek potensi tie:

* Kombinasi lain: misal Tim A: satu R2 + dua E2 = 7 + 3 + 3 = 13; Tim B: satu R1 + dua E1 = 10 + 1 + 1 = 12 → tidak tie.
* Sulit cari kombinasi total sama:

  * R1 + E1 + E2 = 10 + 1 + 3 = 14
  * R2 + E2 + E1 = 7 + 3 + 1 = 11
  * 3×E2 tidak mungkin karena maksimal 2 survivals dari ronde 1 ke 2.
  * Dsb.
    Jadi tie sangat kecil kemungkinannya.

### 5.3. Jika Tie Terjadi (Sangat Jarang)

Misalkan terjadi kombinasi aneh yang menghasilkan total sama:

* Gunakan tie-breaker:

  1. Periksa apakah salah satu tim memiliki anggota di R1 (pemenang match). Tim dengan pemenang unggul.
  2. Jika tidak ada pemenang match di salah satu tim (misal kedua tim tidak punya R1), periksa runner-up (R2).
  3. Jika tetap sama, periksa jumlah anggota yang sampai ronde 2 (survivors ronde 1). Tim dengan lebih banyak survivors ronde 1 diunggulkan.
  4. Jika masih sama, mini-match 1 vs 1 di map singkat.

---

## 6. Penjelasan Langkah Pencatatan untuk Panitia

1. **Ronde 1**:

   * Jalankan map Cannonball Chaos. Sistem game otomatis menyingkirkan pemain setelah quota 4 finishers terpenuhi; sisanya dieliminasi otomatis (tanpa finish time).
   * Catat siapa 4 finishers (nama), siapa 2 yang gagal finish, dan spectator.
   * Tandai grup: finishers → lanjut ronde 2; gagal finish → E1.
2. **Ronde 2**:

   * Jalankan map Super Slide dengan 4 survivors. Sistem game menyingkirkan setelah quota 2 finishers terpenuhi; sisanya dieliminasi otomatis.
   * Catat 2 finishers → lanjut ronde 3; 2 gagal finish → E2.
3. **Ronde 3**:

   * Jalankan map Block Dash Endless dengan 2 survivors. Catat siapa bertahan lebih lama (pemenang match R1) dan siapa runner-up (R2).
4. **Konversi ke Poin**:

   * Untuk masing-masing pemain, tentukan grup (R1/R2/E2/E1) dan ambil poin sesuai tabel skema yang sudah disepakati (contoh 10-7-3-1).
   * Jika spectator dianggap, berikan 0 atau abaikan dalam penjumlahan tim.
5. **Hitung Total Poin Tim**:

   * Jumlahkan poin ketiga anggota tim → Total Poin Tim.
6. **Tentukan Pemenang Match**:

   * Bandingkan Total Poin Tim A vs Tim B.
   * Jika berbeda → Tim dengan poin lebih tinggi menang.
   * Jika sama → gunakan tie-breaker sesuai prosedur (cek keberadaan R1, R2, jumlah survivors ronde 1, atau mini-match).
7. **Dokumentasi**:

   * Sediakan template sederhana (spreadsheet atau kertas formulir) dengan kolom: Nama, Tim, Status Ronde (survivor/elim), Grup (E1/E2/R2/R1), Poin, Total poin tim.
   * Setelah match selesai, panitia hitung bersama untuk transparansi.

---

## 7. Tips untuk Mengurangi Ambiguitas

* **Pengumuman di awal match**: Jelaskan singkat ke peserta bahwa:

  * Di ronde 1 & 2, hanya sejumlah finisers diperhitungkan; sisanya dieliminasi bersamaan.
  * Semua yang dieliminasi di ronde yang sama akan mendapat poin identik sesuai grup.
  * Di ronde 3, head-to-head survival: pemenang mendapat poin tertinggi, runner-up poin kedua.
  * Pemenang match ditentukan dari total poin ketiga anggota tim; tie-breaker disiapkan.
* **Spectator**: Pastikan spectator tahu ia dieliminasi ronde 1; biasanya diberi poin 0.
* **Pemilihan skema angka**: Putuskan skema poin (misal 10-7-3-1) sebelum turnamen, informasikan panitia, cek di contoh skenario bahwa kombinasi poin jarang menghasilkan tie. Jika ingin lebih aman, bisa coba simulasi beberapa kombinasi distribusi anggota di spreadsheet sederhana: possible grup distribusi per tim di match 3 vs 3.
* **Tie-breaker**: Meskipun jarang, siapkan aturan jelas dan singkat sehingga panitia/peserta tidak bingung jika muncul tie (cek keberadaan pemenang match di tim, atau mini-match 1v1 jika perlu).
* **Pencatatan Manual vs Otomatis**: Karena tidak ada finish time untuk yang gagal finish, panitia hanya mencatat siapa finishers dan siapa tidak. Itu memudahkan pencatatan. Tidak perlu mencatat waktu bagi yang gagal finish.
* **Contoh Template Pencatatan**:

  | Nama                                                                      | Tim | Ronde Eliminasi        | Grup        | Poin |
  | ------------------------------------------------------------------------- | --- | ---------------------- | ----------- | ---- |
  | A1                                                                        | A   | Ronde 2 gagal finish   | E2          | 3    |
  | A2                                                                        | A   | Ronde 3 runner-up      | R2          | 7    |
  | A3                                                                        | A   | Ronde 1 gagal finish   | E1          | 1    |
  | B1                                                                        | B   | Ronde 3 pemenang match | R1          | 10   |
  | B2                                                                        | B   | Ronde 1 gagal finish   | E1          | 1    |
  | B3                                                                        | B   | Ronde 2 gagal finish   | E2          | 3    |
  | S                                                                         | —   | Ronde 1 (spectator)    | – atau E1\* | 0    |
  | Lalu hitung total tim A = 3+7+1 = 11; tim B = 10+1+3 = 14 → Tim B menang. |     |                        |             |      |

---

## 8. Ringkasannya

1. **Poin sama untuk eliminasi di ronde yang sama**: Ya, bisa. Semua yang gagal finish di ronde 1 (Group E1) dapat poin identik; semua gagal finish ronde 2 (Group E2) dapat poin identik.
2. **Tetapkan skema poin**: Misalnya R1=10, R2=7, E2=3, E1=1, Spectator=0. Pilih jarak angka agar kombinasi distribusi anggota tim sulit menghasilkan tie.
3. **Tie-breaker**:

   * Utama: keberadaan anggota di R1 atau R2 di salah satu tim.
   * Sekunder: jumlah survivors dari ronde sebelumnya (misal, berapa anggota tim yang sampai ronde 2).
   * Jika masih sama, mini-match 1 vs 1.
4. **Pencatatan mudah**: Cukup catat siapa finishers di ronde 1 & 2, siapa runners di ronde 3; lalu konversi grup ke poin dan jumlahkan.
5. **Komunikasi transparan**: Beri tahu peserta dan panitia mekanisme ini agar semua paham bahwa eliminasi bersama mendapat poin sama, dan bagaimana tie diatasi.

Dengan skema ini, perhitungan poin menjadi sederhana dan sesuai kondisi “tidak ada finish time untuk yang gagal finish”: semua yang gagal finish di ronde yang sama mendapat poin identik; pembedaan poin terutama hanya terjadi antar grup ronde (E1 vs E2 vs R2 vs R1). Pastikan spread poin cukup agar total tim berbeda di mayoritas kasus, dan siapkan tie-breaker praktis untuk situasi amat jarang tie.

Semoga revisi skema ini membantu, serta memudahkan panitia dan peserta memahami perhitungan poin match Stumble Guys pada classmeet. Selamat menyelenggarakan turnamen!
