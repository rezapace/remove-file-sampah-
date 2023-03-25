# Remove File Sampah

Script ini akan menghapus file sampah pada Windows 10 dengan 1 kali klik. File sampah yang akan dihapus adalah:

- "C:\Windows\Prefetch"
- "C:\Users\R\AppData\Local\Temp"
- "C:\Windows\Temp"

## Penjelasan Script

```
Get-ChildItem -Path "C:\Windows\Temp" *.* -Recurse | Remove-Item -Force -Recurse
```

Script di atas akan menghapus semua file dengan ekstensi apa saja pada direktori "C:\Windows\Temp" beserta subdirektorinya.

```
Get-ChildItem -Path "C:\Users\R\AppData\Local\Temp" *.* -Recurse | Remove-Item -Force -Recurse
```

Script di atas akan menghapus semua file dengan ekstensi apa saja pada direktori "C:\Users\R\AppData\Local\Temp" beserta subdirektorinya.

```
Get-ChildItem -Path "C:\Windows\Prefetch" *.* -Recurse | Remove-Item -Force -Recurse
```

Script di atas akan menghapus semua file dengan ekstensi apa saja pada direktori "C:\Windows\Prefetch" beserta subdirektorinya.

```
Clear-RecycleBin -Force
```

Script di atas akan menghapus semua file yang ada di recycle bin.

## Cara Menggunakan

1. Buka PowerShell dengan cara klik kanan pada Start Menu dan pilih "Windows PowerShell".
2. Copy script di atas dan paste ke PowerShell.
3. Tekan Enter untuk menjalankan script.
4. Tunggu hingga proses selesai.
5. File sampah pada direktori yang telah disebutkan di atas akan terhapus.