---
layout: post
title: "[part 1] Tổng quan về Ruby on Rails - Ruby on Rails là gì ?"
date:   2016-08-05 15:23:11 +0700
author: Sưu tầm
comments: yes
image: ruby-on-rails.jpg
---

Ruby là gì ?
Ruby là một ngôn ngữ lập trình. Nó được tạo ra khoảng 20 năm trước bởi Yukihiro “Matz” Matsumoto. Bằng nhiều phương pháp kiểm chứng thông dụng, Ruby nằm trong top ten về sự phổ biến, mặc dù nó thường ở vị trí thứ 10 hay chừng đó, bởi vì sự lớn mạnh của Rails. Giống như ngôn ngữ Java hay C, Ruby là một ngôn ngữ lập trình có thể dùng cho nhiều mục đích (general-purpose programming language), mặc dù nó được biết nhiều nhất trong việc lập trình web.
Bạn có thể tìm hiểu thêm về Ruby trên

- Wiki : [https://en.wikipedia.org/wiki/Ruby_(programming_language)](https://en.wikipedia.org/wiki/Ruby_(programming_language))
hoặc 
- Ruby : [https://www.ruby-lang.org/en/about/](https://www.ruby-lang.org/en/about/) .

Rails là gì ?

David Heinemeier Hansson đã tạo ra Rails, và ông ta đặt tên cho hệ thống này là “Ruby on Rails” vì nó được viết dựa trên ngôn ngữ Ruby, dù vậy người ta vẫn thường gọi nó là “Rails”. Ruby On Rails là một framework mã nguồn mở dùng cho ứng dụng web dùng ngôn ngữ lập trình Ruby, và nó còn là một full-stack framework. Để hiểu được Rails, đầu tiên bạn nên hiểu thế nào là 1 “stack”, và thế nào là 1 “full-stack”.
Stack: là thuật ngữ dùng để chỉ một cụm các công cụ đi kèm với nhau để thực thi hoàn chỉnh một nhiệm vụ vào đó. Ví dụ như sau đây là một stack phổ biến của PHP: LAMP. Stack “LAMP” bao gồm Linux (hệ điều hành) + Apache (web server) + MySQL (hệ quản trị cơ sở dữ liệu) + PHP.
Full-stack: có nghĩa là một stack đầy đủ, không nhất thiết phải thêm công cụ khác. Và Rails là một full-stack framework (mặc dù dĩ nhiên là nó cần hệ điều hành, và người ta thường chọn các hệ điều hành có nguồn gốc Unix như Linux hay Mac). Có nghĩa là Rails bao gồm web server, các hỗ trợ kết nối cơ sở dữ liệu và nhiều thứ khác nữa.
Chính vì vậy mà Rails rất mạnh mẽ. Và nó cũng trở nên khó tự học hơn (dĩ nhiên không có nghĩa là không thể tự học :) ).
Ruby On Rails chứa đựng các “quy ước” (convention) để việc bảo trì và phối hợp giữa các lập trình viên dễ dàng hơn (collaboration and maintenance). Những quy ước được tuân theo khi viết ra các Rails API (application programming interface). Nhờ đó một lập trình viên Rails có thể dễ dàng hiểu được code của lập trình viên khác.

Tại sao Rails lại dùng Ruby mà không phải là một ngữ lập trình nào khác ?

David Heinemeier Hansson, tác giả của Rails, mô tả lại quá trình mà ông ta xây dựng một ứng dụng quản lý dự án trực tuyến có tên là Basecamp vào năm 2004. Ông đã sử dụng ngôn ngữ lập trình PHP nhưng đã thất vọng vì thiếu tính trừu tượng và mã (code) thường xuyên lặp đi lặp lại khiến PHP “không đẹp” (dirty). Hansson muốn sử dụng một công cụ “sạch” giống như trong Java nhưng thấy phát triển bằng Java thì cồng kềnh. Ông đã thử Ruby và vô cùng phấn khích vì tính dễ sử dụng được tìm thấy trong các ngôn ngữ Ruby.
Ưu điểm chính của Ruby là RubyGems (gem giống như một plugin vậy), nó là một trình quản lý các gói (package manager) giúp tạo ra và chia sẻ các gems một cách dễ dàng. RubyGems cung cấp một hệ thống đơn giản để cài đặt cácgems. Bất cứ ai cũng có thể tải một gem lên trang web RubyGems (RubyGems website), từ đó bất cứ ai cũng có thể cài đặt. Trang web RubyGems là nơi chứa các phiên bản mới nhất của Ruby On Rails. Và nó cũng là nơi mà bạn thường truy cập để có được các gems hữu ích cho việc xây dựng trang web phức tạp.

Tại sao Ruby on Rails lại mạnh mẽ cho việc phát triên web đến như vậy ?

Rails có nhiều quy ước phổ biến và sắc sảo. Nếu không dùng bất kỳ framework nào thì lập trình viên cần phải làm một nhiệm vụ khổng lồ để hoàn thành các chức năng trên. Thậm chí ngay cả khi dùng web framework, một lập trình viên có thể có cách tiếp cận mang phong cách riêng, xây dựng ra một cái gì đó mà không ai khác có thể dễ dàng hiểu được. Heinemeier Hansson và đội ngũ cốt lõi tham gia cùng ông đã quyết định rằng có chỉ có một cách tốt nhất để thực hiện cơ sở hạ tầng (infrastructure) cần thiết của một ứng dụng web. Heinemeier Hansson và đội ngũ của ông đã định nghĩa Rails API mà phản ánh kinh nghiệm sâu sắc và thông minh trong việc thực hiện các yêu cầu của một web framework.
Ưu điểm của việc thiết lập các quy ước (convention) ở thời điểm hiện tại có vẻ hiển nhiên (nhiều framework khác đã học tập từ ưu điểm này của Rails), nhưng khi Ruby On Rails được phát hành vào năm 2004 thì tất cả các framework không hề có. Ngày nay, các framework của PHP, Java, và .NET vẫn còn phổ biến, nhưng đã học tập nhiều thứ từ Ruby On Rails. Hiểu được Rails, bạn sẽ dễ dàng hiểu được các framework hiện đại khác của PHP, Python,..
Chính nhờ những ưu việt như ngôn ngữ Ruby dễ học, framework hoàn chỉnh (full-stack), các định nghĩa hàm sâu sắc và thông minh (bằng các convention), Rails đã trở thành framework rất phổ biến cho các dự án start-up. Vì chúng thường cần thay đổi nhiều, Rails dùng ít code hơn các framework khác, web site được xây dựng nhanh chóng nhưng tại tốn ít chi phí bảo trì. Đó là lý do các công ty startup rất thích dùng Rails, và tiền công cho Rails developers thường cao hơn các developer của các framework khác (với cùng số năm kinh nghiệm).

Bài viết có sử dụng tài liệu tham khảo từ các trang web :
- [Wiki-ruby](https://en.wikipedia.org/wiki/Ruby_(programming_language))
- [Ruby-lang.org](https://www.ruby-lang.org/en/about/)
- [Wiki](https://en.wikipedia.org/wiki/Application_programming_interface)
- [Rubygem](https://rubygems.org/)
