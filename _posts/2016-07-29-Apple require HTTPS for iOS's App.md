---
layout: post  
title: Apple require HTTPS for iOS's App.   
comments: true  
category: general
tags: []
---

## Bắt đầu từ tháng 1 năm 2017, sẽ yêu cầu các App của iOS sử dụng HTTPS để truy cập vào Web. Chú ý dành cho các developer. 


![image](/res/HTTPS for iOS's App/1.png)

Tại buổi trình bày về vấn đề Security của Worldwide Developers’Conference (WWDC), Apple đã thông báo hạn chót để tất cả các App trên App Store phải chuyển sang chức năng Security quan trọng đó được gọi là App Transport Security. Bắt đầu từ tháng 1 năm 2017.
	
App Transport Security (ATS) là chức năng được Apple giới thiệu trên iOS. Nếu ATS đang được kích hoạt thì các App khi truy cập vào Web service sẽ không dùng HTTP mà bắt buộc phải dùng HTTPS. Bởi lẽ, HTTPS sẽ mã hóa thông tin, từ đó các thông tin dữ liệu của User sẽ được an toàn.
	
Chữ “ S “ của HTTPS là chữ đầu tiên trong chữ secure có nghĩa là an toàn, có thể để ý thấy được bằng mắt thường trên trình duyệt khi đăng nhập vào tài khoản ngân hàng hay mail chẳng hạn. Tuy nhiên, các App trên Mobile khi truy cập vào Web thì cũng có nhiều khi không thông báo cho User vấn đề liên quan tới Security. Việc truy cập đó đang dùng HTTP hay là HTPPS thì User khó mà biết được.

	
ATS mặc dù được kích hoạt mặc định từ iOS 9 trở đi nhưng các developer có thể tự vô hiệu hóa nó từ trong chính App của họ. Đối với những App mà làm điều này thì sẽ truy cập vào Web bằng HTTP. Tuy nhiên điều này cũng chỉ có thể làm cho tới cuối năm nay. Về mặt kĩ thuật thì ATS yêu cầu TLS v1.2, ngoại trừ bulk data đang được mã hóa sẵn giống như Media streaming.
	
Đến cuối năm 2016 thì đối với tất cả các App đưa lên App Store sẽ bắt buộc phải kích hoạt ATS. Bây giờ thì các developer cũng sẽ làm dễ dàng vì đã có thông báo rõ ràng về kì hạn sẽ phải chuyển sang dùng HTPPS. Ngoài ra, các User cũng biết được và an tâm hơn khi truy cập từ các ứng dụng trên iPhone và iPad an toàn.
	
Với việc yêu cầu các developer sử dụng HTTPS, Apple đã tham gia vào một phong trào lớn là làm sao cho các dữ liệu online được an toàn. Mặc dù đang dần trở nên phổ biến phương thức an toàn chẳng hạn trên các trang đăng nhập, nhưng vẫn còn tồn tại nhiều phương thức truy cập bằng HTTP. Tuy vậy điều này sẽ dần dần thay đổi hoàn toàn sang sử dụng HTPPS. Tạp chí Wired đã có bài viết tốt tập hợp lại quá trình này.　　

↓

http://www.niemanlab.org/2016/04/wireds-making-the-long-and-slow-switch-to-https-and-it-wants-to-help-other-news-sites-do-the-same/


 **Trích từ nguồn :** 

` Webに接続するiOSアプリは2017年1月からHTTPSの使用が絶対条件になる、デベロッパーはご注意を`

` http://jp.techcrunch.com/2016/06/15/20160614apple-will-require-https-connections-for-ios-apps-by-the-end-of-2016/ `

