# Dokumentasi Packet Tracer

## Topologi Jaringan

![](https://i.ibb.co/JyxyFph/Whats-App-Image-2022-09-17-at-09-37-33.jpg)

Topologi diatas terdiri dari 2 Router dan 2 PC client dengan subneting

## Konfigurasi IP pada PC
![](https://i.ibb.co/74vFhMS/Whats-App-Image-2022-09-17-at-09-41-32.jpg)

PC1 IP
Address -> 192.168.1.2
Subnet Mask -> 255.255.255.0 
Gateway -> 192.168.1.1

## Konfigurasi IP pada router
![](https://i.ibb.co/37d12vf/Whats-App-Image-2022-09-17-at-09-46-26.jpg)
![](https://i.ibb.co/S3rgGBY/Whats-App-Image-2022-09-17-at-09-49-10.jpg)

Untuk setting static routing di cisco packet tracer menggunakan perintah:
#IP Route [destination] [subnet] [next hop address] 

Keterangan:
IP Route: Perintah membuat tabel routing
Static Destination: Network jaringan yang dituju
Subnet: Subnet mask jaringan yang dituju
Next Hop Address: IP dari router yang akan dilewati

## Test Ping
![](https://i.ibb.co/DpN6PbP/Whats-App-Image-2022-09-17-at-09-56-31.jpg)

![](https://i.ibb.co/8gRdDBW/Whats-App-Image-2022-09-17-at-09-58-41.jpg)

Pada gambar di atas PC2-192.168.3.3/24 tidak melakukan request ping dan hanya replay ping sebelumnya dari PC1-192.168.1.2/24 dan sudah memiliki daftar arp-a cache yaitu IP 192.168.1.1 (Router 1) dengan Physical / MAC Address 0001.9724.4801 sehingga untuk melakukan ping pada PC2-192.168.3.3/24 ke PC1-192.168.1.2/24 tidak terjadi RTO lagi.