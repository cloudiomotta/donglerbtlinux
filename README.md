# donglerbtlinux
Driver RTL8761B Linux

Se o comando resulta no ouput:
$ dmesg | egrep -i 'rtl_bt'
$ [    2.251752] Bluetooth: hci0: RTL: loading rtl_bt/rtl8761b_fw.bin
$ [    2.252974] bluetooth hci0: Direct firmware load for rtl_bt/rtl8761b_fw.bin failed with error -2
$ [    2.252978] Bluetooth: hci0: RTL: firmware file rtl_bt/rtl8761b_fw.bin not found

Indica que o driver Realtek RTL8761B está faltando. Baixe os arquivos binários disponíveis no repositório e copie-os para o diretório de drivers Bluetooth do seu Linux (/lib/firmware/rtl_bt/ no meu Ubuntu 20.04.3) com permissão de admin. Reinicie seu computador e seu problema deve estar resolvido.
