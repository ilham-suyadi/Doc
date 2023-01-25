# menganti port ssh

## 1. edit di sshd_config

1. masuk ke file config dengan memasukkan perintah :

    ```sh
    vi /etc/ssh/sshd_config
    ```

2. selanjutnya mengubah atau menambah port ssh :
   sebelum mengubah port ssh:
   ![sebelum ganti ssh](/assets/img/linux-sebelum%20mengubah%20port%20ssh.png)
   sesudah mengubah port ssh:
3. memasukkan port baru di ssh daemon dengan perintah di bawah ini:

   ```sh
   semanage port -a -t ssh_port_t -p tcp (port)
   semanage port -m -t ssh_port_t -p tcp (port)
   ```

    ![ssh daemon](../assets/img/linux-ssh%20daemon.png)
4. merestart sshd :

   ```sh
   systemctl restart sshd
   ```

   ![restart sshd](../assets/img/restart%20sshd.png)

5. mengupdate firewall :

   ```sh
   firewall-cmd --add-port=(port)/tcp --permanent
   firewall-cmd --remove-service=ssh --permanent
   ```

    ![firewall](../assets/img/linux-mengubah%20firewall.png)

> :link: [Referensi]<https://docs.rackspace.com/support/how-to/change-the-ssh-port-in-centos-and-redhat/>
