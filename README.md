# **Practice-JS-Looping**
by Syifa Hadiarti Aulia | FE 8

**Exercise Number 1**
Soal : Kita sudah mengetahui bahwa banyaknya user maksimal adalah 100.
Buat sebuah program yang menampilkan teks ‘User ke - 1 … User ke - 100’ pada setiap baris di halaman HTML.
Lakukan FOR LOOP pada Javascript.

Jawaban : Tertera pada [Practice1.html](https://github.com/Syifaaahdr29/Practice-JS-Looping/blob/master/Practice1.html).

...<body>
        <div class="nama">Syifa Hadiarti Aulia | FE 8</div>
        <h3>Practice 1 JS Looping | List User</h3>
        <ul id="list"></ul>
        <script>
            // mengambil elemen list
            const list = document.getElementById("list");
            // memasukkan nilai ke variabel user
            let user = 100;
            // perulangan jumlah user
            for (let i = 1; i <= 100; i++) {
                list.innerHTML += `<li>User ke : ${i}</li>`; //menampilkan urutan user
            };
        </script>
    </body>
...



