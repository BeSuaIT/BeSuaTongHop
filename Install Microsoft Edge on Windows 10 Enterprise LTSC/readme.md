# Hướng dẫn cài Microsoft Edge cho Windows 10 Enterprise LTSC

Như các bạn biết, Windows 10 Enterprise LTSC là 1 bản Windows của Microsoft đã lượt bỏ hầu hết các Metro Apps (Microsoft Store, Cortana, ....) nhằm mục đích dành cho các máy yếu. Sau đây là cách cài lại Microsoft Edge cho Windows 10 Enterprise LTSC. Cái này là mình nói đến Microsoft Edge gốc chứ mình không nói đến Microsoft Edge Chromium nhé, bạn nào không muốn cài lại Microsoft Edge này thì link bản [Microsoft Edge Chromium](https://www.microsoft.com/en-us/edge) đây.

Bước 1: Tải file dưới về (32bit chọn x86, 64bit chọn x64) và giải nén ra copy 2 file .cab vào C:\Windows\System32

Phiên bản | Google Drive | Dự phòng
 ------------ | ------------ | -------------
x86 | [Download Now](https://drive.google.com/file/d/1Sz_2K40gvPP-AyYdoX8IF9MpgicEwOXb/view?usp=sharing) | [Download Now](https://www.upload.ee/files/12103838/Edge-10.0.17763.1_x86.rar.html)
x64 | [Download Now](https://drive.google.com/file/d/1Xfc9SO8AxAy1rQLnZ2o-cjqYL1orh3CZ/view?usp=sharing) | [Download Now](https://www.upload.ee/files/12103837/Edge-10.0.17763.1_x64.rar.html)

Bước 2: Mở Powershell với quyền administrator, copy từng lệnh dưới vào (lưu ý chạy xong lệnh 1 mới copy lệnh 2)

```
x86:
* dism /online /add-package /packagepath:Microsoft-Windows-Internet-Browser-Package-x86-10.0.17763.1.cab
* dism /online /add-package /packagepath:Microsoft-Windows-Internet-Browser-Package-x86-10.0.17763.1-en-US.cab

x64:
* dism /online /add-package /packagepath:Microsoft-Windows-Internet-Browser-Package-amd64-10.0.17763.1.cab
* dism /online /add-package /packagepath:Microsoft-Windows-Internet-Browser-Package-amd64-10.0.17763.1-en-US.cab
```

Bước 3: Sau khi chạy xong 2 lệnh trên, tiếp tục copy lệnh dưới vào

```
Add-AppxPackage -DisableDevelopmentMode -Register $Env:SystemRoot\SystemApps\Microsoft.MicrosoftEdge_8wekyb3d8bbwe\AppxManifest.xml
```

![Microsoft Edge](https://scontent.fhan2-6.fna.fbcdn.net/v/t1.0-9/s960x960/43237930_1097171220452261_490187800063246336_o.jpg?_nc_cat=103&_nc_sid=8024bb&_nc_ohc=fhfqIsV09jIAX8wXGsL&_nc_ht=scontent.fhan2-6.fna&_nc_tp=7&oh=3caf65d51451f1fb656b2bc12931137c&oe=5F4E91CA)
