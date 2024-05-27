# 3ddose-analysis

## Giới thiệu
Code này dùng để đọc file 3ddose, sau đó tính tổng năng lượng lắng đọng trong phantom, và vẽ profile.

## Giải Thích Quy Trình

### Bước 1: Đọc Dữ Liệu từ File 3ddose
Hàm `read_3ddose` đọc file 3ddose và trả về tọa độ x, y, z, liều và sai số.

### Bước 2: Tính Kích Thước Voxel
Hàm `calculate_voxel_size` nhận vào các tọa độ ranh giới và tính toán kích thước của mỗi voxel.

### Bước 3: Xác định mật độ
Ở đây, mật độ của chất liệu được xác định, trong ví dụ này là 1.0 g/cm³.

### Bước 4: Tính Toán Năng Lượng Lắng Đọng
Sử dụng kích thước voxel và mật độ để chuyển đổi liều thành năng lượng lắng đọng trong hàm `calculate_energy_deposited`.

### Bước 5: Vẽ Profile
Các hàm vẽ profile giúp bạn hình dung sự phân bố năng lượng lắng đọng dọc theo các trục x, y, và z tại vị trí trung tâm của các trục còn lại.

## Hướng dẫn sử dụng

# Khai báo Đường dẫn đến file 3ddose.
#file_path = 'DPK_Lu177.3ddose'
# file_path = 'DPK_Cu67.3ddose'
# file_path = 'DPK_Sc47.3ddose'
# file_path = 'DPK_Tb161.3ddose'
