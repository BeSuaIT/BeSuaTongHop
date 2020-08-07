# Hướng dẫn cài lại Microsoft Store cho Windows 10 Enterprise LTSC

Như các bạn biết, Windows 10 Enterprise LTSC là 1 bản Windows của Microsoft đã lượt bỏ hầu hết các Metro Apps (Microsoft Store, Cortana, ....) nhằm mục đích dành cho các máy yếu. Sau đây là cách cài lại Microsoft Store cho Windows 10 Enterprise LTSC.

Bước 1: Tải về file theo link dưới và giải nén ra.

Google Drive | Dự phòng
------------ | -------------
[Download Now](https://drive.google.com/file/d/1H12bkRJkYF3uioxJfB2OB5lEOIiI5pcX/view?usp=sharing) | [Download Now](https://www.upload.ee/files/12103839/MicrosoftStore-RS5.zip.html)

Bước 2: Chuột phải file "Add-Store.cmd" >>> Run as administrator và chờ 1 lúc.

Sau khi cài xong, nếu Microsoft Store không hoạt động thì bạn hãy copy lệnh dưới vào CMD với quyền administrator:

```
PowerShell -ExecutionPolicy Unrestricted -Command "& {$manifest = (Get-AppxPackage Microsoft.WindowsStore).InstallLocation + '\AppxManifest.xml' ; Add-AppxPackage -DisableDevelopmentMode -Register $manifest}"
```

Nếu vẫn không chạy được thì lại tiếp tục mở Run lên >>> Gõ "WSReset.exe" và Enter, lúc này chắc chắn thành công.

![Microsoft Store](https://21ak22.com/wp-content/uploads/2020/04/huong-dan-cai-dat-them-microsoft-store-cho-windows-10-ltsc-1.jpg)
