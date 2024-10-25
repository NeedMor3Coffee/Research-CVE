<h2>POC APACHE SKYWALKING 8.3.0 RCE</h2>
Apache Skywalking là công cụ giám sát hiệu suất ứng dụng cho các hệ thống phân tán, được thiết kế đặc biệt cho các kiến trúc vi dịch vụ, đám mây gốc và dựa trên container (Docker, Kubernetes, Mesos).<br><br>
Trong giao diện GraphQL của Apache Skywalking 8.3.0 và các phiên bản trước đó, có lỗ hổng tiêm SQL vào cơ sở dữ liệu H2.

<h2>VULNERABILITY ENVIRONMENT</h2>
Cài đặt Apache SkyWalking phiên bản 8.3.0<br>

<h2>PREREQUISITES</h2>
Yêu cầu cài đặt môi trường Java(JDK) phiên bản 8 trở lên trên hệ thống của mình<br>

```bash
sudo apt update && sudo apt install openjdk-11-jdk -y
```
Thiết lập môi trường
```bash 
export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64
```
<h2>DOWNLOAD APACHE SKYWALKING 8.3.0</h2>

```bash 
wget https://archive.apache.org/dist/skywalking/8.3.0/apache-skywalking-apm-8.3.0.tar.gz
```
Giải nén file apache-skywalking-apm-8.3.0.tar.gz 
```bash
tar -zxvf apache-skywalking-apm-8.3.0.tar.gz
```
Khởi chạy dịch vụ Apache SkyWalking 
```bash
cd apache-skywalking-apm-bin/bin
./startup.sh
```
Sau khi cài đặt thành công chúng ta có thể vào http://your-ip:8080 để xem trang web
<h2>POC APACHE SKYWALKING 8.3.0</h2>
![All Text](https://github.com/NeedMor3Coffee/Research-CVE/blob/main/img/hinh1.png)
Bây giờ chúng ta cùng nhau phân tích một chút về mã nguồn của Apache SkyWalking phiên bản 8.3.0. Chúng ta có thể thấy ở dòng thứ 





