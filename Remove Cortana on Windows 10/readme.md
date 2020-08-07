# Gỡ bỏ hoàn toàn Cortana trên Windows 10

Bắt đầu từ bản Windows 10 Ver 2004, Microsoft đã bắt đầu biến Cortana thành Metro App, hoạt động độc lập với Windows Search. Cho nên, các bạn có thể gỡ Cortana ra mà không hề ảnh hưởng đến khung tìm kiếm. Dưới đây là cách gỡ.

# Cách gỡ bỏ hoàn toàn Cortana:

Các bạn mở Powershell với quyền Administrator >>> Copy code dưới vào >>> Enter

Get-AppxPackage -allusers Microsoft.549981C3F5F10 | Remove-AppxPackage

Còn icon trên thanh taskbar, các bạn chỉ cần chuột phải thanh taskbar >>> bỏ tích Show Cortana button là xong nhé.

# Cách cài lại Cortana:

Các bạn chỉ cần vào Microsoft Store tìm Cortana tải lại là được.

Link Microsoft Store: [Download Cortana](https://www.microsoft.com/en-us/p/cortana/9nffx4szz23l?irgwc=1&OCID=AID2000142_aff_7593_159229&tduid=%28ir__i0jkofdjywkftyv1xmdf30kppu2xigv3v6bwihvp00%29%287593%29%28159229%29%28%29%28UUwpUdUnU78036YYwYd%29&irclickid=_i0jkofdjywkftyv1xmdf30kppu2xigv3v6bwihvp00&activetab=pivot%3Aoverviewtab)

![Image](https://www.windowscentral.com/sites/wpcentral.com/files/styles/xlarge/public/field/image/2020/06/cortana-uninstall-windows-10_2020.jpg?itok=7iCoW4LA)
