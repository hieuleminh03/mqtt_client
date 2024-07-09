## Ghi chú

 - Publish được QoS 0. Subcribe được QoS 0 hoặc QoS 1.
 - Cỡ message cả header là **256 bytes** (mặc định). Chỉnh qua 
 `MQTT_MAX_PACKET_SIZE` trong `PubSubClient.h` 
 hoặc gọi `PubSubClient::setBufferSize(size)`.
 - Mặc định connection sẽ đợi 15 giây. Có thể chỉnh qua `MQTT_KEEPALIVE` trong `PubSubClient.h` hoặc gọi
   `PubSubClient::setKeepAlive(keepAlive)`.
 - Client mặc định dùng MQTT 3.1.1. Chỉnh qua MQTT 3.1 bằng cách đổi
   giá trị `MQTT_VERSION` trong `PubSubClient.h`.


## Phần cứng

Phát triển cho:
 - ESP8266
 - ESP32