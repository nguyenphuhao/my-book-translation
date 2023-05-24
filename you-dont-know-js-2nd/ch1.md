# Chapter 1: What Is JavaScript?

Bạn chưa biết Javascript (JS), và tôi cũng chưa biết hoàn toàn. Chúng ta có thể bắt đầu tìm hiểu JS một cách tốt hơn.

Trong chương đầu tiên của cuốn sách You Don't Know JS Yet (YDKJSY), chúng ta xây dựng nền tảng để tiến xa hơn. Chúng ta sẽ giải thích các chi tiết quan trọng, xóa đi những thắc mắc và hiểu lầm về ngôn ngữ này.

Điều này giúp hiểu rõ về cách tổ chức và duy trì JS, điều mà tất cả lập trình viên JS nên biết. Nếu bạn muốn hiểu JS, đây là bước đầu tiên trong hành trình đó.

## Về cuốn sách này
Tôi nhấn mạnh từ khóa "journey" vì biết về JS không phải là một điểm đến, mà là một hướng. Dù bất kỳ thời gian nào bạn dành cho ngôn ngữ này, bạn luôn có thể tìm hiểu thêm và hiểu sâu hơn một chút. Vì vậy, đừng xem cuốn sách này như một thứ để vội vã hoàn thành một cách nhanh chóng. Thay vào đó, sự kiên nhẫn và kiên trì là tốt nhất khi bạn tiến bộ từng bước nhỏ này.

Sau chương giới thiệu này, phần còn lại của cuốn sách trình bày một bản đồ mức cao về những gì bạn sẽ gặp khi khám phá và nghiên cứu về JS với các cuốn sách YDKJSY.

Đặc biệt, Chapter 4 xác định ba trụ cột chính mà ngôn ngữ JS được tổ chức xung quanh: scope/closures, prototypes/objects và types/coercion. JS là một ngôn ngữ rộng lớn và tinh vi, với nhiều tính năng và khả năng. Nhưng tất cả JS dựa trên ba trụ cột cơ bản này.

Hãy nhớ rằng, mặc dù cuốn sách này mang tiêu đề "Get Started," nó không phải là một cuốn sách dành cho người mới/bắt đầu. Nhiệm vụ chính của cuốn sách này là chuẩn bị bạn để nghiên cứu sâu về JS trong phần còn lại của loạt sách; nó được viết dựa trên giả định rằng bạn đã quen thuộc với JS trong ít nhất vài tháng trước khi tiến vào YDKJSY. Vì vậy, để tận dụng tối đa cuốn "Get Started," hãy đảm bảo bạn dành đủ thời gian viết mã JS để tích lũy kinh nghiệm.

Ngay cả khi bạn đã viết rất nhiều JS trước đây, cuốn sách này không nên chỉ đọc qua hoặc bỏ qua; hãy dành thời gian để hoàn toàn tiếp thu thông tin ở đây. Một khởi đầu tốt luôn phụ thuộc vào bước đầu tiên vững chắc.

## Chuyện gì đã xảy ra với cái tên Javascript

Tên JavaScript có lẽ là tên ngôn ngữ lập trình gây nhầm lẫn và hiểu lầm nhất.

Ngôn ngữ này có liên quan đến Java không? Chỉ là phiên bản script cho Java? Chỉ để viết các kịch bản và không phải là chương trình thực sự?

Thực tế là tên JavaScript là một kết quả của những chiêu trò tiếp thị. Khi Brendan Eich lần đầu tạo ra ngôn ngữ này, ông đặt tên mã Mocha. Trong nội bộ của Netscape, tên thương hiệu LiveScript được sử dụng. Nhưng khi đến lúc đặt tên ngôn ngữ công khai, "JavaScript" đã giành chiến thắng trong cuộc bỏ phiếu.

Tại sao? Bởi vì ngôn ngữ này ban đầu được thiết kế để hấp dẫn đối tượng là những lập trình viên Java, và vì từ "script" phổ biến để chỉ các chương trình nhẹ nhàng. Những "script" nhẹ nhàng này sẽ là những chương trình đầu tiên nhúng vào trong trang web, điều gọi là web mới!

Nói cách khác, JavaScript là một chiến lược tiếp thị nhằm thể hiện ngôn ngữ này là một lựa chọn dễ chịu thay thế cho việc viết Java nặng hơn và nổi tiếng hơn vào thời điểm đó. Nó có thể dễ dàng được gọi là "WebJava".

Có một số sự tương đồng bề ngoài giữa mã của JavaScript và mã Java. Những sự tương đồng đó không đến từ việc phát triển chung, mà đến từ cả hai ngôn ngữ đều nhắm đến các nhà phát triển với kỳ vọng cú pháp từ C (và một phần đến từ C++).

Ví dụ, chúng ta sử dụng dấu { để bắt đầu một khối mã và dấu } để kết thúc khối mã đó, giống như C/C++ và Java. Chúng ta cũng sử dụng dấu ; để kết thúc một câu lệnh.

Một số mặt, mối quan hệ pháp lý còn sâu sắc hơn cú pháp. Oracle (qua Sun), công ty hiện vẫn sở hữu và vận hành Java, cũng sở hữu thương hiệu chính thức cho tên "JavaScript" (qua Netscape). Thương hiệu này hiếm khi được thực thi, và có thể không thể thực thi được vào thời điểm này.

Vì những lý do này, một số người đã đề xuất sử dụng JS thay vì JavaScript. Đó là một cách viết tắt rất phổ biến, mặc dù không phải là một ứng viên lý tưởng cho việc đặt tên chính thức cho ngôn ngữ. Thực tế, những cuốn sách này sử dụng JS gần như độc quyền để chỉ đến ngôn ngữ này.

Để tách biệt ngôn ngữ khỏi thương hiệu được sở hữu bởi Oracle, tên chính thức của ngôn ngữ được chỉ định bởi TC39 và được hình thành bởi tổ chức tiêu chuẩn ECMA là ECMAScript. Và từ năm 2016, tên chính thức của ngôn ngữ cũng được thêm hậu tố là năm sửa đổi; vào thời điểm viết bài này, đó là ECMAScript 2019, hoặc viết tắt khác là ES2019.

Nói cách khác, JavaScript/JS chạy trên trình duyệt của bạn hoặc trên Node.js, là một phiên bản thực thi của tiêu chuẩn ES2019.

LƯU Ý: Đừng sử dụng các thuật ngữ như "JS6" hoặc "ES8" để chỉ đến ngôn ngữ. Một số người có thể dùng nhưng những thuật ngữ đó chỉ gây lẫn lộn. "ES20xx" hoặc chỉ "JS" là những thuật ngữ bạn nên sử dụng. Cho dù bạn gọi nó là JavaScript, JS, ECMAScript hay ES2019, chắc chắn đó không phải là một biến thể của ngôn ngữ Java!

## Language Specification

Tôi đã đề cập đến TC39, ủy ban chỉ đạo kỹ thuật quản lý JS. Nhiệm vụ chính của họ là quản lý quy định chính thức cho ngôn ngữ. Họ họp thường xuyên để bỏ phiếu về bất kỳ thay đổi đã được thống nhất nào, sau đó gửi đến ECMA, tổ chức tiêu chuẩn.

Cú pháp và hành vi của JS được định nghĩa trong quy định ES.

ES2019 ngẫu nhiên là phiên bản đánh số lớn thứ 10 kể từ khi JS ra đời vào năm 1995, vì vậy trong URL chính thức của quy định được lưu trữ bởi ECMA, bạn sẽ thấy "10.0":

https://www.ecma-international.org/ecma-262/10.0/

Uỷ ban TC39 bao gồm từ 50 đến khoảng 100 người khác nhau đến từ các công ty đầu tư rộng rãi trong lĩnh vực web, chẳng hạn như nhà sản xuất trình duyệt (Mozilla, Google, Apple) và nhà sản xuất thiết bị (Samsung, v.v.). Tất cả các thành viên của ủy ban đều là tình nguyện viên, mặc dù nhiều người trong số họ là nhân viên của các công ty này và có thể nhận được bù trừ một phần cho nhiệm vụ của họ trong ủy ban.

TC39 họp gần như hai tháng một lần, thông thường trong khoảng ba ngày, để xem xét công việc đã được các thành viên thực hiện kể từ cuộc họp trước đó, thảo luận vấn đề và bỏ phiếu về các đề xuất. Địa điểm họp thay đổi giữa các công ty thành viên sẵn lòng đăng cai.

Tất cả các đề xuất của TC39 tiến bộ qua một quy trình gồm năm giai đoạn - tất nhiên, vì chúng ta là những lập trình viên, nó bắt đầu từ 0! - Giai đoạn 0 đến giai đoạn 4. Bạn có thể đọc thêm về quy trình giai đoạn tại đây: https://tc39.es/process-document/

Giai đoạn 0 có nghĩa là, đại khái, một thành viên TC39 nghĩ rằng đó là một ý tưởng đáng xem và kế hoạch bảo vệ và làm việc trên nó. Điều đó có nghĩa là nhiều ý tưởng mà những người không phải là thành viên TC39 "đề xuất", thông qua các phương tiện không chính thức như mạng xã hội hoặc bài đăng trên blog, thực sự chỉ là "trước giai đoạn 0". Bạn phải có một thành viên TC39 bảo vệ đề xuất để nó được xem xét "Giai đoạn 0" chính thức.

Khi một đề xuất đạt đến trạng thái "Giai đoạn 4", nó có thể được bao gồm trong phiên bản sửa đổi hàng năm tiếp theo của ngôn ngữ. Thời gian để một đề xuất hoàn thành các giai đoạn này có thể kéo dài từ vài tháng đến vài năm.

Tất cả các đề xuất được quản lý công khai, trên kho lưu trữ Github của TC39: https://github.com/tc39/proposals

Bất kỳ ai, có là thành viên TC39 hay không, đều được hoan nghênh tham gia vào các cuộc thảo luận công khai và quy trình làm việc với các đề xuất. Tuy nhiên, chỉ thành viên TC39 mới có thể tham dự các cuộc họp và bỏ phiếu về các đề xuất và thay đổi. Vì vậy, thực tế là giọng nói của một thành viên TC39 mang rất nhiều trọng lượng về hướng đi của JS.

Không giống như một số lời đồn cũ và đáng thất vọng, không có nhiều phiên bản của JavaScript. Chỉ có một JS, tiêu chuẩn chính thức được quản lý bởi TC39 và ECMA.

Trong thập kỷ đầu 2000, khi Microsoft duy trì một phiên bản "JScript" được sao chép và đảo ngược (và không hoàn toàn tương thích) của JS, thì thực sự đã có "nhiều phiên bản" JS. Nhưng những ngày đó đã qua rồi. Việc tuyên bố như vậy về JS ngày nay đã cũ và không chính xác.

Tất cả các trình duyệt chính và nhà sản xuất thiết bị đã cam kết duy trì việc triển khai JS của họ tuân thủ với tiêu chuẩn trung tâm này. Tất nhiên, các engine triển khai tính năng vào thời điểm khác nhau. Nhưng không bao giờ có trường hợp mà engine v8 (engine JS của Chrome) triển khai một tính năng được chỉ định khác biệt hoặc không tương thích so với engine SpiderMonkey (engine JS của Mozilla).

Điều đó có nghĩa là bạn có thể học một JS và tin cậy vào cùng một JS đó ở mọi nơi.

Web Chi phối mọi thứ về (JS) Trong khi danh sách môi trường chạy JS ngày càng mở rộng (từ trình duyệt, đến máy chủ (Node.js), đến robot, đèn LED, v.v.), môi trường duy nhất chi phối JS là web. Nói cách khác, cách JS được triển khai cho trình duyệt web, về mặt thực tế, là thực tế duy nhất quan trọng.

Phần lớn cú pháp và hành vi JS được định nghĩa trong quy định ES.

ES2019 tình cờ là phiên bản/sửa đổi đánh số chính thứ 10 kể từ khi JS ra đời năm 1995, vì vậy trong URL chính thức của quy định được lưu trữ bởi ECMA, bạn sẽ tìm thấy "10.0":

https://www.ecma-international.org/ecma-262/10.0/

Hội đồng TC39 bao gồm từ 50 đến khoảng 100 người khác nhau đến từ các công ty liên quan đa dạng như các nhà làm trình duyệt (Mozilla, Google, Apple) và các nhà sản xuất thiết bị (Samsung, v.v). Tất cả các thành viên của hội đồng đều là tình nguyện viên, tuy nhiên nhiều người trong số họ là nhân viên của những công ty này và có thể nhận được tiền bồi dưỡng một phần cho nhiệm vụ của họ trong hội đồng.

TC39 họp tổng cộng khoảng mỗi hai tháng một lần, thường trong khoảng ba ngày, để xem xét công việc đã được các thành viên thực hiện kể từ cuộc họp trước đó, thảo luận về các vấn đề và bỏ phiếu về các đề xuất. Địa điểm họp hẹn xoay vòng giữa các công ty thành viên sẵn lòng đăng cai.

Tất cả các đề xuất của TC39 đi qua một quy trình gồm năm giai đoạn - tất nhiên, vì chúng ta là những lập trình viên, nên nó dựa trên số 0! - Giai đoạn 0 đến Giai đoạn 4. Bạn có thể đọc thêm về quy trình Giai đoạn tại đây: https://tc39.es/process-document/

Giai đoạn 0 đại diện đại khái cho việc một thành viên TC39 cho rằng đó là một ý tưởng đáng xem và đề xuất kế hoạch để nghiên cứu và làm việc với nó. Điều này có nghĩa rằng nhiều ý tưởng mà các người không phải là thành viên TC39 "đề xuất" thông qua các phương tiện không chính thức như mạng xã hội hoặc bài viết trên blog thực sự chỉ là "trước Giai đoạn 0" chính thức. Bạn phải có một thành viên TC39 bảo vệ đề xuất để nó được coi là "Giai đoạn 0".

Khi một đề xuất đạt Giai đoạn 4, nó có thể được bao gồm trong phiên bản sửa đổi hàng năm tiếp theo của ngôn ngữ. Thời gian mà một đề xuất hoàn thành các giai đoạn này có thể kéo dài từ vài tháng đến vài năm.

Tất cả các đề xuất được quản lý công khai, trên kho lưu trữ GitHub của TC39: https://github.com/tc39/proposals

Bất kỳ ai, có hoặc không phải là thành viên TC39, đều được khuyến khích tham gia vào các cuộc thảo luận công khai và quy trình làm việc với các đề xuất. Tuy nhiên, chỉ có các thành viên TC39 mới có thể tham dự các cuộc họp và bỏ phiếu về các đề xuất và thay đổi. Vì vậy, thực tế là giọng nói của một thành viên TC39 mang nhiều trọng số về hướng phát triển của JS.

Đừng lo lắng, không có nhiều phiên bản của JavaScript như một số tin đồn cũ và đáng thất vọng. Chỉ có một JavaScript, tiêu chuẩn chính thức được quản lý bởi TC39 và ECMA.

Trong thập kỷ đầu 2000, khi Microsoft duy trì một phiên bản "JScript" được sao chép và đảo ngược (và không hoàn toàn tương thích) của JavaScript, thì thực tế đã có "nhiều phiên bản" JavaScript. Nhưng những ngày đó đã qua rồi. Việc tuyên bố như vậy về JavaScript ngày nay đã cũ và không chính xác.

Tất cả các trình duyệt chính và các nhà sản xuất thiết bị đã cam kết duy trì triển khai JavaScript của họ tuân theo tiêu chuẩn trung tâm này. Tất nhiên, các engine triển khai tính năng vào thời điểm khác nhau, nhưng không bao giờ có trường hợp mà engine V8 (engine JavaScript của Chrome) triển khai một tính năng được chỉ định khác biệt hoặc không tương thích so với engine SpiderMonkey (engine JavaScript của Mozilla).

Điều đó có nghĩa là bạn có thể học một JavaScript và tin tưởng vào JavaScript đó ở bất kỳ đâu.

### Mọi thứ về Quy tắc trên Web (JS)

Trong khi danh sách các môi trường chạy JS ngày càng mở rộng (từ trình duyệt, máy chủ (Node.js), robot, bóng đèn, vv...), môi trường duy nhất quản lý JS là web. Nói cách khác, cách JS được triển khai cho trình duyệt web, thực tế, là thực tế duy nhất quan trọng.

Phần lớn JS được xác định trong quy định và JS chạy trong các trình duyệt dựa trên engine JS là giống nhau. Tuy nhiên, có một số khác biệt phải được xem xét.

Đôi khi quy định JS sẽ chỉ định một số hành vi mới hoặc được cải tiến, nhưng nó không khớp hoàn toàn với cách nó hoạt động trong các engine JS dựa trên trình duyệt. Sự không khớp này là lịch sử: các engine JS đã có hơn 20 năm kinh nghiệm về các trường hợp đặc biệt của tính năng mà các nội dung web đã dựa vào. Vì vậy, đôi khi các engine JS sẽ từ chối tuân thủ một thay đổi được quy định trong quy định vì nó sẽ làm hỏng nội dung web đó.

Trong những trường hợp này, thường TC39 sẽ rút lại và chỉ đơn giản chọn tuân thủ quy định theo thực tế trên web. Ví dụ, TC39 đã lên kế hoạch thêm một phương thức contains(..) cho Arrays, nhưng đã phát hiện rằng tên này xung đột với các framework JS cũ vẫn đang được sử dụng trên một số trang web, vì vậy họ đã thay đổi tên thành includes(..) không gây xung đột. Điều tương tự xảy ra với một cuộc khủng hoảng hài hước/đau buồn trong cộng đồng JS được đặt tên là "smooshgate", nơi phương thức dự định flatten(..) cuối cùng được đổi tên thành flat(..).

Nhưng đôi khi, TC39 sẽ quyết định quy định nên tuân thủ một số điểm dù khó có thể các engine JS dựa trên trình duyệt sẽ tuân thủ.

Giải pháp là ghi chú B, "Các tính năng ECMAScript bổ sung cho Trình duyệt Web". Quy định JS bao gồm phụ lục này để chỉ ra bất kỳ sự không khớp đã biết nào giữa quy định JS chính thức và thực tế JS trên web. Nói cách khác, đây là các ngoại lệ chỉ áp dụng cho JS web; các môi trường JS khác phải tuân theo nguyên tắc của quy định.

Phần B.1 và B.2 bao gồm thêm vào JS (cú pháp và API) mà JS web bao gồm, một lần nữa vì lý do lịch sử, nhưng mà TC39 không lên kế hoạch chỉ định chính thức trong lõi JS. Ví dụ bao gồm octal literals với tiền tố 0, các tiện ích escape(..) / unescape(..) toàn cục, các "trợ giúp" String như anchor(..) và blink(), và phương thức compile(..) của RegExp.

Phần B.3 bao gồm một số xung đột trong đó mã có thể chạy trên cả trình duyệt web và các engine JS không web, nhưng hành vi có thể khác nhau một cách có thể quan sát được, dẫn đến kết quả khác nhau. Đa số các thay đổi được liệt kê liên quan đến các tình huống được gắn nhãn là lỗi sớm khi mã đang chạy ở chế độ nghiêm ngặt.

Những điểm cần lưu ý trong phụ lục B không gặp quá nhiều, nhưng nó vẫn là ý tưởng tốt để tránh những cấu trúc này để đảm bảo sự an toàn trong tương lai. Bất cứ khi nào có thể, tuân theo quy định JS và không phụ thuộc vào hành vi chỉ áp dụng trong một số môi trường JS cụ thể.

### Không phải tất cả (Web) JS…

Đoạn mã này là một chương trình JS không?
```
alert("Hello, JS!");
```
Tùy thuộc vào cách bạn nhìn vào vấn đề. Hàm alert(..) được hiển thị ở đây không được bao gồm trong quy định JS, nhưng nó được sử dụng trong tất cả các môi trường JS web. Tuy nhiên, bạn sẽ không tìm thấy nó trong Phụ lục B, vậy điều gì đã xảy ra?

Các môi trường JS khác nhau (như trình duyệt, Node.js, vv.) thêm các API vào phạm vi toàn cục của chương trình JS của bạn để cung cấp các khả năng cụ thể cho môi trường đó, chẳng hạn như hiển thị hộp thoại cảnh báo trên trình duyệt người dùng.

Thực tế, có một loạt các API trông giống JS như fetch(..), getCurrentLocation(..), và getUserMedia(..), đều là các API web trông giống JS. Trong Node.js, chúng ta có thể truy cập hàng trăm phương thức API từ các module tích hợp khác nhau, chẳng hạn như fs.write(..).

Một ví dụ phổ biến khác là console.log(..) (và tất cả các phương thức console.* khác!). Chúng không được quy định trong JS, nhưng vì tính hữu dụng chung của chúng, chúng được định nghĩa bởi hầu hết các môi trường JS, theo một sự thỏa thuận đồng ý đầy đủ.

Vì vậy, alert(..) và console.log(..) không được định nghĩa bởi JS. Nhưng chúng trông giống JS. Chúng là các hàm và các phương thức của đối tượng và chúng tuân theo các quy tắc cú pháp JS. Hành vi bên trong chúng được điều khiển bởi môi trường chạy engine JS, nhưng ở mặt bề ngoài, chúng chắc chắn phải tuân thủ JS để có thể hoạt động trong môi trường JS.

Hầu hết sự khác biệt trên các trình duyệt mà mọi người than phiền với các tuyên bố “JS không nhất quán!” thực tế là do sự khác biệt trong cách các hành vi môi trường đó hoạt động, không phải cách JS hoạt động.

Vì vậy, một cuộc gọi alert(..) là JS, nhưng alert chính nó thực sự chỉ là một khách mời, không phải một phần của quy định JS chính thức.

Đó không phải lúc nào cũng là JS
Sử dụng bảng điều khiển/REPL (Read-Evaluate-Print-Loop) trong Công cụ Phát triển trình duyệt của bạn (hoặc Node) ban đầu có vẻ như môi trường JS rõ ràng. Nhưng thực tế không phải vậy.

Công cụ Phát triển là… công cụ cho nhà phát triển. Mục đích chính của chúng là làm cho cuộc sống của nhà phát triển dễ dàng hơn. Chúng ưu tiên DX (Developer Experience). Mục tiêu của các công cụ như vậy là giúp bạn kiểm tra, thử nghiệm và gỡ lỗi mã JS của bạn một cách nhanh chóng và hiệu quả.

Vì vậy, các công cụ phát triển đã tích hợp sẵn các tiện ích và API khác nhau, nhưng chúng không phải là một phần của quy định JS chính thức. Chẳng hạn, công cụ phát triển có thể cung cấp các phương thức hữu ích như $_(..) để tham chiếu đến kết quả trước đó từ REPL, nhưng đó không phải là JS tiêu chuẩn. Nó chỉ là một tiện ích hỗ trợ được cung cấp bởi công cụ phát triển để bạn làm việc hiệu quả hơn.

Vì vậy, hãy nhớ rằng mỗi môi trường JS có thể cung cấp các tiện ích và API riêng, và không phải tất cả đều là JS chính thức. Hãy luôn kiểm tra tài liệu cụ thể của môi trường mà bạn đang sử dụng để biết các tính năng và hành vi đặc biệt của nó.

## Có nhiều khía cạnh

Thuật ngữ “paradigm (mô hình)” trong ngữ cảnh ngôn ngữ lập trình liên quan đến một tư duy và phương pháp tổ chức mã nguồn rộng (gần như phổ quát). Trong một mô hình, có vô số các biến thể về phong cách và hình thức phân biệt các chương trình, bao gồm vô số các thư viện và frameworks khác nhau tạo nên dấu ấn riêng của chúng trên bất kỳ mã nguồn cụ thể nào.

Nhưng dù cho phong cách riêng của một chương trình có thể là gì, các phân chia tổng thể về mô hình hầu như luôn rõ ràng ngay từ cái nhìn đầu tiên vào bất kỳ chương trình nào.

Các loại mã theo mô hình thông thường bao gồm mô hình thủ tục, hướng đối tượng (OO/classes) và hàm (FP):

Phong cách thủ tục tổ chức mã nguồn theo một tiến trình từ trên xuống dưới, tiến hành qua một tập hợp các hoạt động đã được xác định trước, thường được tổ chức lại thành các đơn vị có liên quan được gọi là các thủ tục.

Phong cách hướng đối tượng tổ chức mã nguồn bằng cách tập trung logic và dữ liệu vào các đơn vị được gọi là lớp.

Phong cách hàm tổ chức mã nguồn thành các hàm (tính toán thuần túy so với các thủ tục), và các biến thể của các hàm đó là các giá trị.

Các mô hình không phải đúng hay sai. Chúng là hướng dẫn và tạo hình cách các lập trình viên tiếp cận vấn đề và giải pháp, cách họ tổ chức và duy trì mã nguồn của mình.

Một số ngôn ngữ hướng mạnh vào một mô hình cụ thể – ví dụ, C là mô hình thủ tục, Java/C++ hầu như hoàn toàn hướng đối tượng, và Haskell chẳng hạn là hàm trong và ngoài.

Nhưng nhiều ngôn ngữ cũng hỗ trợ các mẫu mã nguồn có thể xuất phát từ và kết hợp từ các mô hình khác nhau. Các “ngôn ngữ đa mô hình” được gọi như vậy mang lại tính linh hoạt tối đa. Trong một số trường hợp, một chương trình duy nhất có thể có hai hoặc nhiều biểu thức của các mô hình này cùng tồn tại bên nhau.

JavaScript chắc chắn là một ngôn ngữ đa mô hình. Bạn có thể viết mã theo phong cách thủ tục, hướng đối tượng hoặc hàm, và bạn có thể đưa ra những quyết định đó dựa trên từng dòng mã thay vì bị buộc phải chọn giữa một lựa chọn tất cả hoặc không có gì.
