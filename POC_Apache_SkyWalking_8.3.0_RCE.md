<h2>POC APACHE SKYWALKING 8.3.0 RCE</h2>
Apache Skywalking là công cụ giám sát hiệu suất ứng dụng cho các hệ thống phân tán, được thiết kế đặc biệt cho các kiến trúc vi dịch vụ, đám mây gốc và dựa trên container (Docker, Kubernetes, Mesos).<br><br>
Trong giao diện GraphQL của Apache Skywalking 8.3.0 và các phiên bản trước đó, có lỗ hổng tiêm SQL vào cơ sở dữ liệu H2.

<h2>VULNERABILITY ENVIRONMENT</h2>
Cài đặt Apache SkyWalking phiên bản 8.3.0<br>

<h2>Prerequisites</h2>
Yêu cầu cài đặt môi trường Java(JDK) phiên bản 8 trở lên trên hệ thống của mình<br>

```bash
sudo apt update && sudo apt install openjdk-11-jdk -y
```
Thiết lập môi trường
