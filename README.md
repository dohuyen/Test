
#**I.Học cách sử dụng Github**
* Bước 1 : Đăng ký một tài khoản tại Github và đăng nhập.
* Bước 2 : Học cách sử dụng ngôn ngữ `Markdown`
* Bươc 3 : Tạo một repo đầu tiên và gõ bài bằng `Markdown`

#**II.Mô hình OSI và TCP/IP**
##**A.Mô hình OSI**
**Mô hình OSI** (*Open Systems Interconnection*) được tổ chức ISO tạo ra năm 1984. Đó là **mô hình hệ thống mở, là mô hình giúp hai hệ thống khác nhau có thể thông tin với nhau bất kể kiến trúc mạng của chúng ra sao.** Mô hình này bao gồm 7 tầng .Mỗi tầng đều có đặc tính là nó *chỉ sử dụng chức năng của tầng dưới nó* , đồng thời chỉ cho phép tầng trên sử dụng các chức năng của mình.
##**1.Ưu điểm của mô hình OSI :**
* Giảm độ phức tạp của truyền dữ liệu.
* Chuẩn hoa giao diện giữa các tầng .
* Chuyên môn hóa các công nghệ.
* Tạo ra sự tương thích giữa các nhà sản xuất khác nhau.
* Dễ dàng trong việc dạy và học.

![Mô Hình OSI](http://1.bp.blogspot.com/-dEPOLAvxsek/UzQcvDS44KI/AAAAAAAAACw/c_Fxrkuul7k/s1600/Osi-model-jb.png)

##**2.Tổ chức của các tầng :**
Bảy tầng có thể được xem như là thuộc ba nhóm con sau: Tầng 1, 2, 3 - tầng vật lý, kết nối dữ liệu và mạng: là nhóm con các tầng **hỗ trợ mạng, nhằm giải quyết các yếu tố vật lý và truyền dữ liệu từ một thiết bị này sang một thiết bị khác** (như các đặc tính điện học, kết nối vật lý, định địa chỉ vật lý và thời gian truyền cũng như độ tin cậy). Tầng 5, 6, và 7: tầng kiểm soát kết nối, biểu diễn và ứng dựng có thể được xem là nhóm con các tầng **hỗ trợ user** ; chúng cho phép khả năng truy cập đến nhiều hệ thống phần mềm. Tầng  4: tầng vận chuyển, bảo đảm tính tin cậy cho việc truyền dẫn end to end (hai đầu mút) trong khi đó tầng 2 đảm bảo tính tin cậy trên một đường truyền đơn.
##**3.Các tầng trong mô hình OSI :**
###**3.1: TẦNG VẬT LÝ (*PHYSICAL LAYER*)**
Còn gọi là tầng thiết bị, có liên quan tới việc truyền và nhận dòng bit thô chưa có cấu trúc trên một phương tiện vật lý. Tầng này mô tả các giao diện điện/quang học, cơ học và chức năng cho phương tiện vật lý, và mang tín hiệu cho tất cả các tầng cao hơn.
   *Các đặc tính liên quan như sau :*
- Đặc tính vật lý của giao diện và môi trường: 
- Biểu diễn các bit.
- Tốc độ dữ liệu.
- Đồng bộ  bit.
- Cấu hình đường dây.
- Tôpô mạng.
- Chế độ truyền.
 
###**3.2: TẦNG KẾT NỐI DỮ LIỆU (*DATALINK LAYER*)**
Tầng kết nối dữ liệu truyền các dữ liệu thô từ lớp vật lý thành dữ liệu có độ tin cây cao hơn và có thể truyền khung (frame) từ nút đến nút; hỗ trợ cơ chế phát hiện và xử lý lỗi dữ liệu. 
   *Các đặc tính liên quan như sau :*
- Tạo khung (framing). 
-	Định (tạo) địa chỉ vật lý.
-	Điều khiển lưu lượng.
-	Kiểm tra lỗi.
-	Điều khiển truy cập.

###**3.3: TẦNG MẠNG (*NETWORK LAYER*):**
Tầng mạng tìm đường đi cho hai dữ liệu truyền thông giữa hai máy bất kỳ. 
   *Các đặc tính liên quan như sau :*
-	Định (tạo) địa chỉ logic.
-	Định tuyến (routing).

###**3.4: TẦNG VẬN CHUYỂN (*TRANSPORT LAYER*)**
Tầng vận chuyển nhằm chuyển toàn bản tin từ thiết bị đầu cuối phát đến thiết bị đầu cuối thu (end to end). Tầng này có nhiệm vụ phân nhỏ có gói tin có kích thước lớn khi gửi và tập hợp lại khi nhận, đảm bảo tính toàn vẹn cho dữ liệu( không lỗi, không mất, không lặp, đúng thứ tự). 
   *Các nhiệm vụ của tầng vận chuyển :*
-    Định địa chỉ điểm dịch vụ (service-point addressing).
-    Phân đoạn và hợp đoạn.
-	Điều khiển kết nối. 
-	Điều khiển lưu lượng.
-	Kiểm tra lỗi.

###**3.5: TẦNG PHIÊN (*SESSION LAYER*)**
Quản lý phiên làm việc giữa các người sử dụng. Tầng này cung cấp cơ chế nhận biết tên và chức năng về bảo mật thông tin khi truyền qua mạng máy tính. Còn thiết lập, duy trì, giải phóng và đồng bộ hóa tương tác giữa các hệ thống thông tin.
   *Các nhiệm vụ của tầng kiểm soát:*
-	Điều khiển đối thoại.
-	Đồng bộ hoá.

###**3.6: TẦNG TRÌNH BÀY (*PRESENTATION LAYER*)**
Tầng trình bày liên quan đến vấn đề về cú pháp (syntax) và ngữ nghĩa (sematic) của tin tức trao đổi giữa hai hệ thống. Tầng này cung cấp định dạng dữ liệu cho ứng dụng, đảm bảo các máy tính có định dạng dữ liệu khác nhau vẫn có thể truyền thông tin cho nhau bình thường.
   *Các nhiệm vụ của tầng trình bày :*
-	Biên dịch (translation).
-    Mã khóa (encryption) và Giải mã khóa (decryption). 
-	Nén.

###**3.7: TẦNG ỨNG DỤNG (*APPLICATION LAYER*)**
Cho phép người dùng (user) là người hay phần mềm, truy cập vào mạng. Tầng này cung cấp giao diện cho người dùng và hỗ trợ dịch vụ như thư điện tử, remote file access and transfer, shared database management và các dạng dịch vụ phân phối dữ liệu khác.
   *Các đặc tính của tầng ứng dụng :*
-	Mạng đầu cuối ảo (network virtual terminal).
-	Quản lý, truy cập và truyền dữ liệu (FTAM: file transfer, access, and management).
-    Dịch vụ thư mục (directory services).

##**B.Mô hình TCP/IP**
**TCP/IP** là một **hệ thống giao thức - một tập hợp các giao thức hỗ trợ việc lưu truyền trên mạng.** Bất cứ máy nào dùng bộ giao thức TCP/IP đều có thể kết nối được vào Internet. Hai giao thức được dùng chủ yếu ở đây là **TCP** (*Transmission Control Protocol*) và **IP** (*Internet Protocol*). 
###1. Các tầng của mô hình TCP/IP
Để cho các máy tính trao đổi dữ liệu với nhau TCP/IP sử dụng mô hình truyền thông 4 tầng hay còn gọi là Mô Hình DoD (Mô hình của Bộ Quốc Phòng Mỹ).Các tầng trong mô hình này là (Theo thứ tự từ dưới lên):
-    Tầng Giao Diện Mạng (Network Access Layer).
-    Tầng Liên Mạng (Internet Layer).
-    Tầng Vận Chuyển (Transport Layer).
-    Tầng Ứng Dụng (Application Layer).

![Mô Hình TCP/IP](http://lh4.googleusercontent.com/-jH4TzAOcspU/UzQeMUZ1JlI/AAAAAAAAADA/cWNGZjCtkI4/s1600/TCP-IP-Model.png)

###**1.1: TẦNG GIAO DIỆN MẠNG (*NETWORK ACCESS LAYER*)**
**Tầng Giao Diện Mạng** có trách nhiệm đưa dữ liệu tới và nhận dữ liệu từ phương tiện truyền dẫn. Tầng này gồm các thiết bị phần cứng vật lí (Hun, Swtich, cáp mạng, card mạng HBA- Host Bus Adapter và các đặc tả mức thấp như tín hiệu điện). Một số giao thức tiêu biểu thuộc tầng này gồm :
-     ATM (Asynchronous Transfer Mode).
-     Ethernet.
-     Token Ring.
-     FDDI (Fiber Distributed Data Interface).
-     Frame Relay.

###**1.2: TẦNG VẬN CHUYỂN (*TRANSPORT LAYER*)**
Có trách nhiệm thiết lập phiên truyền thông giữa các máy tính và quy định cách truyền dữ liệu. 2 giao thức chính trong tầng này       gồm:
-    UDP (User Datagram Protocol): Còn gọi là Giao Thức Gói Người Dùng. UDP cung cấp các kênh truyền thông phi kết nối nên nó không  đảm bảo truyền dữ liệu 1 cách tin cậy. Các ứng dụng dùng UDP thường chỉ truyền những gói có kích thước nhỏ, độ tin cậy dữ liệu        phụ thuộc vào từng ứng dụng.
-    TCP (Transmission Control Protocol): Ngược lại với UDP, TCP cung cấp các kênh truyền thông hướng kết nối và đảm bảo truyền dữ liệu 1 cách tin cậy. TCP thường truyền các gói tin có kích thước lớn và yêu cầu phía nhận xác nhận về các gói tin đã nhận.

###**1.3: TẦNG MẠNG (*INTERNET LAYER*)**
Mục đích của tầng Internet là chọn đường đi tốt nhất xuyên qua mạng cho các gói dữ liệu di chuyển tới đích.
Giao thức chính của tầng này là Internet Protocol (IP) có các chức năng :
-	Định nghĩa cấu trúc các gói dữ liệu là đơn vị cơ sở cho việc truyền dữ liệu trên Internet.
-	Định nghĩa phương thức đánh địa chỉ IP.
-	Truyền dữ liệu giữa tầng vận chuyển và tầng mạng.
-	Định tuyến để truyền các gói dữ liệu trong mạng.
-	Thực hiện việc phân mảnh và hợp nhất các gói dữ liệu và nhúng/tách chúng trong các gói dữ liệu ở tầng liên kết.
     Ngoài ra còn có một số giao thức khác như : 
-    ARP (Address Resolution Protocol): biên dịch địa chỉ IP của máy đích thành địa chỉ MAC.
-    ICMP (Internet Control Message Protocol): thông báo lỗi trong trường hợp truyền dữ liệu bị hỏng.
-    IGMP (Internet Group Management Protocol): điều khiển truyền đa hướng (Multicast).
- 	 RARP (Reverse Address Resolution Protocol): trả về địa chỉ IP tương ứng cho máy trạm đã gởi yêu cầu.

###**1.4: TẦNG ỨNG DỤNG (*APPLICATION LAYER*)**
Gồm nhiều giao thức cung cấp cho các ứng dụng người dùng. Được sử dụng để định dạng và trao đổi thông tin người dùnng. Một số giao thức chính thông dụng :
-	FTP (File Transfer Protocol): là dịch vụ có tạo cầu nối, sử dụng TCP để truyền các tập tin giữa các hệ thống.
-	TFTP (Trivial File Transfer Protocol): là dịch vụ không tạo cầu nối, sử dụng UDP. Được dùng trên router để truyền các file cấu  hình và hệ điều hành.
-	NFS (Network File System): cho phép truy xuất file đến các thiết bị lưu trữ ở xa như một đĩa cứng qua mạng.
-	SMTP (Simple Mail Transfer Protocol): quản lý hoạt động truyền e-mail qua mạng máy tính.
-	SNMP ( Simple Network Management Protocol) : Giao thức được dùng để theo dõi thiết bị phần cứng gắn trên những mạng TCP/IP mà    thực hiện giao thức này . SNMP là giao thức lớp Application dùng UDP trong cổng 161 và 162 .
-	DNS (Domain Name System): thông dịch tên của các miền (Domain) và các node mạng được công khai sang các địa chỉ IP.

#**III.Một số giao thức tầng ứng dụng trong mô hình TCP/IP**
- **FTP(*File Transfer Protocol*)** : Đây là một dịch vụ hướng kết nối và tin cậy, sử dụng giao thức TCP để cung cấp tuyển các tập tin giữa các hệ thống hỗ trợ FTP.
- **Telnet(*Terminal Network*)** : Cho phép các phiên đăng nhập từ xa giữa các máy tính. Do Telnet hỗ trợ chế độ văn bản giao diện người dùng thường ở dạng dấu nhắc lệnh tương tác. Chúng ta có thể đánh lệnh và các trả lời sẽ được hiển thị.
- **HTTP(*Hyper Text Tranfer Protocol*)** :Trao đổi các tài liệu siêu văn bản để hỗ trợ cho WEB.
- **WWW(*World Wide Web*)** : là một khung làm việc có kiến trúc để truy cập các tài liệu liên kết trải khắp hàng ngàn máy trên tất cả mạng Internet.
- **SMTP(*Simple Mail Transfer Protocol*)** : Tuyển thư điện tử các máy tính. Đây là dạng đặc biệt của việc tuyển tin được sử dụng để gửi các thông báo tới một máy chủ thư điện tử( mail sever) hoặc giữa các mail sever với nhau.
- **POP3(*Post Office Protocol version 3*)** : Cho phép lấy thư ddienj tử từ hộp thư trên máy mail sever.
- **DNS(*Domain Name System*)** : Hệ thống chuyển đổi tên miền thành địa chỉ IP và ngược lại. Khi cần truy cập đến một Website trên Internet, người dùng có thể gõ địa chỉ IP của Website đó hoặc gõ tên DNS. Vì các địa chỉ IP rất khó nhớ, DNS là một dịch vụ đáng giá. Nó giúp mọi người tên để truy cập Internet.
- **DHCP(*Dynamic Host Configuration Protocol*)** : Giao thức cung cấp các thông tin cấu hình động cho các máy trạm. 
- **NNTP(*Network News Transfer Protocol*)** : Giao thức được đưa ra nhằm phục vụ nhóm tin trong hệ thống mạng. Nó cho phép trao đổi thư tín, bài báo và bản tin điện tử trên Internet.











     














