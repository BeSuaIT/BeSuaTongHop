# Thêm phần mềm vào menu chuột phải trên Windows

Cái này dành cho ai muốn tiện thì thêm thôi, không thích có thể bỏ qua. 

# Cách 1: Sử dụng Registry Editor.

Bước 1: Các bạn mở regedit lên truy cập đường dẫn:

```
HKEY_CLASSES_ROOT\Directory\Background\shell
```

Bước 2: chuột phải vào Folder "shell" >>> Key >>> Đặt tên folder đó. Tên Folder đó sẽ là tên sẽ hiển thị ở menu chuột phải.

Bước 3: Tiếp tục chuột phải Folder vừa tạo >>> Key >>> Đặt tên Folder là "command".

Bước 4: Copy đường dẫn của phần mềm bạn muốn thêm và String (Default) nó tạo sẵn trong Folder "command"

VD: Ở đây mình sẽ thêm Google Chrome vào menu chuột phải thì sẽ set như dưới (Nhớ vẫn giữ "...")

```
"C:\Program Files (x86)\Google\Chrome\Application\chrome.exe"
```

# Cách 2: Sử dụng Easy Context Menu.

Phần mềm này cũng khá dễ sử dụng, các bạn không phải làm theo cách rườm rà như trên.

Link Download: [Download Now](https://www.sordum.org/7615/easy-context-menu-v1-6/#:~:text=Easy%20Context%20Menu%20(ECM)%20lets,items%20you%20wish%20to%20add.)

![Image](https://www.sordum.org/wp-content/uploads/2014/03/easy_context_menu_main.png)

![Image](https://www.howtogeek.com/wp-content/uploads/2010/12/image24.png)
