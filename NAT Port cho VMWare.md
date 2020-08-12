# Nat port dịch vụ trên WMWare

## 1. Chọn card mạng VM8(NAT)	
<img src="https://imgur.com/60XkTmM.png">

## 2. Kiểm tra IP của máy ảo
```sh
ip a
```
<img src="https://imgur.com/SuJoodi.png">

`ip máy ảo: 192.168.157.132`

## 3. Cấu hình mạng VM8
#### 3.1  Chọn Edit => Virtual Network Editor
<img src="https://imgur.com/UsSBN1C.png">

### 3.2 Chọn NAT Setting
<img src="https://imgur.com/iAtiLvc.png">

### 3.3 Chọn ADD
<img src="https://imgur.com/6QSW2yi.png">

### 3.4 Điền các thông tin cần thiết:
<img src="https://imgur.com/wdoC5kl.png">

- Host port: Cổng port của máy vật lý
- Type: Chọn giao thức kết nối
- Virtual machine IP address: IP của máy ảo
- Vitual machine port: Port của máy ảo


### 3.5 Sau khi cấu hình xong => Ok
<img src="https://imgur.com/Y1UMfZG.png">

## 4. Kiểm tra
- Sử dụng MobaExtern: điền IP của máy thật, sử dụng port 8080 vừa điền:
<img src="https://imgur.com/RCcLWSH.png">
- Hiển thị kết nối thành công
<IMG SRC="https://imgur.com/w2jxsOp.png">
