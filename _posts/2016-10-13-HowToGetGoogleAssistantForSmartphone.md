---
layout: post  
title: Phương pháp tích hợp Google Assistant vào smartphone của bạn chỉ với 2 dòng code.  
comments: true  
category: general
tags: []
---

## Phương pháp tích hợp Google Assistant vào smartphone của bạn chỉ với 2 dòng code.


 
2016-10-13: Bài viết của Devin [Coldewey](http://jp.techcrunch.com/contributor/devinjp/ "Coldewey")

![image](/res/GoogleAssistantForSmartphone/1.png)

Dù có thể có nhiều người muốn trải nghiệm Google Assistant nhưng cũng không phải ai cũng hứng thú với Pixel. Và bây giờ thì có thông tin tốt cho những người như bạn đó là chỉ cần viết 2 dòng code đơn giản vào structure file thôi. Và cũng kèm theo một tin không hay đó là thiết bị của bạn cần phải root, bất kể là từ nhà sản xuất nào, loại thiết bị nào cũng đều hoạt động bình thường được.  
  **Cảnh báo！　Nguy hiểm！**    
Điều này bạn phải hiểu được việc bạn đang là gì nhé! Nếu lạm dụng những đặc quyền của root và bootloaders thì thiết bị của bạn có khi là sẽ trở thành thứ để chận giấy thôi. Đầu tiên là backup lại – có nhiều người dùng đang thông báo về rủi ro này.  
Nói tới cách làm này thì người dùng và shiba inu [brianelv](http://forum.xda-developers.com/member.php?u=5968460 "brianelv") của forum **XDA** đã cung cấp cách làm chi tiết và list các loại thiết bị đã thành công trên [thread](http://forum.xda-developers.com/android/software/guide-how-to-enable-google-assistant-t3477879/ "thread"). Ngoài ra, trên **Lifehacker** cũng đã có [hướng dẫn](http://lifehacker.com/how-to-get-google-assistant-on-any-phone-running-androi-1787706402 "hướng dẫn") chi tiết tương tự.  
Công việc trước tiên hơn hết đó là Nougat phải đang được install. Sau khi Root, sử dụng File Explore sẽ tìm thấy build.prop trên Root/System. Tìm 2 name và điều chỉnh lại giá trị như bên dưới. (Nếu không tìm thấy name thì có thể thêm mới)  

`ro.product.model=Pixel XL`  
`ro.opa.eligible_device=true`  

Sau đó save lại và reboot, đi tới Setting > Apps, chọn Google, xóa dữ liệu và cash. Thực hiện xong và reload thì Assistant sẽ được tích hợp vào, nhấn giữ nút HOME sẽ khởi động lại thiết bị.    

Đối với những ai không thể root thì có thể unlock bootloaders. Bạn cần thông qua customize recovery image và fastboot trong build – in. Thực ra, với cách làm này đang có nhiều cảnh báo rủi ro. Cái này có lẽ là ở vấn đề tính tương tác bổ trợ của file build.prop.  
Mit Panchani đã hướng dẫn cách làm cụ thể ở video bên dưới.   
                     [Click vào đây!](https://youtu.be/hjt4karDZNM "Click vào đây!")  
Sau khi uninstall toàn bộ Google App, sẽ bắt đầu thực hiện. Download file về [tại đây](https://www.androidfilehost.com/?w=files&flid=121914 "tại đây") (cảm ơn FaserF), sau đó flash những file đó đầu tiên là file “GoogleAssistantVelvet.zip”, tiếp theo là file “GoogleAssistantBuildProp.zip”. Thực hiện reboot. Bấm OK tất cả để Google cho phép thêm yêu cầu mới. Và sau đó bạn nên tắt đi để thiết bị chạy.  

Có risk! Nếu không làm thì hơn… Có thể sẽ xảy ra những điều như vậy. Có vẻ như Assistant không phải là một chức năng thú vị. Dù vậy thì bạn có làm không? Vâng tôi đã thử làm rồi đấy!  

Người dịch sang Japanese：iwatani (a.k.a. [hiwa](http://goo.gl/ovDV "hiwa"))




**Trích từ nguồn :** 

**http://jp.techcrunch.com/2016/10/13/20161012add-google-assistant-to-your-phone-by-tweaking-two-lines-of-code/**

`http://jp.techcrunch.com/2016/10/13/20161012add-google-assistant-to-your-phone-by-tweaking-two-lines-of-code/`

