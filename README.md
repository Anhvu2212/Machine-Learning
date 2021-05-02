# Machine-Learning


![SPARK](https://cdn-images-1.medium.com/max/650/0*jiEgRFH0McNEYGae.jpeg)

**1. Tại sao nên sử dụng Spark cho Học máy?**

Khi tạo mô hình học máy, khía cạnh quan trọng nhất để chuẩn bị mô hình là độ chính xác trong xử lý dữ liệu và tiết kiệm bộ nhớ máy tính. 
Nếu tập dữ liệu đã cho không phù hợp với bộ nhớ, thì phải sử dụng tính toán phân phối để tính toán một cụm có nhiều máy. 
Loại mô hình điện toán phân tán có sẵn cho đến bây giờ là HADOOP. 
Tuy nhiên, với SPARK, giờ đây bạn có thể xử lý dữ liệu từ các máy cục bộ độc lập và xây dựng mô hình dữ liệu với bộ dữ liệu đầu vào lớn hơn. 
Thông thường, các tập dữ liệu đầu vào này lớn hơn dung lượng bộ nhớ mà máy tính của bạn có. Đó là loại đàn hồi mà Apache Spark cung cấp. 
Do đó, Apache Spark được đặc trưng với Cơ sở hạ tầng đàn hồi. Điều này cho phép các nhà khoa học dữ liệu lặp lại các vấn đề dữ liệu nhanh hơn 100 lần so với HADOOP. 
Nó có 8000 nút tạo thành cụm lớn nhất thế giới được biết đến.

**2. Spark Mlib**

![SPARK](https://fbd67d5d-a-62cb3a1a-s-sites.googlegroups.com/site/irisforbigdata/3-supporting-tool1/machine-learning-lib-spark/SparkMLlib.png?attachauth=ANoY7cpj-Y8oI-YS4Hg7ICvvTiiUI7MR6xjHaBtahGQSS73vmC_3CCc1PeE3sqg1I-KgS5GK_v3TbpJdnmDVATFq5lSJvK12pjKq9TDrbhI8thwsRfsRGkJNvVGg-3wKkzmH6LL-yETM4qlk00oe3dN-rdVYAv9vCMei1IqDwbco4FnWXlaUrUJWrAC4TFeFP_0hD5dlOVfJjyNjDNyosVqLZEnupQSEbNNldUnlO9pPv0nbVVAKFHV-deJapbBeP88DI_H86KdClG244ZOOyZpT7df7WYfR-Q%3D%3D&attredirects=0)
Apache Spark cung cấp một API Học máy được gọi là MLlib . PySpark cũng có API học máy này bằng Python. Nó hỗ trợ các loại thuật toán khác nhau, được đề cập bên dưới:

**mllib.classification** - Gói spark.mllib hỗ trợ nhiều phương pháp khác nhau để phân loại nhị phân, phân loại đa lớp và phân tích hồi quy. Một số thuật toán phổ biến nhất trong phân loại là Rừng ngẫu nhiên, Vịnh Naive, Cây quyết định , v.v.

**mllib.clustering** - Clustering là một vấn đề học tập không có giám sát, theo đó bạn nhằm mục đích nhóm các tập con của các thực thể với nhau dựa trên một số khái niệm về sự giống nhau.

**mllib.fpm** - Đối sánh mẫu thường xuyên là khai thác các mục thường xuyên, tập phổ biến, chuỗi con hoặc các cấu trúc con khác thường nằm trong số các bước đầu tiên để phân tích một tập dữ liệu quy mô lớn. Đây đã là một chủ đề nghiên cứu tích cực trong việc khai thác dữ liệu trong nhiều năm.

**mllib.linalg** - Tiện ích MLlib cho đại số tuyến tính.

**mllib.recommendation** - Lọc cộng tác thường được sử dụng cho các hệ thống khuyến nghị. Các kỹ thuật này nhằm mục đích điền vào các mục còn thiếu của ma trận liên kết mục người dùng.

**spark.mllib** - Nó hiện hỗ trợ lọc cộng tác dựa trên mô hình, trong đó người dùng và sản phẩm được mô tả bằng một tập hợp nhỏ các yếu tố tiềm ẩn có thể được sử dụng để dự đoán các mục nhập bị thiếu. spark.mllib sử dụng thuật toán Bình phương tối thiểu xen kẽ (ALS) để tìm hiểu các yếu tố tiềm ẩn này.

**mllib.regression** - Hồi quy tuyến tính thuộc họ thuật toán hồi quy. Mục tiêu của hồi quy là tìm mối quan hệ và sự phụ thuộc giữa các biến. Giao diện làm việc với mô hình hồi quy tuyến tính và tóm tắt mô hình tương tự như trường hợp hồi quy logistic.
Spark MLlib được tích hợp chặt chẽ trên Spark giúp giảm bớt sự phát triển của các thuật toán học máy quy mô lớn hiệu quả như thường là lặp đi lặp lại trong tự nhiên.
Cộng đồng mã nguồn mở của Spark đã dẫn đến sự phát triển nhanh chóng và việc áp dụng Spark MLlib. Có hơn 200 cá nhân từ 75 tổ chức cung cấp khoảng hơn 2000 bản vá chỉ riêng cho MLlib.

MLlib dễ triển khai và không yêu cầu cài đặt trước, nếu Hadoop 2 cluster đã được cài đặt và đang chạy.
Khả năng mở rộng, tính đơn giản và khả năng tương thích ngôn ngữ của Spark MLlib (bạn có thể viết ứng dụng bằng Java, Scala và Python) giúp các nhà khoa học dữ liệu giải quyết các vấn đề dữ liệu lặp lại nhanh hơn. Các nhà khoa học dữ liệu có thể tập trung vào các vấn đề dữ liệu quan trọng trong khi tận dụng một cách minh bạch tốc độ, sự dễ dàng và tích hợp chặt chẽ của nền tảng thống nhất của Spark.
MLlib cung cấp hiệu suất cao nhất cho các nhà khoa học dữ liệu và nhanh hơn từ 10 đến 100 lần so với Hadoop và Apache Mahout. Các thuật toán học máy Alternating Least Squares trên Amazon Đánh giá trên tập dữ liệu gồm 660 triệu người dùng, 2,4 triệu mục và xếp hạng 3,5 B chạy trong 40 phút với 50 nút.
