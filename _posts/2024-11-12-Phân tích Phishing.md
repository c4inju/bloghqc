---
layout: post
title:  "Phishing khách hàng X"
description: Một ngày đẹp trời, khách hàng X nhận được hàng loạt Email lạ ....
tags: phishing malware analysis
---
## I. Ngày xửa ngày xưa ....
Vào ngày nọ trong tháng 11, khách hàng gửi cho đội ngũ giám sát một tập tin "lạ". Một số nhân viên nhận được email, tải xuống và đã nhấn vào tập tin.

[Link tải lab](https://github.com/mikesiko/PracticalMalwareAnalysis-Labs)

## II. Kiểm tra
Hash: 4d569f250bdebee74229eff3698629f3a53151f8
![Image]()
Có thể thấy rằng tập tin này chưa từng được submit lên Virustotal.

Mở tập tin trong SandBox điểm kiểm tra
![Image]()
Trong tập tin PDF chỉ có 1 page, và có 1 button. Button này sẽ dẫn đến link Authentication của Google.

Kẻ tấn công lợi dụng chức năng redirect của Authentication của Google để lừa người dùng click vào và redirect sang trang giả mạo đăng nhập Microsoft.

## III. Kết luận
IoC:
Các dạng tấn công phishing càng trở nên chuyên nghiệp, khó để nhận biết đối với người dùng thông thường.

