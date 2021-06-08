# MICROPYTHON For Microcontroller

## Compare miropython with other specify languages (for MCU)
- Dễ học, dễ tiếp cận cho người mơi bắt đầu. Có thể học nhanh from the báics to doing real work, and quickly.
- Là ngôn ngữ phiên dịch (interpretive) nên feedback nhanh, có thể tương tác với MCU với 1 lệnh và 1 phản hồi sẽ trả lại ngay lâpj tức, ở đây ta sử dụng REPL. Có thể chỉnh sửa mã code và chạy ngay lập tức thay vì lăpj lại chu trình code-compile-upload-execute như các ngôn ngữ khác như C.
- Với sự phong phú của python thì có thể thực hiện 1 mối việc nhanh chóng và dễ dàng hơn với tư cách là 1 lập trình viên python. Ví dụ về thực hiện việc call api python sử dụng thư viện request, việc xử lý chuỗi string vfa JSON dễ dàng hơn nhiều khi sử dụng python hơn so với việc dùng C/C++.  


## Setup Micropython

1. Presetup
- kit NodeMCU(ESP8266)
- connect microUSB
- firmware micropython
2. Setup
  - install esptool
  ```
    pip install esptool
  ```
  - Xoa Flash
  ```
    esptool.py --port ten_cong_COM erase_flash
  ```
  (on macOS: --port=/dev/cu.SLAB_USBtoUART)
  
  - Write Firmware:
  ```
    esptool.py --port ten_cong_COM --baud 460800 write_flash --flash_size=detect 0 ten_file_firmware.bin
  ```
3. 
