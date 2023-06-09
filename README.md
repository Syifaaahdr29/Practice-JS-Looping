# **Practice-JS-Looping**
### by Syifa Hadiarti Aulia | FE 8

### Exercise Number 1
1. Kita sudah mengetahui bahwa banyaknya user maksimal adalah 100.
Buat sebuah program yang menampilkan teks ‘User ke - 1 … User ke - 100’ pada setiap baris di halaman HTML.
Lakukan FOR LOOP pada Javascript.

   **Jawaban :** [Practice1.html](https://github.com/Syifaaahdr29/Practice-JS-Looping/blob/master/Practice1.html)
   ```html
   <body>
      <div class="nama"> Syifa Hadiarti Aulia | FE 8 </div>
        <h3>Practice 1 JS Looping | List User</h3>
        <ul id="list"></ul>
      <script>
            const list = document.getElementById("list"); // mengambil elemen list
            let user = 100; // memasukkan nilai ke variabel user
            // perulangan jumlah user
            for (let i = 1; i <= 100; i++) {
                list.innerHTML += `<li>User ke : ${i}</li>`; //menampilkan urutan user
            };
      </script>
   </body>
   ```
   
### Exercise Number 2

2. Lakukan pengulangan menggunakan FOR LOOP untuk melakukan penambahan nilai sebanyak 10 kali.
    * Nilai awal = 0
    * Pengulangan = 10 kali
    * Nilai awal ditambah 2 setiap pengulangan
    * Tampilan hasil penambahan pada setiap pengulangan

   **Jawaban :** [Practice2.html](https://github.com/Syifaaahdr29/Practice-JS-Looping/blob/master/Practice2.html)
   ```html
   <script>
        let nilaiAwal = 0
        for (let i = 1; i <= 10; i++) { // perulangan sebanyak 10 kali
            nilaiAwal += 2; // menambah +2 setiap perulangan
            console.log(`perulangan ke ${i} \n nilai awal = ${nilaiAwal}`) // menampilkan perulangan dan jumlah nilai awal
        }
   </script>
   ```

### Exercise Number 3

3. Lakukan pengulangan dengan FOR LOOP yang melakukan iterasi dari 0..20.
    * Setiap iterasi/pengulangan lakukan pengecekan apakah nilai tersebut ganjil atau genap.
    * Tampilkan keterangan ganjil dan genap pada sebuah nilai setiap pengulangan

    **Jawaban :** [Practice3.html](https://github.com/Syifaaahdr29/Practice-JS-Looping/blob/master/Practice3.html)
    ```html
    <script>
        for (let i = 1; i <=20; i++) { // perulangan sebanyak 20 kali
            i % 2 == 0 ? console.log(`Perulangan ke ${i} adalah angka genap`) : console.log(`Perulangan ke ${i} adalah angka ganjil`);
        } // menentukan angka ganjil dan genap dari perulangan
    </script>
    ```
    
    
### Exercise Number 4

4. Tampilkan sebuah Konfirmasi Pop Up kepada user menggunakan confirm();
    * Berikan teks ‘Apakah anda mau mengulang’ pada box confirm
    * Jika user memilih ‘OK’ maka program akan terus menampilan pop up yang sama
    * Jika user memilih ‘Cancel’ maka program akan menampilkan teks ‘Perulangan sudah dilakukan sebanyak … (jumlah klik OK yang dilakukan user)

     **Jawaban :** [Practice4.html](https://github.com/Syifaaahdr29/Practice-JS-Looping/blob/master/Practice4.html)
     ```html
     <script>
        let looping = 0; // mendeklarasikan nilai awal perulangan 
        let again = true; // mendeklarasikan variable again 

        while (again) {
            looping++;
            let acc = confirm("Apakah anda ingin mengulang lagi? "); // konfirmasi untuk melakukan perulangan 
            acc == true ? (again = true) : (again = false); // validasi nilai variable acc
        }
        alert(`Perulangan telah dilakukan sebanyak : ${perulangan} kali`); // menampilkan jumlah perulangan
     </script>
     ```

### Exercise Number 5

5. Buat sebuah program kuis.
    * Tampilkan prompt() untuk meminta inputan dari user. Tampilan teks ‘Sebutkan kepanjangan dari nama IB (Impact Byte)?’
    * Lakukan pengecekan apakah jawaban dari user sudah benar
    * Jika benar, tampilkan alert ‘Selamat jawaban kamu benar’
    * Jika salah, lakukan pengulangan untuk menampilkan prompt() yg sama hingga jawaban dari user benar

     **Jawaban :** [Practice5.html](https://github.com/Syifaaahdr29/Practice-JS-Looping/blob/master/Practice5.html)
     
     ```html
     <script>
      let benar = true; // mendeklarasikan variable benar
      while (benar) { // kondisi ketika variable benar bernilai true
          let jawaban = prompt("Sebutkan kepanjangan dari nama IB? "); // menampilkan pop up dengan prompt
          jawaban = jawaban.toLowerCase(); // mengubah jawaban menjadi huruf kecil

          if (jawaban == "impact byte"){ 
              benar = false; // kalau jawaban benar maka akan keluar dari perulangan
          } else {
              alert("Jawabanmu Salah, silahkan jawab kembali "); // menampilkan jawaban salah
          }
      }
      alert("Selamat jawaban kamu benar!"); // alert jawaban benar dan keluar dari perulangan
     </script>
     ```
