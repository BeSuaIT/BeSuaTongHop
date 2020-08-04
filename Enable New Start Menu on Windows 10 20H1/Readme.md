# Kích hoạt Start Menu mới trên Windows 10 20H1

Như chúng ta đã biết, trên các diễn đàn, trang web đều đăng các bài nói về sự thay đổi của Windows 10 20H2 sắp tới, Tiêu biểu ở đây là Start Menu. Mình sẽ hướng dẫn các bạn kích hoạt nó mà không cần cập nhật lên Windows 10 20H2.

# Bước 1: Cập nhật Windows của các bạn lên mới nhất (kb4568831 - Bản vá ngày 31/7)

Link: [KB4568831](https://www.catalog.update.microsoft.com/Search.aspx?q=KB4568831)

Link thông tin các thay đổi của bản vá: [Changelogs](https://support.microsoft.com/en-us/help/4568831/windows-10-update-kb4568831)

# Bước 2: Sau khi cập nhật xong, các bạn hãy copy đoạn phía dưới vào notepad rồi save lại và chạy. Khởi động lại máy sẽ có sự thay đổi.

Windows Registry Editor Version 5.00
[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\FeatureManagement\Overrides\0\2093230218]
"EnabledState"=dword:00000002
"EnabledStateOptions"=dword:00000000
