---
layout: post  
title: Amazon đã phát triển phương pháp mới để Alexa có thể trả lời cho những câu hỏi phức tạp.
comments: true  
category: general
tags: []
---

## Amazon đã phát triển phương pháp mới để Alexa có thể trả lời cho những câu hỏi phức tạp.


 
2019-08-02: Bài viết của Darrell Etherington [Etherington](https://jp.techcrunch.com/contributor/darrell-etherington/)

![image](/res/Alexa/amazon-alexa-ios.jpg)

Team dự án Alexa AI của Amazon đã phát triển phương pháp training mới để nâng cao xử lý những câu hỏi phức tạp. Mr Abdalghani Abujabal là Team lead của dự án đang giới thiệu về phương pháp mới này trên blog cá nhân. Được kết hợp giữa 2 phương pháp thông thường sẽ xung đột với nhau đó là Knowledge Graph được customize và search dựa vào keyword.

Mr Abujabal đưa ra câu hỏi như thế này: [Bộ phim nào mà Nolan đã đạt giải Osca nhưng lại trượt Golden Globe?]. Để trả lời được câu hỏi này thì cần phải có nhiều dữ liệu. Xác định “Nolan” tên là Christopher Nolan một đạo diễn phim. Tìm ra những bộ phim mà ông đã đạo diễn,（để tạo được danh sách kết quả thì cần suy đoán “Nolan” là một đạo diễn）, sau đó sẽ tiến hành tham chiếu chéo dữ liệu của list A “ những tác phẩm đã đạt giải Osca” với list B”những tác phẩm đã đạt giải Golden Globel, từ đó lọc ra tác phẩm có trong list A mà không có trong list B.

Để trả lời chính xác những câu hỏi khó như thế này, với phương pháp này đầu tiên là sẽ cố gắng tập hợp những dữ liệu mang tính bao hàm. Đầu tiên thì sẽ có nhiều dữ liệu không chính xác nhưng sẽ xây dựng knowledge graph tự động bằng cách sử dụng các thuật toán. Thuật toán này do chính team nghiên cứu xây dựng cho nên sau khi loại bỏ thông tin rác sẽ đưa đến kết quả mang tính chính xác cao.

Hệ thống mà Amazon đã đưa ra thì đơn giản. Hơn thế nữa đó là kết hợp 2 phương pháp đơn giản. Đầu tiên cơ bản là search web, ví dụ giống với việc input lên Google nội dung như thế này [Bộ phim nào mà Nolan đã đạt giải Osca nhưng lại trượt Golden Globe?] sử dụng nguyên văn câu hỏi tiến hành cross trên web và tìm ra kết quả (có rất nhiều web engine đang được sử dụng trên thực tế). Tiếp theo sẽ search 10 page được xếp hạng từ trên top, sẽ phân tích thành unit là tên và ngữ pháp đã được nhận biết.

Sau khi làm như vậy sẽ thêm vào data set kết quả đã thu thập được, Alexa AI sẽ tạo graph bằng cách tìm kiếm trong cấu trúc của các văn bản, sẽ đánh dấu vào văn bản quan trọng có nội dung là [Inception mà Nolan đã quay] sẽ làm giảm các thông tin. Bằng cách như vậy sẽ có thể tạo ad hoc - knowledge graph, và có thể xác định được “cornerstone”. Cornerstone cơ bản là giống với những từ đang có trong văn bản ban đầu đã được search.

Thuật toán sẽ sort bằng cách mark dữ liệu còn lại và trả về giá trị chính xác là [inception]. Amazon team đã phát hiện ra rằng điều này thực sự tốt hơn một cách tiếp cận phức tạp, chỉ tập trung vào tìm kiếm văn bản hoặc xây dựng một knowledge tùy chỉnh. Nhóm nghiên cứu tin rằng phương pháp này có thể được cải tiến hơn nữa. Ở những cuộc thảo luận khi đã trở nên sôi nổi bởi những câu đố khó khăn, nếu bạn hỏi smart speaker thì có thể giải quyết được. Tôi đang mong chờ ứng dụng này với tư cách một người dùng Alexa.



Người dịch sang Japanese：Kaori Koyama





**Trích từ nguồn :**

**Amazon develops a new way to help Alexa answer complex questions**

`https://jp.techcrunch.com/2019/08/02/2019-07-31-amazon-develops-a-new-way-to-help-alexa-answer-complex-questions/`

