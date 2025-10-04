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
#### • Soal 16.b: How many files are suspected of containing malware?
#### • Soal 16.c: What is the hash of the first file (q.exe)?
#### • Soal 16.d: What is the hash of the second file (w.exe)?
#### • Soal 16.e: What is the hash of the third file (e.exe)?
#### • Soal 16.f: What is the hash of the fourth file (r.exe)?
#### • Soal 16.g: What is the hash of the fifth file (t.exe)?

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
#### • Soal 17.b: What is the name of the second suspicious file?
#### • Soal 17.c: What is the hash of the second suspicious file (knr.exe)?

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
&emsp; Berdasarkan screenshot di atas, bahwasannya terdapat tiga kemungkinan untuk protokol yang digunakan untuk mengirim file malware, yaitu TLS, HTTP, dan SMB. Namun, kita dapat menentukan protokol mana yang sebenarnya digunakan dengan mempertimbangkan hal-hal berikut:
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
#### • Soal 20.b: What is the name of the malicious file placed by the attacker?
#### • Soal 20.c: What is the hash of the file containing the malware?

No. 15
===== Soal 15 =====
Difficulty: Medium
Note: You can exit anytime by typing 'exit'

What device does Melkor use?
Format: string
> Keyboard

Dari soal sudah dinyatakan:
Melkor menyusup ke ruang server dan memasang keyboard USB berbahaya pada node Manwe.

What did Melkor write?
Format: string
> UGx6X3ByMHYxZGVfeTB1cl91czNybjRtZV80bmRfcDRzc3cwcmQ=

Keystroke terletak pada kategori URB_INTERRUPT in dengan destination host (Host dari alat-alat USB)
usb.transfer_type == 0x01 && !usb.src == host

<img width="1920" height="1001" alt="Screenshot From 2025-09-30 15-59-05" src="https://github.com/user-attachments/assets/cf7c2de7-6d0f-4b70-829a-ce8bc535ea97" />


Setiap paket umumnya hanya memuat satu keystroke. Untuk otomasi dan menampilkan seluruh stream keystroke dari target menggunakan tshark.

Data keystroke tersimpan pada field HID (usbhid.data).
Command tshark:
tshark -r /home/fedora/Downloads/hiddenmsg.pcapng   -Y 'usb.transfer_type == 0x01 && !usb.src == host'   -T fields -e usbhid.data

<img width="1920" height="946" alt="Screenshot From 2025-09-30 16-04-44" src="https://github.com/user-attachments/assets/fdeb2b4f-1826-4c85-81dc-a9e52562d8cf" />


Output:
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

Konversi data HID ke ASCII dengan program Python:



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
    if line:
        sys.stdout.write(decode(line))

Pipe output tshark ke python3:

tshark -r /home/fedora/Downloads/hiddenmsg.pcapng   -Y 'usb.transfer_type == 0x01 && !usb.src == host'  -T fields -e usbhid.data | python3 hid2ascii.py

<img width="1920" height="946" alt="Screenshot From 2025-09-30 16-18-19" src="https://github.com/user-attachments/assets/10ce14c9-06e1-4eaa-a420-400a4e8673a6" />



Output:
UGx6X3ByMHYxZGVfeTB1cl91czNybjRtZV80bmRfcDRzc3cwcmQ=

What is Melkor's secret message?
Format: string
> Plz_pr0v1de_y0ur_us3rn4me_4nd_p4ssw0rd
Congratulations! Here is your flag: KOMJAR25{K3yb0ard_W4rr10r_gz6mwpsdLTyJlTNVHeusOzDP0}

Ada sama dengan di akhir -> Base64. Decode:


<img width="1920" height="859" alt="Screenshot From 2025-09-30 19-04-48" src="https://github.com/user-attachments/assets/dafd4d40-7699-4f82-96c2-b0ef35543568" />


Output:
Plz_pr0v1de_y0ur_us3rn4me_4nd_p4ssw0rd

No. 16

FTP = File Transfer Protocol

229    17.282471    216.55.163.106    10.6.13.102    FTP    101    Response: 331 User ind@psg420.com OK. Password required

231    17.282954    10.6.13.102    216.55.163.106    FTP    73    Request: PASS {6r_6e#TfT1p

What credential did the attacker use to log in?
Format: user:pass
> ind@psg420.com:{6r_6e#TfT1p

Pada HTTP tidak ada indikasi seperti GET halaman login. Mencoba protokol lain, seperti FTP.

How many files are suspected of containing malware?
Format: int
> 5

q.exe
w.exe
e.exe
r.exe
t.exe

<img width="1920" height="997" alt="Screenshot From 2025-09-30 19-53-56" src="https://github.com/user-attachments/assets/6c0eb9d1-c86c-4485-91ed-eb581fa5836b" />

Jumlah IP pada PCAP ada 5. IP 10.6.13.102 merupakan IP pertama yang meminta request SYN, Jumlah Bytes yang dikirim cukup besar, Merupakan IP private dan bukan IP eksternal dengan geolokasi. Potensi Malware.
Jadi filter pertama:
ip.src = 10.6.13.102

<img width="1920" height="997" alt="Screenshot From 2025-09-30 19-57-44" src="https://github.com/user-attachments/assets/fae7acaf-d194-4de1-95f2-638edab03e5a" />


FTP menjadi protokol dengan persentase Bytes terbesar pada PCAP. Memiliki potensi membawa malware. FTP didesain untuk mentransfer file.

Filter ke 2:
ftp

<img width="1920" height="997" alt="Screenshot From 2025-10-01 02-27-51" src="https://github.com/user-attachments/assets/4f1fd1d3-32d0-4b52-a89b-1b48a5194a18" />


Secara langsung dapat terlihat dua frame yang menarik, yaitu frame 227 dan frame 231.
Sehingga:
USER ind@psg420.com
PASS PASS {6r_6e#TfT1p

<img width="1920" height="997" alt="Screenshot From 2025-10-01 02-35-15" src="https://github.com/user-attachments/assets/c683932a-50c3-4300-8c87-2b05883da87f" />


Dua command FTP yang menarik perhatian:
RETR <filename> -> Client downloads a file from server.
STOR <filename> -> Client uploads a file to server.

STOR pada file PCAP tidak menunjukkan adanya file malware dan hanya berupa logs. Sedangkan pada RETR terdapat 5 file yang muncul dan kemungkinan berbahaya (File exe).

Jumlah ada 5: q.exe, w.exe, e.exe, r.exe, t.exe

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-05-58" src="https://github.com/user-attachments/assets/98ebe473-9e86-4a97-b6ff-0445fc0b378d" />



Lihat detail SIZE dari setiap file malware
ftp && ip.src == 10.6.13.102 && ftp.request.command == "SIZE"
Mencari IP dan port yang digunakan server untuk terhubung ke client dan mengunduh file malware.

Pindah ke SETUP frame: 241

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-10-11" src="https://github.com/user-attachments/assets/d03247a4-3d53-4c99-be4b-76621f308f67" />


File Transfer Protocol (FTP)
    227 Entering Passive Mode (216,55,163,106,199,145)\r\n
        Response code: Entering Passive Mode (227)
        Response arg: Entering Passive Mode (216,55,163,106,199,145)
        Passive IP address: 216.55.163.106
        Passive port: 51089

Filter paket yang datang (source) dari port 51089 dengan filter:
tcp.port == 51089

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-13-01" src="https://github.com/user-attachments/assets/362cb674-45a0-4c65-b76f-3e152ca58c06" />


Kemudian pilih salah satu paket dan Follow TCP Stream

Isi dari TCP stream tersebut adalah Isi dari q.exe.
Pilih:
Entire Conversations -> Show As Raw -> Save As -> q.exe

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-12-36" src="https://github.com/user-attachments/assets/00c03161-eb6e-4962-b413-bb6cf17150fe" />


Gunakan command sha256sum untuk mengetahui hash dari q.exe:

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-14-02" src="https://github.com/user-attachments/assets/4a1adb68-6136-4710-b22f-d36bc5c8da87" />



Output:
ca34b0926cdc3242bbfad1c4a0b42cc2750d90db9a272d92cfb6cb7034d2a3bd

w.exe:

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-29-36" src="https://github.com/user-attachments/assets/0757b7fb-8891-4029-95b6-c49994b75e85" />


Setup Frame: 1111


<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-15-47" src="https://github.com/user-attachments/assets/aa5f0380-f995-4f2a-b4ff-31b0e373842b" />

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-17-34" src="https://github.com/user-attachments/assets/95b91cba-0cdc-44b4-b49e-4bccaa5c7c11" />

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-17-06" src="https://github.com/user-attachments/assets/4b470a77-c0ba-485a-ac0c-021faebb4cf9" />


SIZE -> Setup Frame -> Port server: 59785
tcp.port == 59785
Follow TCP Stream
Save as w.exe
sha265sum

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-18-47" src="https://github.com/user-attachments/assets/0d80245e-b541-493e-8a9f-b21fc978a8c0" />

e.exe:

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-28-52" src="https://github.com/user-attachments/assets/32207eb6-45c0-47db-9a26-70d2750e2e80" />


Setup Frame: 1295
<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-21-38" src="https://github.com/user-attachments/assets/3fad5f55-6cab-43e4-be7d-b535004e9d42" />



Port: 49506

tcp.port == 49506

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-23-04" src="https://github.com/user-attachments/assets/1a4dc2b3-2525-45ea-bafa-9e9ecfab66f2" />


<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-23-26" src="https://github.com/user-attachments/assets/91b085b1-ddde-40b9-8d9c-022973e59eae" />


<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-24-02" src="https://github.com/user-attachments/assets/6471dc1e-3bd9-44b5-8980-fe037e522e6c" />


r.exe:

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-28-39" src="https://github.com/user-attachments/assets/c3fccab0-e928-4f43-8009-7f3676a905f4" />


Setup Frame: 2445

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-25-33" src="https://github.com/user-attachments/assets/63d6ded1-558a-4aa7-8b72-68405d5cb05b" />


Port: 60899
tcp.port == 60899
<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-26-44" src="https://github.com/user-attachments/assets/ceecb518-f03b-400b-abad-bd918cc2e3f6" />


<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-26-55" src="https://github.com/user-attachments/assets/b6396d0f-3075-4916-943f-9eddc001fea3" />


<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-27-31" src="https://github.com/user-attachments/assets/1838e2ed-8dd8-4468-8abd-2e304d54573b" />



t.exe:

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-28-20" src="https://github.com/user-attachments/assets/1d1c51bc-97af-42fb-8b47-82249a533fcb" />


Setup Frame: 2643
<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-30-59" src="https://github.com/user-attachments/assets/12c1d57f-b119-49ad-b16a-1d3e9ad7bae7" />



Port: 50157
tcp.port == 50157
<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-31-33" src="https://github.com/user-attachments/assets/665f74e1-47d5-49c9-aa6d-ddac8d3ddd02" />

<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-31-45" src="https://github.com/user-attachments/assets/b8e19c48-540a-43b3-bd7a-63e42c362b04" />


<img width="1920" height="997" alt="Screenshot From 2025-10-01 04-32-17" src="https://github.com/user-attachments/assets/b757fb97-3d3d-4f82-a25d-47ee06eee793" />






No. 17
<img width="1920" height="997" alt="Screenshot From 2025-10-01 07-36-33" src="https://github.com/user-attachments/assets/ceb8cb94-d57d-4700-a358-a304fdb0e044" />


Statistics > Conversations
Traffic terbanyak adalah antara IP 10.6.27.102 dan 107.180.50.162. Sehingga kemungkinan besar file malware dikirim antara keduanya. Filter:
ip.addr == 10.6.27.102 && ip.addr == 107.180.50.162

Statistics > Protocol Hierarchy

<img width="1920" height="997" alt="Screenshot From 2025-10-01 07-42-08" src="https://github.com/user-attachments/assets/44fe03a6-db09-4c72-be35-751d0fd7fbb7" />




Volume traffic kebanyakan dari http. Kemungkinan besar mengirim malware.

Filter:
http

Semuanya:
http && ip.addr == 10.6.27.102 && ip.addr == 107.180.50.162
<img width="1920" height="997" alt="Screenshot From 2025-10-01 07-47-33" src="https://github.com/user-attachments/assets/0c1a43cc-abcf-486c-9063-9fd4b80e0c62" />


Urutan file pertama yang muncul berdasarkan GET (Server 107.180.50.162 (IP eksternal) mengirimkan file berdasarkan request client IP 10.6.27.102 (privat)):
71    29.202755    10.6.27.102    107.180.50.162    HTTP    343    GET /Documents/Invoice&MSO-Request.doc HTTP/1.1
 
Urutan file kedua yang muncul berdasarkan GET (Server 107.180.50.162 (IP eksternal) mengirimkan file berdasarkan request client IP 10.6.27.102 (privat)):
356    38.470797    10.6.27.102    107.180.50.162    HTTP    361    GET /knr.exe HTTP/1.1 

File -> Export Objects -> HTTP -> knr.exe -> Save

<img width="1920" height="997" alt="Screenshot From 2025-10-01 07-55-36" src="https://github.com/user-attachments/assets/01218570-1ae9-4363-b702-f626c2aae15e" />


sha256sum knr.exe

<img width="1920" height="997" alt="Screenshot From 2025-10-01 07-57-05" src="https://github.com/user-attachments/assets/8fcaf938-4bc2-4aa4-a805-2ea501044201" />


Output:
749e161661290e8a2d190b1a66469744127bc25bf46e5d0c6f2e835f4b92db18




No. 18

<img width="1920" height="1003" alt="Screenshot From 2025-10-01 20-35-02" src="https://github.com/user-attachments/assets/f3a4654f-cee5-4f06-970f-2791aac087d3" />


Statistics > Protocol Hierarchy

3 protokol ada pada file PCAP ini dengan urutan jumlah bytes:
TLS
HTTP
SMB

Alasan memilih SMB sebagai kemungkinan tempat malware:
1. Soal menyatakan malware diletakkan menggunakan metode berbeda. Soal 17 menggunakan HTTP sehingga tidak mungkin file berada pada HTTP.
2. Soal ini tidak memberikan session key untuk decrypt protokol TLS. Sehingga tidak mungkin file disimpan di sana.

Buka FILE -> Export Objects -> SMB…

<img width="1920" height="1003" alt="Screenshot From 2025-10-01 20-50-51" src="https://github.com/user-attachments/assets/829ce389-d6f5-4343-821e-1a15b5098230" />


Di sini ada dua file yang kemungkinan merupakan malware, yaitu kedua file dengan ekstensi .exe.


Save kedua file. Gunakan command sha256sum untuk mengetahui hash dari kedua file.
<img width="1920" height="1003" alt="Screenshot From 2025-10-01 20-51-18" src="https://github.com/user-attachments/assets/0d4b5bcc-0e6c-4be4-bdf8-a29195ed8cc9" />



Output untuk file: %5cWINDOWS%5coiku9bu68cxqenfmcsos2aek6t07_guuisgxhllixv8dx2eemqddnhyh46l8n_di.exe 

cf99990bee6c378cbf56239b3cc88276eec348d82740f84e9d5c343751f82560

<img width="1920" height="1003" alt="Screenshot From 2025-10-01 20-52-21" src="https://github.com/user-attachments/assets/ba96bb43-336d-44d4-a9cb-5e595a2258e2" />


Output untuk file:
%5cWINDOWS%5cd0p2nc6ka3f_fixhohlycj4ovqfcy_smchzo_ub83urjpphrwahjwhv_o5c0fvf6.exe 

59896ae5f3edcb999243c7bfdc0b17eb7fe28f3a66259d797386ea470c010040



7054    1096.833911    10.6.26.110    10.6.26.6    SMB    219    NT Create AndX Request, FID: 0x4002, Path: \WINDOWS\d0p2nc6ka3f_fixhohlycj4ovqfcy_smchzo_ub83urjpphrwahjwhv_o5c0fvf6.exe

7932    1096.944375    10.6.26.110    10.6.26.6    SMB    219    NT Create AndX Request, FID: 0x4003, Path: \WINDOWS\	


No. 20

<img width="1920" height="1003" alt="Screenshot From 2025-10-01 19-36-04" src="https://github.com/user-attachments/assets/486004da-d834-46ba-accf-8f16792f382c" />


Statistics > Protocol Hierarchy

TLS menjadi protokol dengan persentase Bytes terbesar pada PCAP. Memiliki potensi membawa malware.
Filter:
tls	

<img width="1920" height="1003" alt="Screenshot From 2025-10-01 19-39-18" src="https://github.com/user-attachments/assets/7a40f897-1d40-450f-89ac-a3fc8bb144e6" />


IP 10.4.1.101 merupakan IP dengan jumlah percakapan terbanyak dengan jumlah Bytes yang dikirim cukup besar pula, Merupakan IP private dan bukan IP eksternal dengan geolokasi. Potensi Malware.

Lihat detail paket Server Hello -> Cipher Suite:
TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256

Soal hanya membutuhkan TLS sebagai jawaban, tapi dari sini kita dapat mengetahui bahwa enkripsi yang digunakan oleh TLS adalah AES_128_GCM

TLS bersifat ECDHE di mana membutuhkan client-side pre-master secrets (SSLKEYLOGFILE) (file log key dari client)

Import file key log:
Edit -> Preferences -> Protocols -> TLS -> (Pre)-Master-Secret log filename -> Browse… -> keyslogfile.txt (sudah disediakan) -> Apply -> OK

<img width="1920" height="1003" alt="Screenshot From 2025-10-01 19-49-08" src="https://github.com/user-attachments/assets/b17ed666-c58d-4fcb-a4d0-611d8d3c663a" />


Sekarang paket TLS sudah didekripsi dan muncul paket-paket dengan protokol HTTP.

<img width="1920" height="1003" alt="Screenshot From 2025-10-01 19-50-22" src="https://github.com/user-attachments/assets/ec643924-240b-40aa-84cc-5ab8f506e1d4" />


Gunakan filter:
http && http.request.method == "GET"

<img width="1920" height="1003" alt="Screenshot From 2025-10-01 19-52-15" src="https://github.com/user-attachments/assets/48a19e28-4063-4b69-a69d-cb55ba5e076a" />



Export file:
File -> Export Objects -> HTTP… -> invest_20.dll -> Save -> invest_20.dll

<img width="1920" height="1003" alt="Screenshot From 2025-10-01 19-55-51" src="https://github.com/user-attachments/assets/771b91cd-2502-45b4-ab9a-2e8e08c807ad" />


Gunakan command sha256sum untuk mengetahui hash dari invest_20.dll.

<img width="1920" height="1003" alt="Screenshot From 2025-10-01 19-58-08" src="https://github.com/user-attachments/assets/929589d4-2400-44b8-9473-1b73e04726f1" />


Output:
31cf42b2a7c5c558f44cfc67684cc344c17d4946d3a1e0b2cecb8eb58173cb2f






## Kendala Pengerjaan

## Revisi
