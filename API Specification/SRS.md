1. GIỚI THIỆU
1.1. Mục đích của tài liệu

Tài liệu Software Requirements Specification (SRS) mô tả các yêu cầu của hệ thống CAB System – nền tảng đặt xe được xây dựng cho Công ty ABC.

Tài liệu nhằm xác định rõ phạm vi của hệ thống, các tác nhân tham gia, yêu cầu chức năng, yêu cầu phi chức năng, quy tắc nghiệp vụ, các trường hợp ngoại lệ và những vấn đề cần được xác nhận với khách hàng trước khi triển khai.

Tài liệu là cơ sở để Business Analyst, Developer, Tester và các bên liên quan thống nhất về yêu cầu của hệ thống trong quá trình phát triển.

1.2. Phạm vi hệ thống

CAB System là nền tảng hỗ trợ doanh nghiệp quản lý toàn bộ quy trình đặt xe trực tuyến, bắt đầu từ khi khách hàng tạo yêu cầu đặt xe cho đến khi chuyến đi hoàn thành, thanh toán và đánh giá tài xế.

Hệ thống bao gồm các chức năng chính:

Quản lý tài khoản khách hàng.
Quản lý tài khoản tài xế.
Quản lý phương tiện.
Đặt xe.
Tìm kiếm và phân công tài xế.
Theo dõi trạng thái chuyến đi.
Cập nhật vị trí tài xế.
Tính cước chuyến đi.
Thanh toán.
Gửi và quản lý thông báo.
Đánh giá tài xế.
Quản lý chuyến đi.
Quản lý khách hàng và tài xế.
Quản lý phương tiện.
Theo dõi hoạt động vận hành.
Tra cứu lịch sử giao dịch.
Báo cáo và thống kê.
Phân quyền người dùng.
Ghi nhận nhật ký các thao tác quan trọng.
1.3. Mục tiêu hệ thống

Hệ thống CAB System được xây dựng nhằm:

Giảm sự phụ thuộc vào việc phân công tài xế thủ công.
Tự động hóa quy trình tìm kiếm và phân công tài xế.
Giúp khách hàng dễ dàng đặt và theo dõi chuyến xe.
Quản lý tập trung thông tin chuyến đi và thanh toán.
Hỗ trợ doanh nghiệp quản lý khách hàng, tài xế và phương tiện.
Cung cấp dữ liệu phục vụ vận hành và báo cáo.
Có khả năng hoạt động ổn định khi số lượng người dùng tăng.
Cho phép mở rộng thêm dịch vụ, phương thức thanh toán và kênh thông báo trong tương lai.
Cho phép các thành phần được phát triển và triển khai độc lập nhằm hạn chế ảnh hưởng đến toàn bộ hệ thống.
1.4. Thời gian thực hiện

Dự án dự kiến được xây dựng và triển khai trong thời gian 7 tuần.

Trong thời gian này, nhóm thực hiện các hoạt động phân tích yêu cầu, thiết kế, phát triển, kiểm thử và triển khai phiên bản đầu tiên của hệ thống.

2. MÔ TẢ TỔNG QUAN HỆ THỐNG
2.1. Mô tả sản phẩm

CAB System là một nền tảng đặt xe trực tuyến cho phép khách hàng gửi yêu cầu chuyến đi thông qua hệ thống.

Sau khi khách hàng nhập điểm đón, điểm đến và lựa chọn loại xe, hệ thống tiếp nhận yêu cầu và tìm kiếm tài xế phù hợp.

Hệ thống dựa trên vị trí, trạng thái hoạt động và các tiêu chí vận hành để lựa chọn tài xế. Khi tài xế nhận chuyến, hệ thống thông báo cho khách hàng và cập nhật trạng thái chuyến đi.

Trong quá trình thực hiện chuyến, tài xế cập nhật trạng thái và vị trí. Sau khi chuyến hoàn thành, hệ thống tính cước, thực hiện hoặc ghi nhận thanh toán và cho phép khách hàng đánh giá tài xế.

Nhân viên vận hành sử dụng giao diện quản trị để theo dõi và xử lý các hoạt động của hệ thống.

2.2. Các tác nhân của hệ thống
Khách hàng

Khách hàng là người sử dụng dịch vụ đặt xe.

Khách hàng có thể:

Đăng ký tài khoản.
Đăng nhập.
Cập nhật thông tin cá nhân.
Nhập điểm đón.
Nhập điểm đến.
Lựa chọn loại xe.
Đặt xe.
Theo dõi trạng thái chuyến đi.
Theo dõi thông tin tài xế.
Xem thời gian dự kiến tài xế đến.
Xem lịch sử chuyến đi.
Xem số tiền phải trả.
Thanh toán.
Đánh giá tài xế.
Tài xế

Tài xế là người nhận và thực hiện chuyến xe.

Tài xế có thể:

Đăng ký tài khoản hoặc được nhân viên tạo tài khoản.
Đăng nhập.
Cập nhật hồ sơ cá nhân.
Cập nhật thông tin phương tiện.
Chuyển trạng thái hoạt động.
Nhận thông báo chuyến xe.
Chấp nhận chuyến.
Từ chối chuyến.
Cập nhật trạng thái chuyến.
Cập nhật vị trí.
Hoàn thành chuyến.
Nhân viên vận hành

Nhân viên vận hành chịu trách nhiệm theo dõi và hỗ trợ hoạt động của hệ thống.

Nhân viên có thể:

Quản lý khách hàng.
Quản lý tài xế.
Quản lý phương tiện.
Theo dõi chuyến đi.
Kiểm tra trạng thái tài xế.
Hỗ trợ xử lý chuyến bị lỗi.
Tra cứu lịch sử giao dịch.
Theo dõi hoạt động của hệ thống.
Quản trị viên

Quản trị viên có quyền thực hiện các thao tác quản trị có tính nhạy cảm.

Quản trị viên có thể:

Quản lý tài khoản nhân viên.
Phân quyền người dùng.
Quản lý các cấu hình hệ thống.
Xem nhật ký thao tác.
Quản lý các thông tin vận hành quan trọng.
Theo dõi báo cáo và thống kê.
Nhà cung cấp thanh toán

Nhà cung cấp thanh toán là hệ thống bên ngoài được tích hợp để xử lý các giao dịch thanh toán điện tử.

CAB System không lưu trực tiếp thông tin nhạy cảm của thẻ hoặc tài khoản thanh toán.

Nhà cung cấp thông báo

Nhà cung cấp thông báo là hệ thống bên ngoài hỗ trợ gửi thông báo đến khách hàng hoặc tài xế.

Hệ thống được thiết kế để có thể bổ sung thêm các nhà cung cấp hoặc kênh thông báo trong tương lai.

3. YÊU CẦU CHỨC NĂNG
3.1. Quản lý tài khoản khách hàng
FR-01: Đăng ký tài khoản

Hệ thống phải cho phép khách hàng đăng ký tài khoản bằng các thông tin cần thiết.

Hệ thống phải kiểm tra tính hợp lệ của thông tin đăng ký và đảm bảo tài khoản không bị trùng theo quy tắc được doanh nghiệp xác định.

FR-02: Đăng nhập

Hệ thống phải cho phép khách hàng đăng nhập bằng thông tin xác thực hợp lệ.

Nếu thông tin đăng nhập không chính xác, hệ thống phải thông báo lỗi.

FR-03: Cập nhật thông tin cá nhân

Khách hàng có thể cập nhật các thông tin cá nhân được phép thay đổi.

Hệ thống phải xác thực người dùng trước khi thực hiện thao tác.

4. ĐẶT XE
FR-04: Tạo yêu cầu đặt xe

Khách hàng có thể tạo yêu cầu đặt xe bằng cách cung cấp:

Điểm đón.
Điểm đến.
Loại dịch vụ hoặc loại xe.
Các thông tin cần thiết khác.

Sau khi tiếp nhận, hệ thống tạo một chuyến đi và chuyển sang trạng thái tìm tài xế.

FR-05: Xác nhận yêu cầu đặt xe

Sau khi khách hàng gửi yêu cầu, hệ thống phải thông báo rằng yêu cầu đã được tiếp nhận.

Hệ thống bắt đầu quá trình tìm kiếm tài xế phù hợp.

FR-06: Tìm kiếm tài xế

Hệ thống phải xác định danh sách tài xế phù hợp dựa trên:

Vị trí hiện tại của tài xế.
Trạng thái sẵn sàng.
Loại phương tiện.
Loại dịch vụ.
Các tiêu chí vận hành khác.

Hệ thống ưu tiên những tài xế phù hợp và ở gần khách hàng.

FR-07: Phân công tài xế

Hệ thống gửi yêu cầu chuyến xe đến tài xế phù hợp.

Nếu tài xế chấp nhận, hệ thống gán tài xế cho chuyến đi.

Nếu tài xế từ chối hoặc không phản hồi trong thời gian quy định, hệ thống tiếp tục tìm tài xế khác.

Khách hàng không cần tạo lại yêu cầu đặt xe.

FR-08: Xử lý trường hợp không tìm được tài xế

Nếu hệ thống không tìm được tài xế phù hợp, hệ thống phải thông báo rõ ràng cho khách hàng.

Hệ thống phải lưu lại trạng thái của yêu cầu để phục vụ việc kiểm tra và thống kê.

5. QUẢN LÝ CHUYẾN ĐI
FR-09: Theo dõi trạng thái chuyến

Khách hàng có thể theo dõi trạng thái hiện tại của chuyến đi.

Các trạng thái dự kiến gồm:

Đang tìm tài xế.
Đã có tài xế.
Tài xế đang đến.
Tài xế đã đến điểm đón.
Đã đón khách.
Đang di chuyển.
Hoàn thành.
Đã hủy.
Thất bại.
FR-10: Cập nhật trạng thái chuyến

Tài xế có thể cập nhật trạng thái chuyến trong quá trình thực hiện.

Hệ thống phải kiểm tra trạng thái hiện tại trước khi cho phép chuyển sang trạng thái tiếp theo.

FR-11: Theo dõi vị trí tài xế

Hệ thống phải hỗ trợ ghi nhận vị trí của tài xế trong quá trình hoạt động.

Dữ liệu vị trí được sử dụng để:

Tìm tài xế gần khách hàng.
Hỗ trợ ước tính thời gian tài xế đến.
Hỗ trợ nhân viên vận hành theo dõi chuyến.
6. QUẢN LÝ TÀI XẾ
FR-12: Quản lý tài khoản tài xế

Hệ thống cho phép tài xế đăng ký hoặc cho phép nhân viên vận hành tạo tài khoản.

Thông tin tài xế phải được lưu trữ và bảo vệ.

FR-13: Cập nhật hồ sơ tài xế

Tài xế có thể cập nhật các thông tin cá nhân được phép thay đổi.

FR-14: Quản lý phương tiện

Hệ thống cho phép lưu trữ và quản lý thông tin phương tiện của tài xế.

Thông tin có thể bao gồm:

Biển số xe.
Loại xe.
Mẫu xe.
Thông tin nhận dạng phương tiện.
Trạng thái phương tiện.
FR-15: Cập nhật trạng thái hoạt động

Tài xế có thể chuyển trạng thái hoạt động khi bắt đầu hoặc kết thúc thời gian làm việc.

Các trạng thái dự kiến:

Sẵn sàng.
Đang bận.
Không hoạt động.
Đang thực hiện chuyến.
7. TÍNH CƯỚC
FR-16: Tính cước chuyến đi

Sau khi chuyến đi hoàn thành, hệ thống phải xác định số tiền khách hàng cần thanh toán.

Số tiền được tính dựa trên:

Loại dịch vụ.
Thông tin chuyến đi.
Các quy tắc tính cước do doanh nghiệp quy định.

Công thức tính cước cụ thể cần được xác nhận với doanh nghiệp trước khi triển khai.

FR-17: Hiển thị số tiền phải trả

Hệ thống phải hiển thị số tiền khách hàng cần thanh toán sau khi chuyến đi hoàn thành.

8. THANH TOÁN
FR-18: Thanh toán tiền mặt

Hệ thống phải hỗ trợ phương thức thanh toán bằng tiền mặt.

Sau khi xác nhận thanh toán, hệ thống phải lưu trạng thái giao dịch.

FR-19: Thanh toán điện tử

Hệ thống phải cho phép khách hàng thanh toán thông qua nhà cung cấp thanh toán bên ngoài.

CAB System không được lưu trực tiếp thông tin nhạy cảm của thẻ hoặc tài khoản thanh toán.

FR-20: Xử lý thanh toán thất bại

Nếu thanh toán điện tử thất bại, hệ thống phải:

Thông báo kết quả cho khách hàng.
Ghi nhận trạng thái giao dịch.
Cho phép thực hiện lại thanh toán theo chính sách của doanh nghiệp.
FR-21: Tra cứu giao dịch

Nhân viên vận hành có thể tra cứu lịch sử giao dịch để hỗ trợ khách hàng và xử lý sự cố.

9. THÔNG BÁO
FR-22: Thông báo cho khách hàng

Hệ thống phải gửi thông báo cho khách hàng khi:

Yêu cầu đặt xe được tiếp nhận.
Có tài xế nhận chuyến.
Tài xế đến điểm đón.
Chuyến đi hoàn thành.
Thanh toán thành công hoặc thất bại.
Có thay đổi quan trọng liên quan đến chuyến đi.
FR-23: Thông báo cho tài xế

Tài xế phải nhận được thông báo khi:

Có chuyến mới phù hợp.
Chuyến bị thay đổi.
Chuyến bị hủy.
Có thông tin quan trọng liên quan đến chuyến đang thực hiện.
FR-24: Mở rộng kênh thông báo

Hệ thống phải được thiết kế để có thể tích hợp thêm các kênh thông báo trong tương lai mà không phải thay đổi toàn bộ hệ thống.

10. ĐÁNH GIÁ
FR-25: Đánh giá tài xế

Sau khi chuyến đi hoàn thành, khách hàng có thể đánh giá tài xế.

Hệ thống phải lưu thông tin đánh giá gắn với chuyến đi và tài xế.

FR-26: Quản lý đánh giá

Nhân viên có quyền được phân công có thể xem và quản lý thông tin đánh giá phục vụ việc theo dõi chất lượng dịch vụ.

11. QUẢN TRỊ VÀ VẬN HÀNH
FR-27: Quản lý khách hàng

Nhân viên vận hành có thể:

Xem thông tin khách hàng.
Tra cứu khách hàng.
Cập nhật thông tin được phép.
Kiểm tra lịch sử chuyến đi.
FR-28: Quản lý tài xế

Nhân viên vận hành có thể:

Xem danh sách tài xế.
Tra cứu tài xế.
Kiểm tra trạng thái hoạt động.
Quản lý thông tin tài xế.
Kiểm tra lịch sử chuyến đi.
FR-29: Quản lý chuyến đi

Nhân viên vận hành có thể:

Xem các chuyến đang diễn ra.
Tra cứu chuyến đi.
Kiểm tra trạng thái chuyến.
Hỗ trợ xử lý chuyến bị lỗi.
Xem lịch sử chuyến đi.
FR-30: Quản lý phương tiện

Nhân viên có quyền có thể xem và quản lý thông tin phương tiện.

FR-31: Phân quyền

Hệ thống phải hỗ trợ phân quyền dựa trên vai trò.

Nhân viên thông thường không được phép thực hiện các thao tác nhạy cảm nếu không có quyền.

FR-32: Ghi nhật ký hoạt động

Hệ thống phải ghi nhận các thao tác quan trọng của người dùng và nhân viên quản trị.

Thông tin nhật ký có thể bao gồm:

Người thực hiện.
Thời gian.
Thao tác.
Đối tượng bị tác động.
Kết quả thao tác.
12. BÁO CÁO VÀ THỐNG KÊ
FR-33: Báo cáo số lượng chuyến

Hệ thống phải cung cấp báo cáo về số lượng chuyến theo khoảng thời gian.

FR-34: Báo cáo doanh thu

Hệ thống phải cung cấp thông tin doanh thu theo khoảng thời gian được lựa chọn.

FR-35: Báo cáo trạng thái chuyến

Hệ thống phải thống kê:

Tỷ lệ chuyến hoàn thành.
Tỷ lệ chuyến hủy.
Tỷ lệ chuyến thất bại.
FR-36: Báo cáo hiệu quả tài xế

Hệ thống hỗ trợ thống kê hiệu quả hoạt động của tài xế dựa trên dữ liệu chuyến đi.

13. YÊU CẦU PHI CHỨC NĂNG
NFR-01: Hiệu năng

Hệ thống phải có khả năng phục vụ số lượng lớn khách hàng và tài xế đồng thời.

Các chức năng quan trọng như tạo yêu cầu đặt xe, tìm tài xế và cập nhật trạng thái phải có thời gian phản hồi phù hợp.

Các ngưỡng cụ thể cần được xác định thông qua yêu cầu về tải thực tế của doanh nghiệp.

NFR-02: Khả năng mở rộng

Các thành phần của hệ thống phải có khả năng mở rộng độc lập khi tải tăng.

Hệ thống phải cho phép bổ sung thêm người dùng, tài xế và dịch vụ mà không cần thay đổi toàn bộ hệ thống.

NFR-03: Tính sẵn sàng

Hệ thống phải hoạt động ổn định trong các thời điểm nhu cầu tăng cao.

Lỗi của một thành phần như thanh toán hoặc thông báo không được làm cho toàn bộ chức năng đặt xe ngừng hoạt động.

NFR-04: Khả năng chịu lỗi

Khi một dịch vụ bên ngoài gặp lỗi, hệ thống phải có khả năng xử lý lỗi phù hợp và duy trì các chức năng không bị ảnh hưởng.

Ví dụ, nếu dịch vụ thanh toán gặp lỗi, khách hàng vẫn có thể xem thông tin chuyến đi.

NFR-05: Bảo mật

Hệ thống phải yêu cầu xác thực đối với các chức năng cần tài khoản.

Thông tin quản trị phải được kiểm soát quyền truy cập.

Thông tin cá nhân, thông tin phương tiện, dữ liệu vị trí và dữ liệu giao dịch phải được bảo vệ.

NFR-06: Bảo vệ dữ liệu thanh toán

Hệ thống không được lưu trực tiếp các thông tin nhạy cảm của thẻ hoặc tài khoản thanh toán.

Việc xử lý thông tin thanh toán điện tử phải được thực hiện thông qua nhà cung cấp thanh toán bên ngoài.

NFR-07: Khả năng mở rộng chức năng

Hệ thống phải cho phép bổ sung:

Loại dịch vụ mới.
Phương thức thanh toán mới.
Nhà cung cấp thanh toán mới.
Kênh thông báo mới.

Việc bổ sung không được yêu cầu xây dựng lại toàn bộ hệ thống.

NFR-08: Khả năng bảo trì

Các thành phần của hệ thống phải được tổ chức rõ ràng để dễ dàng bảo trì và nâng cấp.

NFR-09: Khả năng triển khai độc lập

Các thành phần có thể được triển khai hoặc cập nhật từng phần nhằm hạn chế ảnh hưởng đến những chức năng đang hoạt động.

NFR-10: Kiểm toán

Các thao tác quan trọng phải được ghi nhận để phục vụ việc kiểm tra và điều tra khi xảy ra sự cố.

14. QUY TẮC NGHIỆP VỤ
BR-01

Chỉ khách hàng đã xác thực mới được phép tạo yêu cầu đặt xe.

BR-02

Chỉ tài xế ở trạng thái sẵn sàng mới được xem xét để nhận chuyến.

BR-03

Tài xế phải có phương tiện hợp lệ để được phân công chuyến.

BR-04

Một chuyến đi chỉ được gán cho một tài xế tại một thời điểm.

BR-05

Nếu tài xế từ chối chuyến, hệ thống phải tiếp tục tìm tài xế khác.

BR-06

Nếu tài xế không phản hồi trong thời gian quy định, hệ thống phải xử lý tương tự trường hợp không nhận chuyến.

BR-07

Khách hàng không cần tạo lại yêu cầu nếu quá trình tìm tài xế thất bại ở một tài xế cụ thể.

BR-08

Chỉ tài xế được phân công mới được phép cập nhật trạng thái của chuyến tương ứng.

BR-09

Chỉ chuyến đã hoàn thành mới được thực hiện bước tính cước cuối cùng.

BR-10

Khách hàng chỉ được đánh giá tài xế sau khi chuyến hoàn thành.

BR-11

Thông tin thanh toán nhạy cảm không được lưu trực tiếp trong CAB System.

BR-12

Các thao tác quản trị nhạy cảm phải yêu cầu quyền phù hợp.

15. QUY TRÌNH NGHIỆP VỤ CHÍNH
15.1. Quy trình đặt xe

Khách hàng đăng nhập vào hệ thống.

Khách hàng nhập điểm đón và điểm đến.

Khách hàng lựa chọn loại xe hoặc dịch vụ.

Khách hàng gửi yêu cầu đặt xe.

Hệ thống tiếp nhận yêu cầu.

Hệ thống tìm kiếm tài xế phù hợp.

Hệ thống gửi yêu cầu đến tài xế.

Tài xế chấp nhận chuyến.

Hệ thống xác nhận tài xế cho khách hàng.

Tài xế di chuyển đến điểm đón.

Tài xế xác nhận đã đến.

Tài xế đón khách.

Tài xế cập nhật trạng thái đang di chuyển.

Tài xế hoàn thành chuyến.

Hệ thống tính cước.

Khách hàng thanh toán.

Hệ thống ghi nhận kết quả thanh toán.

Khách hàng đánh giá tài xế.

Chuyến đi kết thúc.

16. CÁC TRƯỜNG HỢP NGOẠI LỆ
EX-01: Không tìm được tài xế

Nếu hệ thống không tìm được tài xế phù hợp, hệ thống thông báo cho khách hàng rằng hiện tại chưa có tài xế phù hợp.

EX-02: Tài xế từ chối chuyến

Hệ thống chuyển sang tìm kiếm tài xế tiếp theo.

EX-03: Tài xế không phản hồi

Nếu tài xế không phản hồi trong thời gian quy định, hệ thống tiếp tục tìm tài xế khác.

EX-04: Thanh toán thất bại

Hệ thống thông báo thanh toán thất bại và cho phép khách hàng thực hiện lại theo chính sách doanh nghiệp.

EX-05: Mất kết nối

Khi khách hàng hoặc tài xế mất kết nối mạng, hệ thống phải đảm bảo dữ liệu đã được xác nhận không bị mất.

Khi kết nối được khôi phục, ứng dụng phải có khả năng đồng bộ trạng thái phù hợp.

EX-06: Tài xế hủy chuyến

Hệ thống phải xử lý theo chính sách hủy chuyến được doanh nghiệp xác định và có thể tìm tài xế thay thế nếu chính sách cho phép.

EX-07: Lỗi dịch vụ bên ngoài

Nếu dịch vụ thanh toán hoặc thông báo không hoạt động, hệ thống phải ghi nhận lỗi và không làm ảnh hưởng đến toàn bộ chức năng đặt xe.

17. TÍCH HỢP HỆ THỐNG
17.1. Tích hợp dịch vụ thanh toán

CAB System sẽ tích hợp với nhà cung cấp thanh toán bên ngoài.

Hệ thống gửi yêu cầu thanh toán đến nhà cung cấp.

Nhà cung cấp trả về kết quả giao dịch.

CAB System lưu trạng thái giao dịch thay vì lưu thông tin nhạy cảm của phương thức thanh toán.

17.2. Tích hợp dịch vụ bản đồ và vị trí

Hệ thống có thể tích hợp với dịch vụ bản đồ để:

Xác định vị trí.
Hỗ trợ tìm tài xế gần khách hàng.
Xác định khoảng cách.
Hỗ trợ tính thời gian dự kiến tài xế đến.
Hỗ trợ theo dõi chuyến đi.
17.3. Tích hợp dịch vụ thông báo

Hệ thống có thể tích hợp với các dịch vụ gửi thông báo bên ngoài.

Kiến trúc phải cho phép thay đổi hoặc bổ sung nhà cung cấp thông báo trong tương lai.

18. DỮ LIỆU CHÍNH CỦA HỆ THỐNG

Hệ thống dự kiến quản lý các nhóm dữ liệu chính:

Khách hàng

Bao gồm thông tin tài khoản và thông tin cá nhân.

Tài xế

Bao gồm thông tin tài khoản, hồ sơ và trạng thái hoạt động.

Phương tiện

Bao gồm thông tin phương tiện và trạng thái phương tiện.

Chuyến đi

Bao gồm:

Mã chuyến.
Khách hàng.
Tài xế.
Điểm đón.
Điểm đến.
Loại xe.
Thời gian.
Trạng thái.
Thông tin cước.
Giao dịch

Bao gồm:

Mã giao dịch.
Mã chuyến.
Số tiền.
Phương thức thanh toán.
Trạng thái.
Thời gian giao dịch.
Đánh giá

Bao gồm:

Khách hàng.
Tài xế.
Chuyến đi.
Điểm đánh giá.
Nội dung đánh giá.
Thời gian đánh giá.
Vị trí tài xế

Bao gồm thông tin vị trí và thời gian cập nhật.

Thông báo

Bao gồm người nhận, nội dung, loại thông báo, thời gian và trạng thái gửi.

Nhật ký hệ thống

Bao gồm người thực hiện, thao tác, thời gian và đối tượng bị tác động.

19. PHÂN QUYỀN

Hệ thống dự kiến có các nhóm quyền:

Khách hàng

Chỉ được truy cập và thao tác trên dữ liệu tài khoản và chuyến đi của mình.

Tài xế

Được quản lý hồ sơ, phương tiện và các chuyến được phân công.

Nhân viên vận hành

Được quản lý và theo dõi các đối tượng nghiệp vụ theo quyền được cấp.

Quản trị viên

Có quyền quản trị hệ thống, phân quyền và thực hiện các thao tác nhạy cảm.

20. CÁC YÊU CẦU CHƯA ĐƯỢC XÁC ĐỊNH

Một số yêu cầu hiện tại chưa có thông tin đầy đủ và cần Business Analyst làm rõ với khách hàng.

20.1. Cách tính cước

Cần xác định:

Giá cơ bản.
Giá theo khoảng cách.
Giá theo thời gian.
Phụ phí.
Giá theo từng loại xe.
Chính sách giá vào giờ cao điểm.
20.2. Tiêu chí ưu tiên tài xế

Cần xác định mức độ ưu tiên dựa trên:

Khoảng cách.
Thời gian chờ.
Trạng thái tài xế.
Loại xe.
Hiệu suất tài xế.
Các tiêu chí vận hành khác.
20.3. Thời gian phản hồi của tài xế

Cần xác định tài xế có bao nhiêu giây hoặc phút để chấp nhận hoặc từ chối chuyến.

20.4. Chính sách hủy chuyến

Cần xác định:

Ai được phép hủy.
Thời điểm được hủy.
Có tính phí hủy hay không.
Mức phí hủy.
Trường hợp tài xế hủy.
Trường hợp khách hàng hủy.
20.5. Xử lý mất kết nối

Cần xác định:

Thời gian chờ khi mất kết nối.
Cách đồng bộ dữ liệu.
Cách xử lý trạng thái chuyến khi mất kết nối.
20.6. Thời gian lưu trữ dữ liệu

Cần xác định thời gian lưu trữ:

Thông tin khách hàng.
Thông tin tài xế.
Lịch sử chuyến đi.
Giao dịch.
Dữ liệu vị trí.
Nhật ký hệ thống.
21. GIẢ ĐỊNH VÀ RÀNG BUỘC
21.1. Giả định

Hệ thống được triển khai trên nền tảng có kết nối Internet.

Khách hàng và tài xế sử dụng thiết bị có khả năng kết nối với hệ thống.

Nhà cung cấp thanh toán và dịch vụ thông báo cung cấp API để hệ thống tích hợp.

Dữ liệu bản đồ và vị trí được cung cấp bởi dịch vụ bên ngoài phù hợp.

21.2. Ràng buộc

Thời gian phát triển phiên bản đầu tiên là 7 tuần.

Hệ thống phải đảm bảo các yêu cầu bảo mật đối với dữ liệu người dùng.

Không được lưu trực tiếp thông tin nhạy cảm của phương thức thanh toán.

Hệ thống phải có khả năng mở rộng trong tương lai.

Các thành phần phải được thiết kế theo hướng giảm sự phụ thuộc lẫn nhau.

22. TIÊU CHÍ NGHIỆM THU TỔNG QUÁT

Hệ thống được xem là đáp ứng yêu cầu khi:

Khách hàng có thể đăng ký và đăng nhập.
Khách hàng có thể tạo yêu cầu đặt xe.
Hệ thống có thể tìm kiếm và phân công tài xế.
Tài xế có thể nhận hoặc từ chối chuyến.
Hệ thống có thể tiếp tục tìm tài xế khác khi tài xế từ chối hoặc không phản hồi.
Khách hàng có thể theo dõi trạng thái chuyến.
Tài xế có thể cập nhật trạng thái chuyến.
Hệ thống có thể tính cước.
Khách hàng có thể thanh toán bằng các phương thức được hỗ trợ.
Hệ thống có thể xử lý kết quả thanh toán thất bại.
Khách hàng và tài xế nhận được các thông báo cần thiết.
Khách hàng có thể đánh giá tài xế sau chuyến.
Nhân viên có thể quản lý khách hàng, tài xế, phương tiện và chuyến đi.
Hệ thống hỗ trợ phân quyền.
Hệ thống ghi nhận các thao tác quan trọng.
Hệ thống có báo cáo và thống kê cơ bản.
Các chức năng chính vẫn hoạt động khi một dịch vụ phụ trợ gặp lỗi.
Kiến trúc cho phép mở rộng các dịch vụ trong tương lai.
23. KẾT LUẬN

CAB System được xây dựng nhằm thay thế quy trình đặt xe và phân công tài xế thủ công bằng một nền tảng trực tuyến có khả năng tự động hóa và mở rộng.

Hệ thống tập trung vào toàn bộ quy trình từ đặt xe, tìm kiếm tài xế, thực hiện chuyến, tính cước, thanh toán, thông báo đến đánh giá.

Bên cạnh các chức năng nghiệp vụ, hệ thống phải chú trọng đến khả năng mở rộng, bảo mật, tính sẵn sàng, khả năng chịu lỗi và khả năng tích hợp với các dịch vụ bên ngoài.

Các vấn đề chưa được xác định như cách tính cước, tiêu chí ưu tiên tài xế, thời gian phản hồi, chính sách hủy chuyến, xử lý mất kết nối và thời gian lưu trữ dữ liệu cần được Business Analyst trao đổi với các bên liên quan trước khi nhóm phát triển hoàn thiện thiết kế và triển khai hệ thống.
