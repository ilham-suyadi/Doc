# Text

| perintah | fungsi |
| ---      |    --- |
|head (nama file) | menampilkan baris text *awal*, secara default 10 baris|
|head (nama file 1) (nama file 2)  | head secara *multi file* |
|head -(number) (nama file) | menampilkan head dengan jumlah *baris* yang sesuai dengan number|
|head -c (number) (name file) | menampilkan head dengan *jumlah huruf* yang sesuai dengan number yang dimasukkan |
|tail (nama file) | menampilkan baris text *terakhir*, secara default 10 baris|
|tail -(number) (nama file) | menampilkan *baris* text terakhir sesuai dengan number input|
|tail -c -(number) (name file) | tail dengan *jumlah huruf* tertentu sesuai dengan number |
| (command) [ tail | mengabungkan command dengan tail|
|cat | melihat semua text yang ada di file|
|cat > (nama file baru) | membuat file baru|
|cat (old file) > (new file) | mengopy isi dari file lama ke file baru|
|cat (old file) (old file 2) > (new file) | mengopy isi dari dua file kedalam 1 file baru |
|cat -n (nama file) | menampilkan nomer di setiap baris|
|cat -e (nama file) | menganti akhir baris dengan $ |
|tac (nama file) | melihat text secara kebalik dari bawah ke atas |


> :memo: ***Catatan :*** head & tail akan mengangkap 1 paragraf sebagai 1 baris atau jika kalimat terus lanjut tanpa ganti baris maka di anggap 1 baris.
>
>**[** pengganti dari tanda **|** (garis lurus)
>
> tac (nama file) | head
