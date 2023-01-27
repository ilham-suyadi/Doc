# ssl

1. masuk ke gitlab bash dengan perintah *docker exec -it gitlab bash*
2. add ssl.cert dan ssl.key ke dalam /etc/gitlab/ssl
3. jika menggunakan volume, bisa mengunakan volume tersebut dengan cara masuk ke volume dan ke directory config/ssl dan masukkan ssl.cert dan ssl.key
4. edit gitlab.rb dengan gambar di bawah ini

   - ![ssl](/assets/img/ssl.png)

5. reconfigure gitlab dengan perintah *gitlab-ctl reconfigure* jika anda berada di gitlab bash atau jika anda diluar gitlab bash bisa mengetikkan perintah *docker exec -i gitlab gitlab-ctl reconfigure*

> :memo: Jika ingin lebih rinci bisa mengunjungi [gitlab](https://docs.gitlab.com/omnibus/settings/ssl/)
