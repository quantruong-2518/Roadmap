<strong>#Roadmap-basicjs</strong> <strong>#DOM</strong> <strong>#DOM-manipulations</strong> </br>
by: <strong>Steve Truong</strong> - at: Feb-26th

<h2>1. DOM là gì?</h2> <br />
DOM (Document Object Model – tạm dịch Mô hình Các Đối tượng Tài liệu). Là một chuẩn được định nghĩa bởi W3C (Tổ Chức Web Toàn Cầu – World Wide Web Consortium). DOM được dùng để truy xuất và thao tác trên các tài liệu có cấu trúc dạng HTML hay XML.

<img src="https://topdev.vn/blog/wp-content/uploads/2021/01/dom-la-gi.gif" alt="nodes" />

Các loại Nodes: 
- Node gốc (Root): chính là tài liệu HTML, thường được biểu diễn bởi thẻ <html>.
- Node phần tử (Element): biểu diễn cho 1 phần tử HTML.
- Node văn bản (Text): mỗi đoạn kí tự trong tài liệu HTML, bên trong 1 thẻ HTML đều là 1 node văn bản
- Node thuộc tính (Atrribute)

Quan hệ giữa các Nodes: 
- Node gốc (document) luôn là node đầu tiên.
- Tất cả các node không phải là node gốc đều chỉ có 1 node cha (parent).
- Một node có thể có một hoặc nhiều con, nhưng cũng có thể không có con nào.
- Những node có cùng node cha được gọi là các node anh em (siblings).
- Trong các node anh em, node đầu tiên được gọi là con cả (firstChild) và node cuối cùng là con út (lastChild).
  
<h2>2. DOM Manipulations</h2> <br />
  
 Thuộc tính:
  - id: Định danh – là duy nhất cho mỗi phần tử nên thường được dùng để truy xuất DOM trực tiếp và nhanh chóng.
  - className: Tên lớp – Cũng dùng để truy xuất trực tiếp như id, nhưng 1 className có thể dùng cho nhiều phần tử.
  - tagName: Tên thẻ HTML.
  - innerHTML: Trả về mã HTML bên trong phần tử hiện tại. Đoạn mã HTML này là chuỗi kí tự chứa tất cả phần tử bên trong, bao gồm các node phần tử và node văn bản.
  - outerHTML: Trả về mã HTML của phần tử hiện tại. Nói cách khác, outerHTML = tagName + innerHTML.
  - textContent: Trả về 1 chuỗi kí tự chứa nội dung của tất cả node văn bản bên trong phần tử hiện tại.
  - attributes: Tập các thuộc tính như id, name, class, href, title…
  - style: Tập các định dạng của phần tử hiện tại
  - value: Lấy giá trị của thành phần được chọn thành một biến.

 Phương thức:
  - getElementById(id): Tham chiếu đến 1 node duy nhất có thuộc tính id giống với id cần tìm.
  - getElementsByTagName(tagname): Tham chiếu đến tất cả các node có thuộc tính tagName giống với tên thẻ cần tìm, hay hiểu đơn giản hơn là tìm tất cả các phần tử   - DOM mang thẻ HTML cùng loại. Nếu muốn truy xuất đến toàn bộ thẻ trong tài liệu HTML thì hãy sử dụng document.getElementsByTagName('*').
  - getElementsByName(name): Tham chiếu đến tất cả các node có thuộc tính name cần tìm.
  - getAttribute(attributeName): Lấy giá trị của thuộc tính.
  - setAttribute(attributeName, value): Sửa giá trị của thuộc tính.
  - appendChild(node): Thêm 1 node con vào node hiện tại.
  - removeChild(node): Xóa 1 node con khỏi node hiện tại.
  
 Thuộc tính quan hệ:
  - parentNode: node cha
  - childNodes: Các node con
  - firstChild: node con đầu tiên
  - lastChild: node con cuối cùng
  - nextSibling: node anh em liền kề sau
  - previousSibling: node anh em liền kề trước

  
<h2>3. Attachment</h2> <br />
doc: https://topdev.vn/blog/dom-la-gi/

