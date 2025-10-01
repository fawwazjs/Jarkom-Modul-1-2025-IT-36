# Laporan Resmi Jarkom Modul 1 Kelompok K-36

## Anggota

| Nama 				| NRP		|
|-------------------------------|---------------|
| Ahmad Wildan Fawwaz		| 5027241001 	|
| Muhammad Rakha Hananditya R.	| 5027241015 	|

## Walkthrough
1.	Untuk mempersiapkan pembuatan entitas selain mereka, Eru yang berperan sebagai Router membuat dua Switch/Gateway. Dimana Switch 1 akan menuju ke dua Ainur yaitu Melkor dan Manwe. Sedangkan Switch 2 akan menuju ke dua Ainur lainnya yaitu Varda dan Ulmo. Keempat Ainur tersebut diberi perintah oleh Eru untuk menjadi Client.
2.	Karena menurut Eru pada saat itu Arda (Bumi) masih terisolasi dengan dunia luar, maka buat agar Eru dapat tersambung ke internet.
3.	Sekarang pastikan agar setiap Ainur (Client) dapat terhubung satu sama lain.
4.	Setelah berhasil terhubung, sekarang Eru ingin agar setiap Ainur (Client) dapat mandiri. Oleh karena itu pastikan agar setiap Client dapat tersambung ke internet.
5.	Ainur terkuat Melkor tetap berusaha untuk menanamkan kejahatan ke dalam Arda (Bumi). Sebelum terjadi kerusakan, Eru dan para Ainur lainnya meminta agar semua konfigurasi tidak hilang saat semua node di restart.
6.	Setelah semua Ainur terhubung ke internet, Melkor mencoba menyusup ke dalam komunikasi antara Manwe dan Eru. Jalankan file berikut (link file) lalu lakukan packet sniffing menggunakan Wireshark pada koneksi antara Manwe dan Eru, lalu terapkan display filter untuk menampilkan semua paket yang berasal dari atau menuju ke IP Address Manwe. Simpan hasil capture tersebut sebagai bukti.
7.	Untuk meningkatkan keamanan, Eru memutuskan untuk membuat sebuah FTP Server di node miliknya. Lakukan konfigurasi FTP Server pada node Eru. Buat dua user baru: ainur dengan hak akses write&read dan melkor tanpa hak akses sama sekali ke direktori shared. Buktikan hasil tersebut dengan membuat file teks sederhana kemudian akses file tersebut menggunakan kedua user.
8.	Ulmo, sebagai penjaga perairan, perlu mengirimkan data ramalan cuaca ke node Eru. Lakukan koneksi sebagai client dari node Ulmo ke FTP Server Eru menggunakan user ainur. Upload sebuah file berikut (link file). Analisis proses ini menggunakan Wireshark dan identifikasi perintah FTP yang digunakan untuk proses upload.
9.	Eru ingin membagikan "Kitab Penciptaan" di (link file) kepada Manwe. Dari FTP Server Eru, download file tersebut ke node Manwe. Karena Eru merasa Kitab tersebut sangat penting maka ia mengubah akses user ainur menjadi read-only. Gunakan Wireshark untuk memonitor koneksi, identifikasi perintah FTP yang digunakan, dan uji akses user ainur.
10.	Melkor yang marah karena tidak diberi akses, mencoba melakukan serangan dengan mengirimkan banyak sekali request ke server Eru. Gunakan command ping dari node Melkor ke node Eru dengan jumlah paket yang tidak biasa (spam ping misalnya 100 paket). Amati hasilnya, apakah ada packet loss? Catat average round trip time untuk melihat apakah serangan tersebut mempengaruhi kinerja Eru.
11.	Sebelum era koneksi aman, Eru sering menyelinap masuk ke wilayah Melkor. Eru perlu masuk ke node tersebut untuk memeriksa konfigurasi, namun ia tahu Melkor mungkin sedang memantau jaringan. Buktikan kelemahan protokol Telnet dengan membuat akun dan password baru di node Melkor kemudian menangkap sesi login Eru ke node Melkor menggunakan Wireshark. Tunjukkan bagaimana username dan password dapat terlihat sebagai plain text. 
12.	Eru mencurigai Melkor menjalankan beberapa layanan terlarang di node-nya. Lakukan pemindaian port sederhana dari node Eru ke node Melkor menggunakan Netcat (nc) untuk memeriksa port 21, 80, dalam keadaan terbuka dan port rahasia 666 dalam keadaan tertutup.
13.	Setelah insiden penyadapan Telnet, Eru memerintahkan semua koneksi administratif harus menggunakan SSH (Secure Shell) untuk mengamankan jaringan. Lakukan koneksi SSH dari node Varda ke Eru. Tangkap sesi tersebut menggunakan Wireshark. Analisis dan jelaskan mengapa username dan password tidak dapat dilihat seperti pada sesi Telnet. Tunjukkan paket-paket terenkripsi dalam hasil capture sebagai bukti keamanan SSH.

14.	Setelah gagal mengakses FTP, Melkor melancarkan serangan brute force terhadap  Manwe. Analisis file capture yang disediakan dan identifikasi upaya brute force Melkor. 
(link file) nc 10.15.43.32 3401
15.	Melkor menyusup ke ruang server dan memasang keyboard USB berbahaya pada node Manwe. Buka file capture dan identifikasi pesan atau ketikan (keystrokes) yang berhasil dicuri oleh Melkor untuk menemukan password rahasia.
(link file) nc 10.15.43.32 3402
16.	Melkor semakin murka ia meletakkan file berbahaya di server milik Manwe. Dari file capture yang ada, identifikasi file apa yang diletakkan oleh Melkor.
	(link file) nc 10.15.43.32 3403
17.	Manwe membuat halaman web di node-nya yang menampilkan gambar cincin agung. Melkor yang melihat web tersebut merasa iri sehingga ia meletakkan file berbahaya agar web tersebut dapat dianggap menyebarkan malware oleh Eru. Analisis file capture untuk menggagalkan rencana Melkor dan menyelamatkan web Manwe.
(link file) nc 10.15.43.32 3404
18.	Karena rencana Melkor yang terus gagal, ia akhirnya berhenti sejenak untuk berpikir. Pada saat berpikir ia akhirnya memutuskan untuk membuat rencana jahat lainnya dengan meletakkan file berbahaya lagi tetapi dengan metode yang berbeda. Gagalkan lagi rencana Melkor dengan mengidentifikasi file capture yang disediakan agar dunia tetap aman.
(link file) nc 10.15.43.32 3405
19.	Manwe mengirimkan email berisi surat cinta kepada Varda melalui koneksi yang tidak terenkripsi. Melihat hal itu Melkor sipaling jahat langsung melancarkan aksinya yaitu meneror Varda dengan email yang disamarkan. Analisis file capture jaringan dan gagalkan lagi rencana busuk Melkor.
	(link file) nc 10.15.43.32 3406
20.	Untuk yang terakhir kalinya, rencana besar Melkor yaitu menanamkan sebuah file berbahaya kemudian menyembunyikannya agar tidak terlihat oleh Eru. Tetapi Manwe yang sudah merasakan adanya niat jahat dari Melkor, ia menyisipkan bantuan untuk mengungkapkan rencana Melkor. Analisis file capture dan identifikasi kegunaan bantuan yang diberikan oleh Manwe untuk menggagalkan rencana jahat Melkor selamanya.
(link file) nc 10.15.43.32 3407

Walkthrough
No. 14
Statistics > Capture File Properties

http.response && !data-text-lines contains "Invalid credentials"
Result: Frame 500320
Request in Frame: 500315

Go > Go to packet > 500315

]t]EN@@Qe^@R 8|
ja=POST /login.php HTTP/1.1 
Host: 192.168.129.101:8000 
User-Agent: Fuzz Faster U Fool v2.1.0-dev 
Content-Length: 42 
Content-Type: application/x-www-form-urlencoded 
Accept-Encoding: gzip 
 
username=n1enna&password=y4v4nn4_k3m3nt4r1


Follow HTTP Stream ^
n1enna:y4v4nn4_k3m3nt4r1

Transmission Control Protocol, Src Port: 42334, Dst Port: 8000, Seq: 1, Ack: 1, Len: 233
    Source Port: 42334
    Destination Port: 8000
    [Stream index: 41824]
    [Stream Packet Number: 4]
    [Conversation completeness: Complete, WITH_DATA (31)]
    [TCP Segment Len: 233]
    Sequence Number: 1    (relative sequence number)
    Sequence Number (raw): 3964838560
    [Next Sequence Number: 234    (relative sequence number)]
    Acknowledgment Number: 1    (relative ack number)
    Acknowledgment number (raw): 3292055442
    1000 .... = Header Length: 32 bytes (8)
    Flags: 0x018 (PSH, ACK)
    Window: 502
    [Calculated window size: 64256]
    [Window size scaling factor: 128]
    Checksum: 0xab7c [unverified]
    [Checksum Status: Unverified]
    Urgent Pointer: 0
    Options: (12 bytes), No-Operation (NOP), No-Operation (NOP), Timestamps
    [Timestamps]
    [SEQ/ACK analysis]
    TCP payload (233 bytes)
Packet Details ^

]t]EN@@Qe^@R 8|
ja=POST /login.php HTTP/1.1 
Host: 192.168.129.101:8000 
User-Agent: Fuzz Faster U Fool v2.1.0-dev 
Content-Length: 42 
Content-Type: application/x-www-form-urlencoded 
Accept-Encoding: gzip 
 
username=n1enna&password=y4v4nn4_k3m3nt4r1

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



Setiap paket umumnya hanya memuat satu keystroke. Untuk otomasi dan menampilkan seluruh stream keystroke dari target menggunakan tshark.

Data keystroke tersimpan pada field HID (usbhid.data).
Command tshark:
tshark -r /home/fedora/Downloads/hiddenmsg.pcapng   -Y 'usb.transfer_type == 0x01 && !usb.src == host'   -T fields -e usbhid.data



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




Output:
UGx6X3ByMHYxZGVfeTB1cl91czNybjRtZV80bmRfcDRzc3cwcmQ=

What is Melkor's secret message?
Format: string
> Plz_pr0v1de_y0ur_us3rn4me_4nd_p4ssw0rd
Congratulations! Here is your flag: KOMJAR25{K3yb0ard_W4rr10r_gz6mwpsdLTyJlTNVHeusOzDP0}

Ada sama dengan di akhir -> Base64. Decode:




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


Jumlah IP pada PCAP ada 5. IP 10.6.13.102 merupakan IP pertama yang meminta request SYN, Jumlah Bytes yang dikirim cukup besar, Merupakan IP private dan bukan IP eksternal dengan geolokasi. Potensi Malware.
Jadi filter pertama:
ip.src = 10.6.13.102



FTP menjadi protokol dengan persentase Bytes terbesar pada PCAP. Memiliki potensi membawa malware. FTP didesain untuk mentransfer file.

Filter ke 2:
ftp



Secara langsung dapat terlihat dua frame yang menarik, yaitu frame 227 dan frame 231.
Sehingga:
USER ind@psg420.com
PASS PASS {6r_6e#TfT1p



Dua command FTP yang menarik perhatian:
RETR <filename> -> Client downloads a file from server.
STOR <filename> -> Client uploads a file to server.

STOR pada file PCAP tidak menunjukkan adanya file malware dan hanya berupa logs. Sedangkan pada RETR terdapat 5 file yang muncul dan kemungkinan berbahaya (File exe).

Jumlah ada 5: q.exe, w.exe, e.exe, r.exe, t.exe




Lihat detail SIZE dari setiap file malware
ftp && ip.src == 10.6.13.102 && ftp.request.command == "SIZE"
Mencari IP dan port yang digunakan server untuk terhubung ke client dan mengunduh file malware.

Pindah ke SETUP frame: 241



File Transfer Protocol (FTP)
    227 Entering Passive Mode (216,55,163,106,199,145)\r\n
        Response code: Entering Passive Mode (227)
        Response arg: Entering Passive Mode (216,55,163,106,199,145)
        Passive IP address: 216.55.163.106
        Passive port: 51089

Filter paket yang datang (source) dari port 51089 dengan filter:
tcp.port == 51089



Kemudian pilih salah satu paket dan Follow TCP Stream

Isi dari TCP stream tersebut adalah Isi dari q.exe.
Pilih:
Entire Conversations -> Show As Raw -> Save As -> q.exe



Gunakan command sha256sum untuk mengetahui hash dari q.exe:




Output:
ca34b0926cdc3242bbfad1c4a0b42cc2750d90db9a272d92cfb6cb7034d2a3bd

w.exe:



Setup Frame: 1111






SIZE -> Setup Frame -> Port server: 59785
tcp.port == 59785
Follow TCP Stream
Save as w.exe
sha265sum


e.exe:



Setup Frame: 1295



Port: 49506

tcp.port == 49506







r.exe:



Setup Frame: 2445



Port: 60899
tcp.port == 60899







t.exe:



Setup Frame: 2643



Port: 50157
tcp.port == 50157







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

No. 17


Statistics > Conversations
Traffic terbanyak adalah antara IP 10.6.27.102 dan 107.180.50.162. Sehingga kemungkinan besar file malware dikirim antara keduanya. Filter:
ip.addr == 10.6.27.102 && ip.addr == 107.180.50.162

Statistics > Protocol Hierarchy





Volume traffic kebanyakan dari http. Kemungkinan besar mengirim malware.

Filter:
http

Semuanya:
http && ip.addr == 10.6.27.102 && ip.addr == 107.180.50.162


Urutan file pertama yang muncul berdasarkan GET (Server 107.180.50.162 (IP eksternal) mengirimkan file berdasarkan request client IP 10.6.27.102 (privat)):
71    29.202755    10.6.27.102    107.180.50.162    HTTP    343    GET /Documents/Invoice&MSO-Request.doc HTTP/1.1
 
Urutan file kedua yang muncul berdasarkan GET (Server 107.180.50.162 (IP eksternal) mengirimkan file berdasarkan request client IP 10.6.27.102 (privat)):
356    38.470797    10.6.27.102    107.180.50.162    HTTP    361    GET /knr.exe HTTP/1.1 

File -> Export Objects -> HTTP -> knr.exe -> Save



sha256sum knr.exe



Output:
749e161661290e8a2d190b1a66469744127bc25bf46e5d0c6f2e835f4b92db18

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


No. 18



Statistics > Protocol Hierarchy

3 protokol ada pada file PCAP ini dengan urutan jumlah bytes:
TLS
HTTP
SMB

Alasan memilih SMB sebagai kemungkinan tempat malware:
1. Soal menyatakan malware diletakkan menggunakan metode berbeda. Soal 17 menggunakan HTTP sehingga tidak mungkin file berada pada HTTP.
2. Soal ini tidak memberikan session key untuk decrypt protokol TLS. Sehingga tidak mungkin file disimpan di sana.

Buka FILE -> Export Objects -> SMB…



Di sini ada dua file yang kemungkinan merupakan malware, yaitu kedua file dengan ekstensi .exe.


Save kedua file. Gunakan command sha256sum untuk mengetahui hash dari kedua file.



Output untuk file: %5cWINDOWS%5coiku9bu68cxqenfmcsos2aek6t07_guuisgxhllixv8dx2eemqddnhyh46l8n_di.exe 

cf99990bee6c378cbf56239b3cc88276eec348d82740f84e9d5c343751f82560



Output untuk file:
%5cWINDOWS%5cd0p2nc6ka3f_fixhohlycj4ovqfcy_smchzo_ub83urjpphrwahjwhv_o5c0fvf6.exe 

59896ae5f3edcb999243c7bfdc0b17eb7fe28f3a66259d797386ea470c010040



7054    1096.833911    10.6.26.110    10.6.26.6    SMB    219    NT Create AndX Request, FID: 0x4002, Path: \WINDOWS\d0p2nc6ka3f_fixhohlycj4ovqfcy_smchzo_ub83urjpphrwahjwhv_o5c0fvf6.exe

7932    1096.944375    10.6.26.110    10.6.26.6    SMB    219    NT Create AndX Request, FID: 0x4003, Path: \WINDOWS\	

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


No. 19

Dalam sending email, protokol yang digunakan adalah SMTP.
Filter:
smtp



Untuk mengetahui konten dari email yang dikirim tanpa terbagi-bagi menjadi paket-paket, maka kita bisa melakukan Follow TCP Stream



Seluruh isi dari email bisa dibaca.

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



No. 20



Statistics > Protocol Hierarchy

TLS menjadi protokol dengan persentase Bytes terbesar pada PCAP. Memiliki potensi membawa malware.
Filter:
tls	



IP 10.4.1.101 merupakan IP dengan jumlah percakapan terbanyak dengan jumlah Bytes yang dikirim cukup besar pula, Merupakan IP private dan bukan IP eksternal dengan geolokasi. Potensi Malware.

Lihat detail paket Server Hello -> Cipher Suite:
TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256

Soal hanya membutuhkan TLS sebagai jawaban, tapi dari sini kita dapat mengetahui bahwa enkripsi yang digunakan oleh TLS adalah AES_128_GCM

TLS bersifat ECDHE di mana membutuhkan client-side pre-master secrets (SSLKEYLOGFILE) (file log key dari client)

Import file key log:
Edit -> Preferences -> Protocols -> TLS -> (Pre)-Master-Secret log filename -> Browse… -> keyslogfile.txt (sudah disediakan) -> Apply -> OK



Sekarang paket TLS sudah didekripsi dan muncul paket-paket dengan protokol HTTP.



Gunakan filter:
http && http.request.method == "GET"




Export file:
File -> Export Objects -> HTTP… -> invest_20.dll -> Save -> invest_20.dll



Gunakan command sha256sum untuk mengetahui hash dari invest_20.dll.



Output:
31cf42b2a7c5c558f44cfc67684cc344c17d4946d3a1e0b2cecb8eb58173cb2f

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




## Kendala Pengerjaan
