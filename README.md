# Customers insight
Dự án nhỏ này khám phá các chỉ số về tình hình kinh doanh được ghi nhận tại 1 chuỗi cửa hàng đồ chơi dành cho trẻ em. Qua các phân tích từ đó có cái nhìn tổng quan hơn về tình hình kinh doanh của doanh nghiệp và qua đó có thể cải thiện tình hình kinh doanh.

## Mô tả file
File ghi chép tình hình hoạt động của chuỗi cửa hàng trong tháng 3 năm 2020. Số liệu được chuẩn bị ở dạng csv với 9 cột như sau:
- Brand: thương hiệu đồ chơi được bán
- Category Code: danh mục đồ chơi
- Category ID: id của danh mục đồ chơi
- Event time: thời gian tại thời điểm khách hàng thực hiện hành động
- Event type: hành động của khách hàng. Có 3 loại: view/cart/purchase
- Product ID: id sản phẩm
- User ID: id khách hàng
- User session: id phiên tạm thời của khách hàng
- Price: giá sản phẩm

### Link file
[OpenCDP_Kidstore.csv](https://drive.google.com/file/d/10xewZD2A1kYOtkddtlwWa8-s37A8YofN/view?usp=sharing)

## Hướng phân tích
> Xử lý với thư viện Pandas. Thực hiện câu lệnh thống kê mô tả để nắm được các thông tin như: các giá trị null, độ lệch chuẩn, giá trị min max, trung bình, giá trị tứ phân vị.
> Lọc cột Event type lấy các giá trị purchase. Thêm cột ngày được cắt từ event time. Vẽ biểu đồ doanh thu theo từng ngày.
> Tìm hãng có doanh thu lớn nhất bằng cách tương tự.
> Tách cột giờ từ event time. Tính tổng doanh thu và group by theo ngày. Vẽ biểu đồ doanh thu theo giờ.
