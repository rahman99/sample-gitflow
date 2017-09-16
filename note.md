# Langkah yang dilakukan

1. setelah membuat project, maka otomatis jadi membuat branch develop dan di git di push ke branch develop
2. coba tambahkan file note.md
3. sekarang akan memulai release. yaitu dengan 
    start release:
    ```sh
    $ git flow release start RELEASE [BASE]
    ```
4. maka sekarang branch akan berganti ke release/0.1
5. sekarang akan memulai release. yaitu dengan 
    publish release:
    ```sh
    $ git flow release publish 
        Missing argument <version>
        usage: git flow release [list] [-v]
            git flow release start [-F] <version>
            git flow release finish [-Fsumpk] <version>
            git flow release publish <name>
            git flow release track <name>
    ```
    
    jika ada pesan demikian maka coba git flow release publish list -v 
    maka hasilnya akan meminta untuk commit release terlebih dahulu.

    finish release:
    ```sh
    $ $ git flow release finish 0.1
    ```   

    maka git flow akan diubah ke branch master.

6. merging ke master.
    selanjutnya adalah push ke branch master.
7. coba buat file baru (misal note release 0.2)
8. buat fitur baru di note release 0.2 kemudian lakukan release

