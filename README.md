# Webserver-log-analyst-using-HDFS-Spark-Yarn-cluster

Đề tài này tập trung vào việc phân tích các tệp log của máy chủ web bằng sử dụng một hệ thống xử lý dữ liệu lớn sử dụng Hadoop Distributed File System (HDFS), Apache Spark trên YARN Cluster. Bằng cách kết hợp sức mạnh của HDFS để lưu trữ lượng dữ liệu lớn và Spark để xử lý hiệu quả các phân tích, đề tài nhằm cải thiện khả năng xử lý dữ liệu và khám phá thông tin hữu ích từ tệp log máy chủ web.

**Dataset:**
- Online Shopping Store - Web Server Logs
- Kích thước của bộ dữ liệu là 3.3GB, khoảng hơn 10 triệu dòng log, định dạng file text, mỗi một dòng đại diện cho một record của một lần request gửi về phía server.
- Mẫu record:

  54.36.149.41 - - [22/Jan/2019:03:56:14 +0330] "GET /filter/27|13%20%D9%85%DA%AF%D8%A7%D9%BE%DB%8C%DA%A9%D8%B3%D9%84,27|%DA%A9%D9%85%D8%AA%D8%B1%20%D8%A7%D8%B2%205%20%D9%85%DA%AF%D8%A7%D9%BE%DB%8C%DA%A9%D8%B3%D9%84,p53 HTTP/1.1" 200 30577 "-" "Mozilla/5.0 (compatible; AhrefsBot/6.1; +http://ahrefs.com/robot/)" "-"


  31.56.96.51 - - [22/Jan/2019:03:56:16 +0330] "GET /image/60844/productModel/200x200 HTTP/1.1" 200 5667 "https://www.zanbil.ir/m/filter/b113" "Mozilla/5.0 (Linux; Android 6.0; ALE-L21 Build/HuaweiALE-L21) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/66.0.3359.158 Mobile Safari/537.36" "-"

**Cấu hình:** 

  Hadoop, Spark được chạy trên hai máy ảo Ubuntu trên VMWare. Bao gồm 1 máy master và 2 worker (hai máy ảo, một máy đảm nhiệm hai nhiệm vụ master và worker cùng lúc)

**Set up:** 

  Cách set up Hadoop, Spark, Yarn được tham khảo ở [đây](https://sparkbyexamples.com/apache-hadoop-tutorials-with-examples/)

**Một số phân tích**

![image](https://github.com/ChiThang-50Cent/Webserver-log-analyst-using-HDFS-Spark-Yarn-cluster/assets/62085284/59fcae05-19c0-4696-8ccb-d8d684404436)

