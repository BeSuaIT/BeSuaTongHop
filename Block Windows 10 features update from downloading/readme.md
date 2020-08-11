# Chặn Windows 10 cập nhật tính năng, chỉ cập nhật bản vá.

Mẹo này dành cho ai không muốn lên các bản Windows mới hơn nhưng vẫn muốn nhận các bản cập nhật vá. Dưới đây là hướng dẫn

Lưu ý: 
* Theo mình thấy thì cách này tạm thời không có tác dụng cho những ai đang xài bản Home.
* Mình không đóng file reg vì cái này tuỳ theo vào từng phiên bản.
* Cách này cũng có thể áp dụng cho ai không cập nhật được lên 2004, khi đến bước 3, các bạn set giá trị là "2004" rồi Check For Update là được.

Bước 1: Các bạn mở Registry Editor lên, vào đường dẫn

```
Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate
```

Nếu ở đây không có folder "WindowsUpdate" thì các bạn chuột phải vào Folder "Windows" >>> New >>> Key rồi đặt tên là "WindowsUpdate" nhé.

Bước 2: Chuột phải trong Folder "WindowsUpdate" >>> New >>> DWORD >>> Đặt tên là "TargetReleaseVersion" rồi set giá trị là "1".

Bước 3: Tiếp tục chuột phải trong Folder "WindowsUpdate" >>> New >>> String >>> Đặt tên là "TargetReleaseVersionInfo" rồi set theo phiên bản mà bạn đang dùng.

VD: minh đang dùng 1909 thì mình sẽ set giá trị là "1909". 

Lúc này các bạn thử vào "Check For Update" xem có tác dụng không nhé.

![Image](https://scontent.fhan2-2.fna.fbcdn.net/v/t1.0-9/84028891_1225053497838989_7212047470776088998_n.jpg?_nc_cat=111&_nc_sid=ca434c&_nc_ohc=jDUl-gGnzH8AX88RhIU&_nc_ht=scontent.fhan2-2.fna&oh=795832027e5ae5fc97d0956460da6a31&oe=5F57C587)
