Hướng Dẫn Sử Dụng Chương Trình Irys-Faucet
Chào mừng bạn đến với hướng dẫn sử dụng chương trình irys-faucet! Đây là một công cụ tự động giúp bạn yêu cầu token từ faucet của Irys (https://irys.xyz/faucet) bằng cách sử dụng nhiều ví và proxy. Hướng dẫn này sẽ dẫn bạn qua từng bước để cài đặt và chạy chương trình một cách dễ dàng.

1. Yêu Cầu Trước Khi Bắt Đầu
Trước khi sử dụng chương trình, bạn cần chuẩn bị những thứ sau:

Phần mềm cần thiết
Node.js: Đảm bảo bạn đã cài đặt Node.js (phiên bản 14 hoặc cao hơn). Tải tại: https://nodejs.org/
Một trình chỉnh sửa văn bản như Visual Studio Code, Notepad++, hoặc bất kỳ trình nào bạn thích.
Các tệp cần chuẩn bị
wallets.txt: Danh sách các địa chỉ ví bạn muốn sử dụng để nhận token.
proxies.txt: Danh sách các proxy để gửi yêu cầu (đã được cung cấp trong mã của bạn).
config.yaml: Tệp cấu hình chứa thông tin API key và ngôn ngữ.
Tài khoản dịch vụ giải captcha
Bạn cần một tài khoản từ 2Captcha hoặc CapSolver để giải mã captcha tự động.
Lấy API key từ tài khoản của bạn (2CAPTCHA_KEY hoặc CAPSOLVER_KEY).
2. Cài Đặt Chương Trình
  Bước 1: Tải mã nguồn
Sao chép toàn bộ mã trong tệp index.js mà bạn đã cung cấp và lưu thành tệp có tên index.js trên máy tính của bạn.
  Bước 2: Chuẩn bị các tệp
      Tạo tệp wallets.txt:
          Mở một trình chỉnh sửa văn bản, nhập từng địa chỉ ví (mỗi ví trên một dòng). Ví dụ:
              0x1234567890abcdef1234567890abcdef12345678
              0xabcdef1234567890abcdef1234567890abcdef12
          Lưu tệp với tên wallets.txt trong cùng thư mục với index1.js.
      Tạo hoặc sử dụng tệp proxies.txt:
          Bạn đã cung cấp một danh sách proxy dài trong tệp proxies.txt. Sao chép danh sách này vào một tệp văn bản và lưu với tên proxies.txt trong cùng thư mục với index.js.
          Đảm bảo mỗi proxy nằm trên một dòng, ví dụ:
            http://156.228.124.164:3128
            http://156.228.81.69:3128
      Tạo tệp config.yaml:
          Sao chép nội dung sau, thay thế API key của bạn, rồi lưu thành config.yaml trong cùng thư mục:
          yaml

          captcha_provider: '2captcha'  # Thay bằng 'capsolver' nếu dùng CapSolver
          2CAPTCHA_KEY: 'your_2captcha_api_key_here'
          CAPSOLVER_KEY: 'your_capsolver_api_key_here'
          language: 'vi'  # Thay bằng 'en' nếu muốn dùng tiếng Anh
        Thay your_2captcha_api_key_here hoặc your_capsolver_api_key_here bằng API key thực tế của bạn.
  Bước 3: Cài đặt các thư viện cần thiết: 

  npm install chalk
  npm install axios
  npm install fs
  npm install @2captcha/captcha-solver
  npm install capsolver-npm
  npm install js-yaml
  npm install readline
3. Chạy Chương Trình

  node index1.js
