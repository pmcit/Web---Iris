Ứng dụng web phân loại hoa Iris (Triển khai bằng Flask)
Chương trình này áp dụng các khái niệm cơ bản về máy học (phân loại) trên Dữ liệu Iris của Fisher để dự đoán loài của một mẫu hoa Iris mới.

Phần mềm và Thư viện

Python 3.6.0
Anaconda 4.3.0 (32 bit)
scikit-learn 0.18.1
Giới thiệu
Bộ dữ liệu cho dự án này có nguồn gốc từ Kho lưu trữ máy học UCI . Bộ dữ liệu hoa Iris hoặc bộ dữ liệu Iris của Fisher là một bộ dữ liệu đa biến được nhà thống kê và nhà sinh vật học người Anh Ronald Fisher giới thiệu trong bài báo năm 1936 của ông có tên Sử dụng nhiều phép đo trong các vấn đề phân loại học như một ví dụ về phân tích phân biệt tuyến tính.

Bộ dữ liệu bao gồm 50 mẫu từ mỗi loài trong ba loài Iris (Iris setosa, Iris virginica và Iris versicolor).
Bốn đặc điểm được đo từ mỗi mẫu (tính bằng centimet):
Chiều dài của lá đài
Chiều rộng của lá đài
Chiều dài của cánh hoa
Chiều rộng của cánh hoa
Hoạt động của iris_decision_tree_classifier

Chương trình lấy dữ liệu từ load_iris()hàm có sẵn trong sklearnmô-đun.
Sau đó, chương trình sẽ tạo ra một cây quyết định dựa trên tập dữ liệu để phân loại.
Sau đó, người dùng được yêu cầu nhập bốn thông số của mẫu và dự đoán về loài hoa sẽ được in ra cho người dùng.
Hoạt động của iris_selfmade_KNN

Chương trình lấy dữ liệu từ load_iris()hàm có sẵn trong sklearnmô-đun.
Sau đó, chương trình chia tập dữ liệu thành các mẫu đào tạo và thử nghiệm theo tỷ lệ 80:20 một cách ngẫu nhiên bằng train_test_learn()hàm có sẵn trong sklearnmô-đun.
Không gian mẫu đào tạo được sử dụng để đào tạo chương trình và các dự đoán được đưa ra trên không gian mẫu thử nghiệm.
Điểm chính xác sau đó được tính bằng cách so sánh với kết quả chính xác của tập dữ liệu đào tạo.
