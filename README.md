# YÊU CẦU ĐẦU RA

## phần 1: Phân tích
- Sai lầm của bạn An về bản chất câu lệnh tiềm kiếm là
 
  Lệnh Get-childitem là lệnh để tìm ví trí và danh sách các file trong FODER mà An lại dùng câu lệnh ấy để tìm nội dung "404" nên kết quả trả lại mới trống rỗng dù trong
  file Log có rất nhiều lỗi 404

 - Phân biệt 2 câu lệnh

   1: Lệnh Get-childitem là câu lệnh dùng để tìm ví trịa và danh sách các filr trong FODER

    2: Lệnh Select-String là câu lệnh dùng để chọn nội dung mà mình tìm kiếm trong tệp mà mình đã chọn

## Phần 2: Hoàn thiện 

Câu lệnh PowerShell chuẩn để lọc các dòng chứa chữ "ERROR" từ file access.log là

Select-String access.log -Pattern "ERROR"
