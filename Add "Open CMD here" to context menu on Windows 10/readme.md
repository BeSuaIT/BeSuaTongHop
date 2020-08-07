# Thêm "Open CMD here" vào menu khi giữ Shift+chuột phải trên Windows 10

Như các bạn đã biết, ở Windows 10, khi các bạn giữ Shift+chuột phải thì sẽ không còn thấy mục "Open command window here" mà thay vào đó là "Open Powershell window here". Dưới đây là cách đem lại mục đó khi giữ Shift+chuột phải.

Bước 1: Các bạn vào khung tìm kiếm, gõ "regedit" rồi tìm đến đường dẫn sau:

```
HKEY_CLASSES_ROOT\Directory\shell\cmd

HKEY_CLASSES_ROOT\Directory\Background\shell\cmd
```

Bước 2: (Bắt đầu từ bước này thì các bạn làm cả 2 đường dẫn trên như nhau nhé, mình sẽ gộp vào hướng dẫn chung cho đỡ dài): Chuột phải folder "cmd" >>> Permissions >>> Advanced >>> Change (cạnh TrustedInstaller)

Bước 3: Ở đây các bạn hãy nhập tên máy các bạn rồi bấm "Check Names" (Lưu ý là tên User của máy bạn, chứ không phải cái DESKTOP-XXXX)

![CMD](https://i.imgur.com/x69Npc3.jpg)

Sau khi "Check Names" xong các bạn ấn OK rồi tích vào phần như ảnh >>> Apply >>> OK

![CMD](https://www.windowscentral.com/sites/wpcentral.com/files/styles/xlarge/public/field/image/2017/05/replace-owner-subcontainters-cmd.jpg)

Bước 4: Tiếp tục quay lại bảng Permissions, chọn dòng "Administrators" >>> Tích vào ô "Full Control" >>> Apply >>> OK.

![CMD](https://www.windowscentral.com/sites/wpcentral.com/files/styles/mediumplus/public/field/image/2017/05/permissions-administrators-fullcontrol-cmd.jpg)

Bước 5: Quay lại registry, các bạn chuột phải vào "HideBasedOnVelocityId" >>> Rename >>> đổi tên thành "ShowBasedOnVelocityId". Tương tự đường dẫn "HKEY_CLASSES_ROOT\Directory\Background\shell\cmd" kia cũng làm như thế.

![CMD](https://www.windowscentral.com/sites/wpcentral.com/files/styles/xlarge/public/field/image/2017/11/background-showbasedonvelocityid.jpg)

![CMD](https://www.windowscentral.com/sites/wpcentral.com/files/styles/xlarge/public/field/image/2017/11/background-open-command-window-here.jpg)

# P/s: Mình có nghĩ đến chuyện làm file reg rồi nhưng vì ở đây mình không có quyền chỉnh sửa cho nên không thể sử dụng file reg cho nên các bạn chịu khó thủ công tí.
