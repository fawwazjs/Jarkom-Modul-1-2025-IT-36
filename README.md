# Laporan Resmi Jarkom Modul 1 Kelompok K-36

## Anggota

| Nama 				| NRP		|
|-------------------------------|---------------|
| Ahmad Wildan Fawwaz		| 5027241001 	|
| Muhammad Rakha Hananditya R.	| 5027241015 	|

## Pendahuluan

بِسْمِ اللَّهِ الرَّحْمَنِ الرَّحِيْمِ

<p align="justify">
&emsp; Segala puji syukur kita panjatkan atas kehadirat Allah Subḥānahu wa Ta‘ālā, karena berkat atas rahmat, karunia, dan nikmat-Nya praktikum modul 1 untuk mata kuliah Komunikasi Data dan Jaringan Komputer dapat diselesaikan dengan baik. Tidak lupa shalawat serta salam semoga senantiasa tercurah kepada junjungan kita Nabi Muhammad Shallallāhu ‘alaihi wa Sallam, suri teladan terbaik bagi umat manusia, beserta keluarga, sahabat, dan para pengikutnya hingga akhir zaman.
</p>

<p align="justify">
&emsp; Laporan ini disusun sebagai suatu bentuk pertanggungjawaban akademik atas kegiatan praktikum yang telah dilaksanakan. Selain itu, laporan ini berfungsi sebagai dokumentasi resmi tertulis dari seluruh rangkaian kegiatan yang telah dilakukan, sehingga dapat menjadi acuan dalam evaluasi maupun penilaian praktikum.
</p>

Rasulullah Shallallāhu ‘alaihi wa Sallam pernah bersabda:

إِذَا مَاتَ ابْنُ آدَمَ انْقَطَعَ عَمَلُهُ إِلَّا مِنْ ثَلَاثٍ: صَدَقَةٍ جَارِيَةٍ، أَوْ عِلْمٍ يُنْتَفَعُ بِهِ، أَوْ وَلَدٍ صَالِحٍ يَدْعُو لَهُ


<em>Artinya</em>:
<p align="justify">  
"Apabila anak Adam meninggal dunia, maka terputuslah amalnya kecuali tiga perkara: sedekah jariyah, ilmu yang bermanfaat, atau anak shalih yang mendoakannya." 
  
(HR. Muslim, no. 1631)
</p>
  
<p align="justify">
&emsp; Maka dari itu, semoga apa yang tertulis pada laporan ini dapat menjadi ilmu yang bermanfaat, serta menjadi keberkahan dan amal yang diterima di sisi Allah Subḥānahu wa Ta‘ālā. Semoga bagi yang membaca ini, Allah memudahkan semua langkahnya dalam menuntut ilmu, mengamalkannya, serta menjaganya agar tidak sekadar menjadi hafalan, namun juga menjadi bekal yang membawanya ke surga.
</p>

Āmīn yā Rabbal ‘ālamīn.

## Walkthrough

### • Soal 1

<blockquote>
  <ol>
    <li>
      <p align="justify">
	      Untuk mempersiapkan pembuatan entitas selain mereka, Eru yang berperan sebagai Router membuat dua Switch/Gateway. Dimana Switch 1 akan menuju ke dua Ainur yaitu Melkor dan Manwe. Sedangkan Switch 2 akan menuju ke dua Ainur lainnya yaitu Varda dan Ulmo. Keempat Ainur tersebut diberi perintah oleh Eru untuk menjadi Client.
      </p>
    </li>
  </ol>
</blockquote>
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/1bae475a-4649-471d-844a-324b700c1b92" />

### • Soal 2

<blockquote>
    <ol start="2">
        <li>
            <p align="justify">Karena menurut Eru pada saat itu Arda (Bumi) masih terisolasi dengan dunia luar, maka buat agar Eru dapat tersambung ke internet.
	    </p>
        </li>
    </ol>
</blockquote>

Melakukan   
```bash
ping google.com -c 3
``` 
ke Eru
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/65761b8f-dd93-44e6-b4c6-0dc9760fbeee" />

### • Soal 3

<blockquote>
    <ol start="3">
        <li>
            <p align="justify">Sekarang pastikan agar setiap Ainur (Client) dapat terhubung satu sama lain.
	    </p>
        </li>
    </ol>
</blockquote>

Melakukan deteksi IP nodes dengan menggunakan
```bash
ip a
```
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/d46ed041-9d0b-49e0-a781-2fe9e399ee19" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/abe7e0a6-247c-4eb3-84ae-2e3296498943" />
Lalu setelah menemukan IP dari nodes dapat melakukan ping:
```bash
ping [IP Ainur] -c 3   
```   
ke masing-masing Ainur (Melkor, Manwe, Varda, Ulmo) dan masing-masing Ainur melakukan ping IP dengan Ainur lainnya.
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/fc8952e9-4e99-40eb-9452-0dfc7362a355" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/f76e1dc0-15ec-4c86-aebc-80e61169b0db" />


### • Soal 4
<blockquote>
    <ol start="4">
        <li>
            <p align="justify">Setelah berhasil terhubung, sekarang Eru ingin agar setiap Ainur (Client) dapat mandiri. Oleh karena itu pastikan agar setiap Client dapat tersambung ke internet.
	    </p>
        </li>
    </ol>
</blockquote>

### • Soal 5

<blockquote>
    <ol start="5">
        <li>
            <p align="justify">Ainur terkuat Melkor tetap berusaha untuk menanamkan kejahatan ke dalam Arda (Bumi). Sebelum terjadi kerusakan, Eru dan para Ainur lainnya meminta agar semua konfigurasi tidak hilang saat semua node di restart.
	    </p>
        </li>
    </ol>
</blockquote>

Melakukan edit configurasi network pada masing2 node

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/4f54fba4-6ced-42ec-bbcc-bb049f9343b4" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/8b597da8-fb5a-4b51-b323-2f89937b1356" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/a18d793e-08e5-4e2b-a797-6b5385d90bd5" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/d0bed738-6a74-4948-a7b6-bead088cf4b2" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/da6bbdd6-ea41-4d41-b03e-058d44e31bae" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/ac0dc180-e087-4768-b584-af2b045522ba" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/97d54ff3-45ae-4726-a6b3-84d18e0d696a" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/f13b0cfa-dc3e-44ab-b2be-f8d81bffebcb" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/9d632dbd-d0a8-40c3-93d5-62e8ec640301" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/b9d4c69a-bc8b-4018-a6a5-b6576ae0ecfc" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/f770e236-a76b-448c-9dce-01f8e72342db" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/20e82c8f-b388-42e3-bfa6-c9645f44d2a2" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/ae23ec34-9daf-49b3-835d-5c14904056c9" />

Lalu lakukan penambahan kode pada masing node.
Di terminal, ketik
```bash
nano /root/.bashrc
```
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/aea1e767-01f5-4651-abfc-27f3a6f54650" />
tambahkan di bagian bawah bertanda # seperti gambar

```bash
apt update && apt install -y iptables
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.229.0.0/16
echo nameserver 192.168.122.1 > /etc/resolv.conf
```

### • Soal 6

<blockquote>
    <ol start="6">
        <li>
            <p align="justify">Setelah semua Ainur terhubung ke internet, Melkor mencoba menyusup ke dalam komunikasi antara Manwe dan Eru. Jalankan file berikut (link file) lalu lakukan packet sniffing menggunakan Wireshark pada koneksi antara Manwe dan Eru, lalu terapkan display filter untuk menampilkan semua paket yang berasal dari atau menuju ke IP Address Manwe. Simpan hasil capture tersebut sebagai bukti.
	    </p>
        </li>
    </ol>
</blockquote>
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/27af889c-127c-4457-a819-6ae33c77e2ff" />

### • Soal 7

<blockquote>
    <ol start="7">
        <li>
            <p align="justify">Untuk meningkatkan keamanan, Eru memutuskan untuk membuat sebuah FTP Server di node miliknya. Lakukan konfigurasi FTP Server pada node Eru. Buat dua user baru: ainur dengan hak akses write &amp; read dan melkor tanpa hak akses sama sekali ke direktori shared. Buktikan hasil tersebut dengan membuat file teks sederhana kemudian akses file tersebut menggunakan kedua user.
	    </p>
        </li>
    </ol>
</blockquote>

### • Soal 8

<blockquote>
    <ol start="8">
        <li>
            <p align="justify">Ulmo, sebagai penjaga perairan, perlu mengirimkan data ramalan cuaca ke node Eru. Lakukan koneksi sebagai client dari node Ulmo ke FTP Server Eru menggunakan user ainur. Upload sebuah file berikut (link file). Analisis proses ini menggunakan Wireshark dan identifikasi perintah FTP yang digunakan untuk proses upload.
	    </p>
        </li>
    </ol>
</blockquote>

### • Soal 9

<blockquote>
    <ol start="9">
        <li>
            <p align="justify">Eru ingin membagikan "Kitab Penciptaan" di (link file) kepada Manwe. Dari FTP Server Eru, download file tersebut ke node Manwe. Karena Eru merasa Kitab tersebut sangat penting maka ia mengubah akses user ainur menjadi read-only. Gunakan Wireshark untuk memonitor koneksi, identifikasi perintah FTP yang digunakan, dan uji akses user ainur.
	    </p>
        </li>
    </ol>
</blockquote>

### • Soal 10

<blockquote>
    <ol start="10">
        <li>
            <p align="justify">Melkor yang marah karena tidak diberi akses, mencoba melakukan serangan dengan mengirimkan banyak sekali request ke server Eru. Gunakan command ping dari node Melkor ke node Eru dengan jumlah paket yang tidak biasa (spam ping misalnya 100 paket). Amati hasilnya, apakah ada packet loss? Catat average round trip time untuk melihat apakah serangan tersebut mempengaruhi kinerja Eru.
	    </p>
        </li>
    </ol>
</blockquote>

### • Soal 11

<blockquote>
    <ol start="11">
        <li>
            <p align="justify">Sebelum era koneksi aman, Eru sering menyelinap masuk ke wilayah Melkor. Eru perlu masuk ke node tersebut untuk memeriksa konfigurasi, namun ia tahu Melkor mungkin sedang memantau jaringan. Buktikan kelemahan protokol Telnet dengan membuat akun dan password baru di node Melkor kemudian menangkap sesi login Eru ke node Melkor menggunakan Wireshark. Tunjukkan bagaimana username dan password dapat terlihat sebagai plain text.
	    </p>
        </li>
    </ol>
</blockquote>

### • Soal 12

<blockquote>
    <ol start="12">
        <li>
            <p align="justify">Eru mencurigai Melkor menjalankan beberapa layanan terlarang di node-nya. Lakukan pemindaian port sederhana dari node Eru ke node Melkor menggunakan Netcat (nc) untuk memeriksa port 21, 80, dalam keadaan terbuka dan port rahasia 666 dalam keadaan tertutup.
	    </p>
        </li>
    </ol>
</blockquote>

### • Soal 13

<blockquote>
    <ol start="13">
        <li>
            <p align="justify">Setelah insiden penyadapan Telnet, Eru memerintahkan semua koneksi administratif harus menggunakan SSH (Secure Shell) untuk mengamankan jaringan. Lakukan koneksi SSH dari node Varda ke Eru. Tangkap sesi tersebut menggunakan Wireshark. Analisis dan jelaskan mengapa username dan password tidak dapat dilihat seperti pada sesi Telnet. Tunjukkan paket-paket terenkripsi dalam hasil capture sebagai bukti keamanan SSH.
	    </p>
        </li>
    </ol>
</blockquote>

### • Soal 14

<blockquote>
    <ol start="14">
        <li>
            <p align="justify">Setelah gagal mengakses FTP, Melkor melancarkan serangan brute force terhadap Manwe. Analisis file capture yang disediakan dan identifikasi upaya brute force Melkor.
	    </p>
        </li>
    </ol>
</blockquote>

```bash
nc 10.15.43.32 3401

===== Soal 14 =====
Difficulty: Easy
Note: You can exit anytime by typing 'exit'

How many packets are recorded in the pcapng file?
Format: int
> 500358

What are the user that successfully logged in?
Format: user:pass
> n1enna:y4v4nn4_k3m3nt4r1

In which stream were the credentials found?
Format: int
> 41824

What tools are used for brute force?
Format: Hydra v1.8.0-dev
> Fuzz Faster U Fool v2.1.0-dev
Congratulations! Here is your flag: KOMJAR25{Brut3_F0rc3_LlP4CsiExCnDT7yPEZP3GTJhX}
```

#### • Soal 14.a: How many packets are recorded in the pcapng file?

<p align="justify">
&emsp; Untuk mengetahui jumlah paket yang ditangkap dari suatu file PCAP, maka kita dapat melihatnya dengan beralih ke menu <code>Statistics > Capture File Properties</code>.
</p>

<p align="center">
	<img src="https://github.com/user-attachments/assets/d29f9533-d028-4aea-9be9-b60f35285d74" alt="a" width="80%" height="80%">  
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya terdapat <b>500358</b> paket yang tertangkap pada file PCAP <code>shortbf.pcapng</code>.
</p>

#### • Soal 14.b: What are the user that successfully logged in?

<p align="justify">
&emsp; Sebelum kita dapat mengetahui user mana yang berhasil login, maka kita perlu terlebih dahulu mengetahui protokol apa yang digunakan untuk mengirim data user tersebut pada jaringan. Hal ini dapat dilakukan dengan beralih ke menu <code>Statistics > Protocol Hierarchy</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="b" src="https://github.com/user-attachments/assets/76d06e74-2efb-4311-991d-3b5e2ebd4d78">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya mayoritas paket yang ditangkap pada file PCAP menggunakan protokol <b>HTTP</b>.
</p>

<p align="justify">
&emsp; Selain itu, dalam proses request untuk login, maka server akan mengembalikan respon berdasarkan valid atau tidaknya kredensial yang diberikan selama proses login dalam bentuk suatu paket. Kita bisa melihat paket dengan kriteria tersebut dengan menggunakan display filter yaitu <code>http.response</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="c" src="https://github.com/user-attachments/assets/fb06c33a-737a-4c21-a10c-b4a4a980285b">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dengan memperhatikan detail dari mayoritas paket yang ditampilkan, khususnya pada bagian <code>Line-based text data</code>, server akan merespon dengan <b>Invalid credentials</b>. Hal ini menandakan bahwasannya tidak semua percobaan login yang dilakukan oleh client berhasil.
</p>

<p align="justify">
&emsp; Maka dari itu, untuk mencari paket di mana client berhasil masuk, kita dapat menambahkan display filter berupa <code>!data-text-lines contains "Invalid credentials"</code>. Sehingga secara keseluruhan, display filter yang digunakan adalah <code>http.response && !data-text-lines contains "Invalid credentials"</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="d" src="https://github.com/user-attachments/assets/c05df4bd-cb8a-464a-884f-67f5128efb0d">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya paket pada frame <b>500320</b> menunjukkan keberhasilan login yang dilakukan oleh client.
</p>

<p align="justify">
&emsp; Sehingga, untuk mengetahui secara definitif data terkait username dan password yang digunakan untuk login, kita bisa beralih ke paket request yang direspon oleh frame 500320, yaitu paket pada frame <b>500315</b> dengan cara menggunakan menu <code>Go > Go to Packet... > 500315</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="e" src="https://github.com/user-attachments/assets/6abc8840-599d-4dc4-a00f-1373eaea0491">
</p>

<p align="justify">
&emsp; Setelah mendapatkan paket request dari client, maka langkah selanjutnya adalah untuk membuka <b>stream HTTP</b> dari paket tersebut melalui menu <code>Follow > HTTP Stream</code> dan menampilkan stream dalam bentuk ASCII.
</p>

<p align="center">
	<img width="80%" height="80%" alt="f" src="https://github.com/user-attachments/assets/94dbc523-a645-4889-b38d-401365ff07c7">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya username yang berhasil digunakan untuk login adalah <b>n1enna</b> dengan password <b>y4v4nn4_k3m3nt4r1</b>.
</p>

#### • Soal 14.c: In which stream were the credentials found?

<p align="justify">
&emsp; Untuk mengetahui stream mana yang digunakan untuk membawa data username dan password, maka kita bisa melihat detail dari paket 500315, khususnya pada bagian <code>Transmission Control Protocol > Stream index</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="g" src="https://github.com/user-attachments/assets/bcab3d4d-8fb6-48a6-8605-ab2d06eb73f9">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya stream yang digunakan untuk membawa data username dan password adalah stream dengan indeks <b>41824</b>.
</p>

#### • Soal 14.d: What tools are used for brute force?

<p align="justify">
&emsp; Terakhir, untuk mengetahui tool yang digunakan client dalam proses brute force username dan password, maka kita bisa kembali melihat stream HTTP dari frame 500315, khususnya pada bagian <code>User-Agent</code>.
</p>

<p align="justify">
	<img width="80%" height="80%" alt="h" src="https://github.com/user-attachments/assets/a6079f88-2a21-48d4-91c9-c43274c59e98">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya tool yang digunakan untuk melakukan brute force username dan password adalah <b>Fuzz Faster U Fool v2.1.0-dev</b>.
</p>

### • Soal 15

<blockquote>
    <ol start="15">
        <li>
            <p align="justify">Melkor menyusup ke ruang server dan memasang keyboard USB berbahaya pada node Manwe. Buka file capture dan identifikasi pesan atau ketikan (keystrokes) yang berhasil dicuri oleh Melkor untuk menemukan password rahasia.
	    </p>
        </li>
    </ol>
</blockquote>

```bash
===== Soal 15 =====
Difficulty: Medium
Note: You can exit anytime by typing 'exit'

What device does Melkor use?
Format: string
> Keyboard

What did Melkor write?
Format: string
> UGx6X3ByMHYxZGVfeTB1cl91czNybjRtZV80bmRfcDRzc3cwcmQ=

What is Melkor's secret message?
Format: string
> Plz_pr0v1de_y0ur_us3rn4me_4nd_p4ssw0rd
Congratulations! Here is your flag: KOMJAR25{K3yb0ard_W4rr10r_QxBuvdKhn2ygOjGDBDhAjhPY3}
```

#### • Soal 15.a: What device does Melkor use?

<p align="justify">
Merujuk pada pernyataan yang ada pada soal 15, di mana:
</p>

<blockquote>
Melkor menyusup ke ruang server dan memasang <b><i>keyboard</i></b> USB berbahaya pada node Manwe.
</blockquote>

<p align="justify">
Berdasarkan pernyataan di atas, dapat disimpulkan bahwasannya, perangkat yang digunakan oleh Melkor adalah sebuah <b>keyboard</b>.
</p>

#### • Soal 15.b: What did Melkor write?

<p align="center">
	<img width="80%" height="80%" alt="aj" src="https://github.com/user-attachments/assets/b3cc3ea5-f2e7-4407-9c13-1f92ede7a7a6">
</p>

<p align="justify">
&emsp; Diketahui bahwasannya keypress dari sebuah keyboard direkam pada paket dengan flag <code>URB_INTERRUPT in</code>, data terkait keypress itu sendiri tertera pada detail paket <code>URB_INTERRUPT in</code> khususnya pada bagian <code>HID Data</code>, dan data keypress tersebut sendiri memiliki destinasi yaitu <b>host</b> atau hub sentral dari semua perangkat USB. Maka, kita dapat menggunakan display filter yaitu <code>usb.transfer_type == 0x01 && !usb.src == host</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="ak" src="https://github.com/user-attachments/assets/a8a67bed-b1b0-44a1-8193-8e68781615c6">
</p>

<p align="justify">
&emsp; Namun, mengambil data HID dari setiap paket akan memakan waktu yang sangat lama apabila dilakukan satu per satu. Oleh karena itu, kita dapat menggunakan command <code>tshark</code> atau Wireshark pada CLI untuk melakukan otomatisasi pengambilan data HID daris setiap paket yang sesuai dengan kriteria display filter. Di mana command lengkapnya adalah:
</p>

```sh
tshark -r /home/fedora/Downloads/hiddenmsg.pcapng -Y 'usb.transfer_type == 0x01 && !usb.src == host' -T fields -e usbhid.data
```

Di mana:
- `tshark`: Wireshark pada CLI.
- `-r /home/fedora/Downloads/hiddenmsg.pcapng`: file PCAP yang akan diekstraksi datanya.
- `-Y 'usb.transfer_type == 0x01 && !usb.src == host'`: display filter yang digunakan untuk mencari paket yang sesuai kriteria.
- `-T fields -e usbhid.data`: mengambil field HID data pada detail setiap paket.

<p align="justify">
Output dari command tersebut adalah:
</p>

```sh
0200000000000000
0200180000000000
0200000000000000
0000000000000000
0000000000000000
0200000000000000
02000a0000000000
0200000000000000
0000000000000000
0000000000000000
00001b0000000000
0000000000000000
0000000000000000
0000230000000000
0000000000000000
0000000000000000
0200000000000000
02001b0000000000
0200000000000000
0000000000000000
0000000000000000
0000200000000000
0000000000000000
0000000000000000
0200000000000000
0200050000000000
0200000000000000
0000000000000000
0000000000000000
00001c0000000000
0000000000000000
0000000000000000
0200000000000000
0200100000000000
0200000000000000
02000b0000000000
0200000000000000
02001c0000000000
0200000000000000
0000000000000000
0000000000000000
00001b0000000000
0000000000000000
0000000000000000
0200000000000000
02001d0000000000
0200000000000000
02000a0000000000
0200000000000000
0200190000000000
0200000000000000
0000000000000000
0000000000000000
0000090000000000
0000000000000000
0000000000000000
0000080000000000
0000000000000000
0000000000000000
0200000000000000
0200170000000000
0200000000000000
0200050000000000
0200000000000000
0000000000000000
0000000000000000
00001e0000000000
0000000000000000
0000000000000000
0000060000000000
0000000000000000
0000000000000000
00000f0000000000
0000000000000000
0000000000000000
0000260000000000
0000000000000000
0000000000000000
00001e0000000000
0000000000000000
0000000000000000
0000060000000000
0000000000000000
0000000000000000
00001d0000000000
0000000000000000
0000000000000000
0200000000000000
0200110000000000
0200000000000000
0000000000000000
0000000000000000
00001c0000000000
0000000000000000
0000000000000000
0000050000000000
0000000000000000
0000000000000000
00000d0000000000
0000000000000000
0000000000000000
0200000000000000
0200150000000000
0200000000000000
0000000000000000
0000000000000000
0000170000000000
0000000000000000
0000000000000000
0200000000000000
02001d0000000000
0200000000000000
0000000000000000
0000000000000000
0200000000000000
0200190000000000
0200000000000000
0000000000000000
0000000000000000
0000250000000000
0000000000000000
0000000000000000
0000270000000000
0000000000000000
0000000000000000
0000050000000000
0000000000000000
0000000000000000
0000100000000000
0000000000000000
0000000000000000
0200000000000000
0200150000000000
0200000000000000
0000000000000000
0000000000000000
0000090000000000
0000000000000000
0000000000000000
0000060000000000
0000000000000000
0000000000000000
0200000000000000
0200070000000000
0200000000000000
0000000000000000
0000000000000000
0200000000000000
0200150000000000
0200000000000000
0000000000000000
0000000000000000
00001d0000000000
0000000000000000
0000000000000000
0000060000000000
0000000000000000
0000000000000000
0000200000000000
0000000000000000
0000000000000000
0000060000000000
0000000000000000
0000000000000000
00001a0000000000
0000000000000000
0000000000000000
0000060000000000
0000000000000000
0000000000000000
0000100000000000
0000000000000000
0000000000000000
0200000000000000
0200140000000000
0200000000000000
0000000000000000
0000000000000000
00002e0000000000
0000000000000000
0000000000000000
```

<p align="justify">
&emsp; Namun, output heksadesimal di atas masih bersifat mentah dan sulit dibaca. Oleh karena itu, dibuatlah suatu program Python yang dapat menerjemahkan output tersebut. 
</p>

```py
#!/usr/bin/env python3
import sys

hidmap = {
    0x04: "a", 0x05: "b", 0x06: "c", 0x07: "d", 0x08: "e", 0x09: "f",
    0x0A: "g", 0x0B: "h", 0x0C: "i", 0x0D: "j", 0x0E: "k", 0x0F: "l",
    0x10: "m", 0x11: "n", 0x12: "o", 0x13: "p", 0x14: "q", 0x15: "r",
    0x16: "s", 0x17: "t", 0x18: "u", 0x19: "v", 0x1A: "w", 0x1B: "x",
    0x1C: "y", 0x1D: "z",
    0x1E: "1", 0x1F: "2", 0x20: "3", 0x21: "4", 0x22: "5",
    0x23: "6", 0x24: "7", 0x25: "8", 0x26: "9", 0x27: "0",
    0x28: "\n", 
    0x2C: " ", 
    0x2D: "-", 0x2E: "=", 0x2F: "[", 0x30: "]",
    0x33: ";", 0x34: "'", 0x36: ",", 0x37: ".", 0x38: "/",
}

def decode(keyhex):
    report = bytes.fromhex(keyhex)
    mod = report[0]
    keycodes = report[2:] 
    out = ""
    for keycode in keycodes:
        if keycode == 0: continue
        char = hidmap.get(keycode, f"[{keycode:02x}]")
        if mod & 0x02:
            char = char.upper()
        out += char
    return out

for line in sys.stdin:
    line = line.strip()
    if line:
        sys.stdout.write(decode(line))
```

<p align="justify">
&emsp; Sehingga outputnya menjadi <b>UGx6X3ByMHYxZGVfeTB1cl91czNybjRtZV80bmRfcDRzc3cwcmQ=</b>, di mana ini merupakan apa yang diketik oleh Melkor pada keyboard.
</p>

#### • Soal 15.c: What is Melkor's secret message?

<p align="justify">
&emsp; Diketahui bahwasannya output dari soal 15.b tersebut diakhiri dengan simbol <code>=</code>. Hal ini menyatakan bahwasannya kemungkinan besar output tersebut dienkode menggunakan metode enkode <b>Base64</b>. Di mana jika output tersebut dimasukkan sebagai input (pipe) ke dalam command <code>base64 --decode</code> akan menghasilkan string yaitu <b>Plz_pr0v1de_y0ur_us3rn4me_4nd_p4ssw0rd</b> yang merupakan pesan rahasia dari Melkor.
	
### • Soal 16

<blockquote>
    <ol start="16">
        <li>
            <p align="justify">Melkor semakin murka ia meletakkan file berbahaya di server milik Manwe. Dari file capture yang ada, identifikasi file apa yang diletakkan oleh Melkor.
	    </p>
        </li>
    </ol>
</blockquote>

```bash
nc 10.15.43.32 3403

===== Soal 16 =====
Difficulty: Hard
Note: You can exit anytime by typing 'exit'

What credential did the attacker use to log in?
Format: user:pass
> ind@psg420.com:{6r_6e#TfT1p                                       

How many files are suspected of containing malware?
Format: int
> 5

What is the hash of the first file (q.exe)?
Format: sha256
> ca34b0926cdc3242bbfad1c4a0b42cc2750d90db9a272d92cfb6cb7034d2a3bd

What is the hash of the second file (w.exe)?
Format: sha256
> 08eb941447078ef2c6ad8d91bb2f52256c09657ecd3d5344023edccf7291e9fc

What is the hash of the third file (e.exe)?
Format: sha256
> 32e1b3732cd779af1bf7730d0ec8a7a87a084319f6a0870dc7362a15ddbd3199

What is the hash of the fourth file (r.exe)?
Format: sha256
> 4ebd58007ee933a0a8348aee2922904a7110b7fb6a316b1c7fb2c6677e613884

What is the hash of the fifth file (t.exe)?
Format: sha256
> 10ce4b79180a2ddd924fdc95951d968191af2ee3b7dfc96dd6a5714dbeae613a
Congratulations! Here is your flag: KOMJAR25{Y0u_4r3_4_g00d_4nalyz3r_blETB2xtXYXJAS5ghgqZqxg8B}
```

#### • Soal 16.a: What credential did the attacker use to log in?

<p align="justify">
&emsp; Sebelum dapat mengetahui kredensial yang digunakan attacker (Melkor) untuk login, maka kita perlu terlebih dahulu mengetahui secara definitif protokol apa yang digunakan attacker (Melkor) untuk mengirim file malware. Hal ini dapat dilakukan dengan beralih ke menu <code>Statistics > Protocol Hierarchy</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="ab" src="https://github.com/user-attachments/assets/fae7acaf-d194-4de1-95f2-638edab03e5a">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya kemungkinan protokol yang digunakan untuk mengirim file malware adalah <b>FTP</b>.
</p>

<p align="justify">
&emsp; Selain melihat protokol yang digunakan, kita juga perlu mengetahui secara definitif IP address mana yang berinteraksi dengan file malware tersebut dengan cara beralih ke menu <code>Statistics > Conversations</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="ac" src="https://github.com/user-attachments/assets/045c20d2-8a68-4d50-934e-4d2696cdf22d">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya kemungkinan IP address yang berinteraksi dengan file malware dan bertindak sebagai client adalah IP address <b>10.6.13.102</b> dikarenakan IP address tersebut merupakan <b>IP privat</b>, IP address pertama yang <b>meminta request SYN</b> terhadap server, teserta jumlah bytes dari paket yang dia dapat dari IP address <b>216.55.163.106</b> yang abnormal dibandingkan dengan percakapannya dengan IP address lain. Maka, keseluruhan display filter yang digunakan adalah <code>ftp && ip.src == 10.6.13.102 && ip.dst == 216.55.163.106</code>
</p>

<p align="center">
	<img width="80%" height="80%" alt="ad" src="https://github.com/user-attachments/assets/58cfa04f-deb7-4cd3-a51f-a24a4fbe3e14">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya username yang digunakan untuk login adalah <b>ind@psg420.com</b> serta password yang berkaitan adalah <b>{6r_6e#TfT1p</b>.
</p>

#### • Soal 16.b: How many files are suspected of containing malware?

<p align="justify">
&emsp; Untuk mendapatkan jumlah file yang memuat malware, maka kita dapat menambahkan display filter <code>&& ftp.request.command == "RETR"</code> pada filter yang sudah ada. Hal ini dikarenakan flag <code>RETR</code> umumnya digunakan untuk melakukan request suatu file kepada server pada protokol FTP.

<p align="center">
	<img width="80%" height="80%" alt="ae" src="https://github.com/user-attachments/assets/bbc3efc0-1e69-4d74-ac3f-036f0f70b3f1">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya terdapat <b>lima file</b> yang kemungkinan memuat malware, yaitu file <code>q.exe</code>, <code>w.exe</code>, <code>e.exe</code>, <code>r.exe</code>, dan <code>t.exe</code>.
</p>

#### • Soal 16.c: What is the hash of the first file (q.exe)?

<p align="justify">
&emsp; Sebelum kita dapat mengetahui hash dari file malware pertama, maka terlebih dahulu kita perlu menyimpan file tersebut pada penyimpanan lokal di komputer kita dengan cara:
</p>

<ol>
	<li>
		<p align="justify">
			&emsp; Membuka detail dari paket dengan info <code>SIZE q.exe</code> dengan cara menggunakan display filter <code>ftp && ip.src == 10.6.13.102 && ip.dst == 216.55.163.106 && _ws.col.info contains "SIZE q.exe"</code>.
		</p>
		<p align="center">
			<img width="80%" height="80%" alt="af" src="https://github.com/user-attachments/assets/55e1042c-5122-4c66-8865-6e7503d391f6">
		</p>
	</li>
	<li>
		<p align="justify">
			&emsp; Pindah ke frame yang tertera pada <code>File Transfer Protocol (FTP) > Setup frame</code> dengan cara beralih ke menu <code>Go > Go to Packet... > 241</code>. Pada detail paket, temukan port yang digunakan untuk mengirim file <code>q.exe</code> dengan cara melihat pada <code>File Transfer Protocol (FTP) > 227 Entering Passive Mode (216,55,163,106,199,145)\r\n > Passive port</code>.
		</p>
		<p align="center">
			<img width="80%" height="80%" alt="ag" src="https://github.com/user-attachments/assets/32887a2e-034b-49ac-868f-16f7aa4db274">
		</p>
	</li>
	<li>
		<p align="justify">
			&emsp; Gunakan port yang telah ditemukan pada detail paket <code>Setup Frame</code> tersebut sebagai display filter. Yaitu <code>tcp.port == 51089</code>.
		</p>
		<p align="center">
			<img width="80%" height="80%" alt="ah" src="https://github.com/user-attachments/assets/6f19fcb4-2b44-4c3b-ac5b-f3c7f1f1dcd2">
		</p>
	</li>
	<li>
		<p align="justify">
			&emsp; Pilih salah satu paket dan lakukan <code>Follow > TCP Stream > Show as Raw</code>. Di mana angka-angka panjang yang tertera pada menu tersebut merupakan <b>isi dari file</b> <code>q.exe</code>, hanya saja isinya dibagi-bagi menjadi paket yang berbeda saat proses transmisi namun tetap satu stream. Setelah itu, pilih opsi <code>Save as... > q.exe</code> untuk menyimpan isi file tersebut pada penyimpanan lokal di komputer.
		</p>
		<p align="center">
			<img width="80%" height="80%" alt="ai" src="https://github.com/user-attachments/assets/8aef956e-9bec-4fa4-b1e3-a4dfacf272de">
		</p>
	</li>
</ol>

<p align="justify">
Hanya setelah itu baru kita dapat mendapatkan hash dari file <code>q.exe</code> dengan <b>membuka terminal</b> dan menjalankan command <code>sha256sum [alamat file]</code>.
</p>

```sh
sha256sum /home/fedora/Downloads/q.exe 
ca34b0926cdc3242bbfad1c4a0b42cc2750d90db9a272d92cfb6cb7034d2a3bd  /home/fedora/Downloads/q.exe
```

<p align="justify">
&emsp; Setelah menjalankan command <code>sha256sum</code> pada file <code>q.exe</code>, dapat disimpulkan bahwasannya hash dari file pertama dengan format SHA256 adalah <b>ca34b0926cdc3242bbfad1c4a0b42cc2750d90db9a272d92cfb6cb7034d2a3bd</b>.
</p>

#### • Soal 16.d: What is the hash of the second file (w.exe)?

<p align="justify">
&emsp; Sebelum kita dapat mengetahui hash dari file malware kedua, maka terlebih dahulu kita perlu menyimpan file tersebut pada penyimpanan lokal di komputer kita dengan metode yang sama untuk menyimpan file <code>q.exe</code>. Hanya setelah itu baru kita dapat mendapatkan hash dari file <code>w.exe</code> dengan <b>membuka terminal</b> dan menjalankan command <code>sha256sum [alamat file]</code>.
</p>

```sh
sha256sum /home/fedora/Downloads/w.exe
08eb941447078ef2c6ad8d91bb2f52256c09657ecd3d5344023edccf7291e9fc  /home/fedora/Downloads/w.exe
```

<p align="justify">
&emsp; Setelah menjalankan command <code>sha256sum</code> pada file <code>w.exe</code>, dapat disimpulkan bahwasannya hash dari file kedua dengan format SHA256 adalah <b>08eb941447078ef2c6ad8d91bb2f52256c09657ecd3d5344023edccf7291e9fc</b>.
</p>

#### • Soal 16.e: What is the hash of the third file (e.exe)?

<p align="justify">
&emsp; Sebelum kita dapat mengetahui hash dari file malware ketiga, maka terlebih dahulu kita perlu menyimpan file tersebut pada penyimpanan lokal di komputer kita dengan metode yang sama untuk menyimpan file <code>q.exe</code>. Hanya setelah itu baru kita dapat mendapatkan hash dari file <code>e.exe</code> dengan <b>membuka terminal</b> dan menjalankan command <code>sha256sum [alamat file]</code>.
</p>

```sh
sha256sum /home/fedora/Downloads/e.exe
32e1b3732cd779af1bf7730d0ec8a7a87a084319f6a0870dc7362a15ddbd3199  /home/fedora/Downloads/e.exe
```

<p align="justify">
&emsp; Setelah menjalankan command <code>sha256sum</code> pada file <code>e.exe</code>, dapat disimpulkan bahwasannya hash dari file ketiga dengan format SHA256 adalah <b>32e1b3732cd779af1bf7730d0ec8a7a87a084319f6a0870dc7362a15ddbd3199</b>.
</p>

#### • Soal 16.f: What is the hash of the fourth file (r.exe)?

<p align="justify">
&emsp; Sebelum kita dapat mengetahui hash dari file malware keempat, maka terlebih dahulu kita perlu menyimpan file tersebut pada penyimpanan lokal di komputer kita dengan metode yang sama untuk menyimpan file <code>q.exe</code>. Hanya setelah itu baru kita dapat mendapatkan hash dari file <code>r.exe</code> dengan <b>membuka terminal</b> dan menjalankan command <code>sha256sum [alamat file]</code>.
</p>

```sh
sha256sum /home/fedora/Downloads/r.exe
4ebd58007ee933a0a8348aee2922904a7110b7fb6a316b1c7fb2c6677e613884  /home/fedora/Downloads/r.exe
```

<p align="justify">
&emsp; Setelah menjalankan command <code>sha256sum</code> pada file <code>r.exe</code>, dapat disimpulkan bahwasannya hash dari file keempat dengan format SHA256 adalah <b>4ebd58007ee933a0a8348aee2922904a7110b7fb6a316b1c7fb2c6677e613884</b>.
</p>

#### • Soal 16.g: What is the hash of the fifth file (t.exe)?

<p align="justify">
&emsp; Sebelum kita dapat mengetahui hash dari file malware kelima, maka terlebih dahulu kita perlu menyimpan file tersebut pada penyimpanan lokal di komputer kita dengan metode yang sama untuk menyimpan file <code>q.exe</code>. Hanya setelah itu baru kita dapat mendapatkan hash dari file <code>t.exe</code> dengan <b>membuka terminal</b> dan menjalankan command <code>sha256sum [alamat file]</code>.
</p>

```sh
sha256sum /home/fedora/Downloads/t.exe
10ce4b79180a2ddd924fdc95951d968191af2ee3b7dfc96dd6a5714dbeae613a  /home/fedora/Downloads/t.exe
```

<p align="justify">
&emsp; Setelah menjalankan command <code>sha256sum</code> pada file <code>t.exe</code>, dapat disimpulkan bahwasannya hash dari file kelima dengan format SHA256 adalah <b>10ce4b79180a2ddd924fdc95951d968191af2ee3b7dfc96dd6a5714dbeae613a</b>.
</p>

### • Soal 17

<blockquote>
    <ol start="17">
        <li>
            <p align="justify">Manwe membuat halaman web di node-nya yang menampilkan gambar cincin agung. Melkor yang melihat web tersebut merasa iri sehingga ia meletakkan file berbahaya agar web tersebut dapat dianggap menyebarkan malware oleh Eru. Analisis file capture untuk menggagalkan rencana Melkor dan menyelamatkan web Manwe.
	    </p>
        </li>
    </ol>
</blockquote>

```bash
nc 10.15.43.32 3404

===== Soal 17 =====
Difficulty: Hard
Note: You can exit anytime by typing 'exit'

What is the name of the first suspicious file?
Format: file.exe
> Invoice&MSO-Request.doc

What is the name of the second suspicious file?
Format: file.exe
> knr.exe

What is the hash of the second suspicious file (knr.exe)?
Format: sha256
> 749e161661290e8a2d190b1a66469744127bc25bf46e5d0c6f2e835f4b92db18
Congratulations! Here is your flag: KOMJAR25{M4ster_4n4lyzer_9kTRAJDBg0k4TphQM6UI7BrYf}
```

#### • Soal 17.a: What is the name of the first suspicious file?

<p align="justify">
&emsp; Sebelum dapat mengetahui nama file yang memuat malware, maka kita perlu terlebih dahulu mengetahui secara definitif protokol apa yang digunakan attacker (Melkor) untuk mengirim file malware. Hal ini dapat dilakukan dengan beralih ke menu <code>Statistics > Protocol Hierarchy</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="x" src="https://github.com/user-attachments/assets/44fe03a6-db09-4c72-be35-751d0fd7fbb7">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya kemungkinan protokol yang digunakan untuk mengirim file malware adalah <b>HTTP</b>.
</p>

<p align="justify">
&emsp; Selain melihat protokol yang digunakan, kita juga perlu mengetahui secara definitif IP address mana yang berinteraksi dengan file malware tersebut dengan cara beralih ke menu <code>Statistics > Conversations</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="y" src="https://github.com/user-attachments/assets/ceb8cb94-d57d-4700-a358-a304fdb0e044">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya kemungkinan IP address yang berinteraksi dengan file malware dan bertindak sebagai client adalah IP address <b>10.6.27.102</b> dikarenakan IP address tersebut merupakan IP privat, serta jumlah bytes dari paket yang dia dapat dari IP address <b>107.180.50.162</b> yang abnormal dibandingkan dengan percakapannya dengan IP address lain. Maka, keseluruhan display filter yang digunakan adalah <code>http && ip.src == 10.6.27.102 && ip.dst == 107.180.50.162</code>
</p>

<p align="center">
	<img width="80%" height="80%" alt="z" src="https://github.com/user-attachments/assets/0b1ba4f1-7f7e-4799-8cfc-f80fb2c674f8">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya nama file pertama yang memuat malware, dengan mengurutkannya berdasarkan frame di mana file tersebut berada, maka nama file malware pertama adalah <code>Invoice&MSO-Request.doc</code> yang berada pada frame <b>71</b>.
</p>

#### • Soal 17.b: What is the name of the second suspicious file?

<p align="center">
	<img width="80%" height="80%" alt="aa" src="https://github.com/user-attachments/assets/6c49e2ff-d78e-4198-a58e-7b2cc8a1bcdb">
</p>

<p align="justify">
&emsp; Berdasarkan hasil temuan pada 17.a dan mengurutkannya berdasarkan frame di mana file tersebut berada, maka dapat disimpulkan bahwasannya file malware kedua adalah <code>knr.exe</code> yang berada pada frame <b>356</b>.
</p>

#### • Soal 17.c: What is the hash of the second suspicious file (knr.exe)?

<p align="justify">
&emsp; Sebelum kita dapat mengetahui hash dari file malware kedua, maka terlebih dahulu kita perlu menyimpan file tersebut pada penyimpanan lokal di komputer kita dengan memilih opsi <code>Save</code> untuk file <code>knr.exe</code> pada menu <code>File > Export Objects > HTTP...</code>. Hanya setelah itu baru kita dapat mendapatkan hash dari file <code>knr.exe</code> dengan <b>membuka terminal</b> dan menjalankan command <code>sha256sum [alamat file]</code>.
</p>

```sh
sha256sum /home/fedora/Downloads/knr.exe
749e161661290e8a2d190b1a66469744127bc25bf46e5d0c6f2e835f4b92db18  /home/fedora/Downloads/knr.exe
```

<p align="justify">
&emsp; Setelah menjalankan command <code>sha256sum</code> pada file <code>knr.exe</code>, dapat disimpulkan bahwasannya hash dari file pertama dengan format SHA256 adalah <b>749e161661290e8a2d190b1a66469744127bc25bf46e5d0c6f2e835f4b92db18</b>.

### • Soal 18

<blockquote>
    <ol start="18">
        <li>
            <p align="justify">Karena rencana Melkor yang terus gagal, ia akhirnya berhenti sejenak untuk berpikir. Pada saat berpikir ia akhirnya memutuskan untuk membuat rencana jahat lainnya dengan meletakkan file berbahaya lagi tetapi dengan metode yang berbeda. Gagalkan lagi rencana Melkor dengan mengidentifikasi file capture yang disediakan agar dunia tetap aman.
	    </p>
        </li>
    </ol>
</blockquote>

```bash
nc 10.15.43.32 3405

===== Soal 18 =====
Difficulty: Hard
Note: You can exit anytime by typing 'exit'

How many files are suspected of containing malware?
Format: int
> 2

What is the name of the first malicious file?
Format: file.exe
> d0p2nc6ka3f_fixhohlycj4ovqfcy_smchzo_ub83urjpphrwahjwhv_o5c0fvf6.exe

Apa nama file berbahaya yang kedua?
Format: file.exe
> oiku9bu68cxqenfmcsos2aek6t07_guuisgxhllixv8dx2eemqddnhyh46l8n_di.exe

What is the hash of the first malicious file?
Format: sha256
> 59896ae5f3edcb999243c7bfdc0b17eb7fe28f3a66259d797386ea470c010040

What is the hash of the second malicious file?
Format: sha256
> cf99990bee6c378cbf56239b3cc88276eec348d82740f84e9d5c343751f82560
Congratulations! Here is your flag: KOMJAR25{Y0u_4re_g0dl1ke_LfpxF7WQlyONdAnhyZqyNex5T}
```

#### • Soal 18.a: How many files are suspected of containing malware?

<p align="justify">
&emsp; Sebelum dapat mengetahui jumlah file yang memuat malware, kita perlu terlebih dahulu mengetahui secara definitif protokol apa yang digunakan attacker (Melkor) untuk mengirim file malware. Hal ini dapat dilakukan dengan beralih ke menu <code>Statistics > Protocol Hierarchy</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="n" src="https://github.com/user-attachments/assets/f3a4654f-cee5-4f06-970f-2791aac087d3">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya terdapat tiga kemungkinan untuk protokol yang digunakan untuk mengirim file malware, yaitu TLS, HTTP, dan SMB. Namun, kita dapat menentukan protokol mana yang sebenarnya digunakan dengan mempertimbangkan hal-hal berikut:
	<ol>
		<li>
			<p align="justify">
			Pada soal sebelumnya, Melkor telah menggunakan protokol HTTP untuk mengirim file malware. Hal ini didasari dengan merujuk pada pernyataan yang ada pada soal 18, di mana:
			</p>
			<blockquote>
			"Pada saat berpikir ia akhirnya memutuskan untuk membuat rencana jahat lainnya dengan meletakkan file berbahaya lagi tetapi dengan <b>metode yang berbeda</b>."
			</blockquote>
			Sehingga kemungkinan besar, Melkor tidak menggunakan HTTP untuk serangan kali ini.
		</li>
		<li>
			<p align="justify">
			Spesifik untuk soal ini, kita tidak disediakan file key log yang krusial untuk dapat mendekripsi dan membaca data yang terkirim melalui protokol TLS. Sehingga kemungkinan besar, Melkor tidak menggunakan TLS untuk serangan kali ini (Sebenarnya bisa saja, namun kalau masalah memakai protokol TLS tetapi tidak ada file key log-nya itu beda cerita).
			</p>
		</li>
	</ol>
Maka dari itu, kemungkinan besar Melkor menggunakan protokol <b>SMB</b> untuk serangan kali ini.
</p>

<p align="justify">
&emsp; Setelah mengetahui protokol apa yang digunakan, maka selanjutnya kita dapat melihat file-file apa saja yang dikirimkan melalui protokol SMB dengan cara beralih ke menu <code>File > Export Objects > SMB...</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="o" src="https://github.com/user-attachments/assets/005bd4be-9b37-4fcb-8f91-0070b776268f">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya terdapat <b>dua file</b> yang membawa malware pada file PCAP ini, yaitu <code>\WINDOWS\d0p2nc6ka3f_..._o5c0fvf6.exe</code> dan <code>\WINDOWS\oiku9bu68cxqenfmcsos...hyh46l8n_di.exe</code> dengan mempertimbangkan beberapa hal ini:
	<ol>
		<li>
			<p align="justify">
			Kedua file memiliki ukuran yang abnormal dibandingkan dengan file yang lain, di mana kedua file memiliki ukuran pada rentang <b>kB</b>, sedangkan file lain hanya berada di kisaran <b>puluhan byte</b> atau bahkan <b>nol</b>.
			</p>
		</li>
		<li>
			<p align="justify">
			Kedua file memiliki ekstensi berupa <code>.exe</code> di mana ekstensi executable rentan dianggap sebagai pembawa malware.
			</p>
		</li>
		<li>
			<p align="justify">
			Kedua file memiliki <code>Content Type</code> berupa <code>FILE</code>.
			</p>
		</li>
		<li>
			<p align="justify">
			Hostname dari kedua file merupakan IP address privat dan bukan IP address eksternal seperti yang tertera pada file <code>\cliffstone.net\Policies\{31B2F340-016D-11D2-945F-00C04FB984F9}\gpt.ini</code>.
			</p>
		</li>
	</ol>
</p>

#### • Soal 18.b: What is the name of the first malicious file?

<p align="center">
	<img width="80%" height="80%" alt="p" src="https://github.com/user-attachments/assets/f97fb5ab-dd1d-4ea5-98ec-65c187e7dba3">
</p>

<p align="justify">
&emsp; Berdasarkan hasil temuan pada 14.a dan mengurutkannya berdasarkan frame di mana file tersebut berada, maka dapat disimpulkan bahwasannya file malware pertama adalah <code>\WINDOWS\d0p2nc6ka3f_fixhohlycj4ovqfcy_smchzo_ub83urjpphrwahjwhv_o5c0fvf6.exe</code> yang berada pada frame <b>7058</b>.
</p>

#### • Soal 18.c: Apa nama file berbahaya yang kedua?

<p align="center">
	<img width="80%" height="80%" alt="q" src="https://github.com/user-attachments/assets/b3483335-b5fd-4590-82e1-61ee090a3fc1">
</p>

<p align="justify">
&emsp; Berdasarkan hasil temuan pada 14.a dan mengurutkannya berdasarkan frame di mana file tersebut berada, maka dapat disimpulkan bahwasannya file malware kedua adalah <code>\WINDOWS\oiku9bu68cxqenfmcsos2aek6t07_guuisgxhllixv8dx2eemqddnhyh46l8n_di.exe</code> yang berada pada frame <b>7936</b>.
</p>

#### • Soal 18.d: What is the hash of the first malicious file?

<p align="justify">
&emsp; Sebelum kita dapat mengetahui hash dari kedua file malware, maka terlebih dahulu kita perlu menyimpan kedua file pada penyimpanan lokal di komputer kita dengan memilih opsi <code>Save</code> pada menu <code>File > Export Objects > SMB...</code> yang sama. Hanya setelah itu baru kita dapat mendapatkan hash dari kedua file dengan <b>membuka terminal</b> dan menjalankan command <code>sha256sum [alamat file]</code>.
</p>

```sh
sha256sum /home/fedora/Downloads/%5cWINDOWS%5cd0p2nc6ka3f_fixhohlycj4ovqfcy_smchzo_ub83urjpphrwahjwhv_o5c0fvf6.exe 
59896ae5f3edcb999243c7bfdc0b17eb7fe28f3a66259d797386ea470c010040  /home/fedora/Downloads/%5cWINDOWS%5cd0p2nc6ka3f_fixhohlycj4ovqfcy_smchzo_ub83urjpphrwahjwhv_o5c0fvf6.exe
```

<p align="justify">
&emsp; Setelah menjalankan command <code>sha256sum</code> pada file <code>\WINDOWS\d0p2nc6ka3f_..._o5c0fvf6.exe</code>, dapat disimpulkan bahwasannya hash dari file pertama dengan format SHA256 adalah <b>59896ae5f3edcb999243c7bfdc0b17eb7fe28f3a66259d797386ea470c010040</b>.

#### • Soal 18.e: What is the hash of the second malicious file?

<p align="justify">
&emsp; Sebelum kita dapat mengetahui hash dari kedua file malware, maka terlebih dahulu kita perlu menyimpan kedua file pada penyimpanan lokal di komputer kita dengan memilih opsi <code>Save</code> pada menu <code>File > Export Objects > SMB...</code> yang sama. Hanya setelah itu baru kita dapat mendapatkan hash dari kedua file dengan <b>membuka terminal</b> dan menjalankan command <code>sha256sum [alamat file]</code>.
</p>

```sh
sha256sum /home/fedora/Downloads/%5cWINDOWS%5coiku9bu68cxqenfmcsos2aek6t07_guuisgxhllixv8dx2eemqddnhyh46l8n_di.exe 
cf99990bee6c378cbf56239b3cc88276eec348d82740f84e9d5c343751f82560  /home/fedora/Downloads/%5cWINDOWS%5coiku9bu68cxqenfmcsos2aek6t07_guuisgxhllixv8dx2eemqddnhyh46l8n_di.exe
```

<p align="justify">
&emsp; Setelah menjalankan command <code>sha256sum</code> pada file <code>\WINDOWS\oiku9bu68cxqenfmcsos...hyh46l8n_di.exe</code>, dapat disimpulkan bahwasannya hash dari file kedua dengan format SHA256 adalah <b>cf99990bee6c378cbf56239b3cc88276eec348d82740f84e9d5c343751f82560</b>.
</p>

### • Soal 19

<blockquote>
    <ol start="19">
        <li>
            <p align="justify">Manwe mengirimkan email berisi surat cinta kepada Varda melalui koneksi yang tidak terenkripsi. Melihat hal itu Melkor sipaling jahat langsung melancarkan aksinya yaitu meneror Varda dengan email yang disamarkan. Analisis file capture jaringan dan gagalkan lagi rencana busuk Melkor.
	    </p>
        </li>
    </ol>
</blockquote>

```bash
nc 10.15.43.32 3406

===== Soal 19 =====
Difficulty: Hard
Note: You can exit anytime by typing 'exit'

Who sent the threatening message?
Format: string (name)
> Your Life

How much ransom did the attacker demand ($)?
Format: int
> 1600

What is the attacker's bitcoin wallet?
Format: string
> 1CWHmuF8dHt7HBGx5RKKLgg9QA2GmE3UyL
Congratulations! Here is your flag: KOMJAR25{Y0u_4re_J4rk0m_G0d_mZTuSO0QZ9AdMjOB4686nU0U1}
```

#### • Soal 19.a: Who sent the threatening message?

<p align="justify">
&emsp; Diketahui bahwasannya protokol yang digunakan E-mail, khususnya perihal transfer atau pengiriman E-mail adalah protokol <b>SMTP</b>. Maka dari itu, display filter yang digunakan adalah <code>smtp</code>.
</p>

<p align="center"> 
	<img width="80%" height="80%" alt="i" src="https://github.com/user-attachments/assets/7a9e7001-31ce-425d-a155-630412f58980">
</p>

<p align="justify">
&emsp; Kemudian, langkah selanjutnya setelah memfilter paket yang menggunakan protokol SMTP adalah kita dapat membuka <b>stream TCP</b> dari salah satu paket SMTP yang tertera tersebut untuk mengetahui isi dari E-mail yang dikirim oleh client (Melkor). Hal ini dikarenakan protokol SMTP tidak mengirimkan isi E-mail serta merta dilakukan sekaligus dalam satu paket, melainkan membagi isi E-mail ke dalam paket-paket yang berbeda.
</p>

<p align="center"> 
	<img width="80%" height="80%" alt="j" src="https://github.com/user-attachments/assets/4ddb0fef-eddb-4d44-aafb-2fd1bc95db39">
</p>

<p align="center"> 
	<img width="80%" height="80%" alt="k" src="https://github.com/user-attachments/assets/ebc9be2c-8816-4995-81f4-7c5bcfcc61b2">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya user yang mengirimkan E-mail ancaman tersebut adalah <b>Your Life</b>.
</p>

#### • Soal 19.b: How much ransom did the attacker demand ($)?

<p align="justify">
Pada stream TCP yang sama kita dapat mengetahui seberapa jumlah uang dalam bentuk Bitcoin yang diminta oleh Your Life.
</p>

<p align="center"> 
	<img width="80%" height="80%" alt="l" src="https://github.com/user-attachments/assets/597256c9-9eff-4b7e-9e51-b7fadbdb5040">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya jumlah uang yang diminta oleh Your Life dalam bentuk Bitcoin adalah <b>1600$</b>.
</p>

#### • Soal 19.c: What is the attacker's bitcoin wallet?

<p align="justify">
Pada stream TCP yang sama kita dapat mengetahui alamat dari dompet Bitcoin Your Life.
</p>

<p align="center"> 
	<img width="80%" height="80%" alt="m" src="https://github.com/user-attachments/assets/9e489f9c-e76e-44cd-8d7b-b792d0656021">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya alamat dari dompet Bitcoin Your Life adalah <b>1CWHmuF8dHt7HBGx5RKKLgg9QA2GmE3UyL</b>.
</p>

### • Soal 20

<blockquote>
    <ol start="20">
        <li>
            <p align="justify">Untuk yang terakhir kalinya, rencana besar Melkor yaitu menanamkan sebuah file berbahaya kemudian menyembunyikannya agar tidak terlihat oleh Eru. Tetapi Manwe yang sudah merasakan adanya niat jahat dari Melkor, ia menyisipkan bantuan untuk mengungkapkan rencana Melkor. Analisis file capture dan identifikasi kegunaan bantuan yang diberikan oleh Manwe untuk menggagalkan rencana jahat Melkor selamanya.
	    </p>
        </li>
    </ol>
</blockquote>

```bash
nc 10.15.43.32 3407

===== Soal 20 =====
Difficulty: Hard
Note: You can exit anytime by typing 'exit'

What encryption method is used?
Format: string
> TLS

What is the name of the malicious file placed by the attacker?
Format: file.exe
> invest_20.dll

What is the hash of the file containing the malware?
Format: sha256
> 31cf42b2a7c5c558f44cfc67684cc344c17d4946d3a1e0b2cecb8eb58173cb2f
Congratulations! Here is your flag: KOMJAR25{B3ware_0f_M4lw4re_yau7ElDfafuTufKs0aXlBTA8b}
```

#### • Soal 20.a: What encryption method is used?

<p align="justify">
&emsp; Sebelum dapat mengetahui jumlah file yang memuat malware, kita perlu terlebih dahulu mengetahui secara definitif protokol apa yang digunakan attacker (Melkor) untuk mengirim file malware. Hal ini dapat dilakukan dengan beralih ke menu <code>Statistics > Protocol Hierarchy</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="r" src="https://github.com/user-attachments/assets/486004da-d834-46ba-accf-8f16792f382c">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya kemungkinan protokol yang digunakan sekaligus metode enkripsi yang digunakan untuk mengirim file malware adalah <b>TLS</b> (Soal hanya membutuhkan TLS sebagai jawaban, namun pada detail salah satu paket yang menggunakan protokol TLS, khususnya pada bagian <code>Server Hello -> Cipher Suite</code>, kita dapat mengetahui bahwasannya enkripsi yang digunakan oleh TLS adalah <code>TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256</code>).
</p>

#### • Soal 20.b: What is the name of the malicious file placed by the attacker?

<p align="justify">
&emsp; Selain melihat protokol yang digunakan, kita juga perlu mengetahui secara definitif IP address mana yang berinteraksi dengan file malware tersebut dengan cara beralih ke menu <code>Statistics > Conversations</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="s" src="https://github.com/user-attachments/assets/7a40f897-1d40-450f-89ac-a3fc8bb144e6">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya kemungkinan IP address yang berinteraksi dengan file malware dan bertindak sebagai client adalah IP address <b>10.4.1.101</b> dikarenakan IP address tersebut merupakan IP privat, serta jumlah bytes dari paket yang dia dapat dari IP address <b>94.103.84.245</b> yang abnormal dibandingkan dengan percakapannya dengan IP address lain.
</p>

<p align="justify">
&emsp; Juga, sebelum dapat melihat data yang berada paket-paket yang melalui IP address 10.4.1.101 dan dienkripsi dengan TLS, khususnya yang bersifat ECDHE, maka kita perlu meng-import suatu file lient-side pre-master secrets (SSLKEYLOGFILE) yang telah disediakan oleh soal dengan cara beralih ke menu <code>Edit -> Preferences -> Protocols -> TLS -> (Pre)-Master-Secret log filename -> Browse… -> keyslogfile.txt (sudah disediakan) -> Apply -> OK</code>. 
</p>

<p align="center">
	<img width="80%" height="80%" alt="t" src="https://github.com/user-attachments/assets/b17ed666-c58d-4fcb-a4d0-611d8d3c663a">
</p>

<p align="justify">
Sehingga tampilan paket-paket yang terenkripsi TLS akan berubah menjadi:
</p>

<p align="center">
	<img width="80%" height="80%" alt="u" src="https://github.com/user-attachments/assets/ec643924-240b-40aa-84cc-5ab8f506e1d4">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, terdapat beberapa paket-paket yang pada awalnya tertera menggunakan protokol TLS yang terenkripsi berubah menjadi menunjukkan protokol <b>HTTP</b> yang dapat dibaca. Sehingga untuk mencari file, kita dapat menggunakan display filter yaitu <code>http && http.request.method == "GET"</code>, di mana <code>GET</code> umumnya digunakan untuk melakukan request suatu file kepada server pada protokol HTTP.
</p>

<p align="center">
	<img width="80%" height="80%" alt="v" src="https://github.com/user-attachments/assets/f6dd7269-c790-43c9-a482-c9f88637aa0e">
</p>

<p align="justify">
&emsp; Berdasarkan screenshot di atas, dapat disimpulkan bahwasannya file malware yang digunakan oleh attacker (Melkor) adalah <code>invest_20.dll</code> dikarenakan kedua file yang lain kemungkinan besar hanya merupakan konfigurasi yang dilakukan oleh sistem Windows.
</p>

#### • Soal 20.c: What is the hash of the file containing the malware?

<p align="justify">
&emsp; Sebelum kita dapat mengetahui hash dari file malware, maka terlebih dahulu kita perlu menyimpan file <code>invest_20.dll</code> pada penyimpanan lokal di komputer kita dengan cara beralih ke menu <code>File > Export Objects > HTTP...</code> dan memilih opsi <code>Save</code>.
</p>

<p align="center">
	<img width="80%" height="80%" alt="w" src="https://github.com/user-attachments/assets/771b91cd-2502-45b4-ab9a-2e8e08c807ad">
</p>

<p align="justify">
&emsp; Hanya setelah itu baru kita dapat mendapatkan hash dari file malware <code>invest_20.dll</code> dengan <b>membuka terminal</b> dan menjalankan command <code>sha256sum [alamat file]</code>.
</p>

```sh
sha256sum /home/fedora/Downloads/invest_20.dll 
31cf42b2a7c5c558f44cfc67684cc344c17d4946d3a1e0b2cecb8eb58173cb2f  /home/fedora/Downloads/invest_20.dll
```

<p align="justify">
&emsp; Setelah menjalankan command <code>sha256sum</code> pada file <code>invest_20.dll</code>, dapat disimpulkan bahwasannya hash dari file kedua dengan format SHA256 adalah <b>31cf42b2a7c5c558f44cfc67684cc344c17d4946d3a1e0b2cecb8eb58173cb2f</b>.
</p>

## Kendala Pengerjaan

## Revisi
