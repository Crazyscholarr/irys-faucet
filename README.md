## Irys-Faucet Tutorial
Welcome to the irys-faucet tutorial! This is an automated tool that helps you request tokens from the Irys faucet (https://irys.xyz/faucet) using multiple wallets and proxies. This tutorial will guide you through the steps to install and run the program easily.

### 1. Prerequisites
Before you start using the program, you need to prepare the following:

Required software
Node.js: Make sure you have Node.js installed (version 14 or higher). Download from: https://nodejs.org/
A text editor like Visual Studio Code, Notepad++, or any other you like.
Required files
wallets.txt: List of wallet addresses you want to use to receive tokens.
proxies.txt: List of proxies to send requests to (provided in your code).

config.yaml: Configuration file containing API key and language information.
Captcha Solving Service Account
You need an account from 2Captcha or CapSolver to solve captchas automatically.
Get the API key from your account (2CAPTCHA_KEY or CAPSOLVER_KEY).
### 2. Install the Program
Step 1: Download the source code
Copy all the code in the index.js file you provided and save it as a file named index.js on your computer.
Step 2: Prepare the files
Create a wallets.txt file:
Open a text editor, enter each wallet address (one wallet on a line). For example:
``
0x1234567890abcdef1234567890abcdef12345678
0xabcdef1234567890abcdef1234567890abcdef12
``
Save the file as wallets.txt in the same directory as index1.js.
Create or use the proxies.txt file:
You have provided a long list of proxies in the proxies.txt file. Copy this list to a text file and save it as proxies.txt in the same directory as index.js.
Make sure each proxy is on its own line, for example:
``
http://156.228.124.164:3128
http://156.228.81.69:3128
``
Create a config.yaml file:
Copy the following content, replacing it with your API key, and save it as config.yaml in the same directory:
yaml
``
captcha_provider: '2captcha' # Replace with 'capsolver' if using CapSolver
2CAPTCHA_KEY: 'your_2captcha_api_key_here'
CAPSOLVER_KEY: 'your_capsolver_api_key_here'
language: 'vi' # Replace with 'en' if using English
Replace your_2captcha_api_key_here or your_capsolver_api_key_here with your actual API key.
``
Step 3: Install the necessary libraries:
```bash
npm install chalk
npm install axios
npm install fs
npm install @2captcha/captcha-solver
npm install capsolver-npm
npm install js-yaml
npm install readline
```
### 3. Run the Program
```bash
node index1.js
```
Hướng Dẫn Sử Dụng Chương Trình Irys-Faucet
Chào mừng bạn đến với hướng dẫn sử dụng chương trình irys-faucet! Đây là một công cụ tự động giúp bạn yêu cầu token từ faucet của Irys (https://irys.xyz/faucet) bằng cách sử dụng nhiều ví và proxy. Hướng dẫn này sẽ dẫn bạn qua từng bước để cài đặt và chạy chương trình một cách dễ dàng.

# 1. Yêu Cầu Trước Khi Bắt Đầu
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
# 2. Cài Đặt Chương Trình
  Bước 1: Tải mã nguồn
Sao chép toàn bộ mã trong tệp index.js mà bạn đã cung cấp và lưu thành tệp có tên index.js trên máy tính của bạn.
  Bước 2: Chuẩn bị các tệp
      Tạo tệp wallets.txt:
      Mở một trình chỉnh sửa văn bản, nhập từng địa chỉ ví (mỗi ví trên một dòng). Ví dụ:
``
              0x1234567890abcdef1234567890abcdef12345678
              0xabcdef1234567890abcdef1234567890abcdef12
``
          Lưu tệp với tên wallets.txt trong cùng thư mục với index1.js
      Tạo hoặc sử dụng tệp proxies.txt:
          Bạn đã cung cấp một danh sách proxy dài trong tệp proxies.txt. Sao chép danh sách này vào một tệp văn bản và lưu với tên proxies.txt trong cùng thư mục với index.js.
          Đảm bảo mỗi proxy nằm trên một dòng, ví dụ:
          ```bash
            http://156.228.124.164:3128
            http://156.228.81.69:3128
            ```
      Tạo tệp config.yaml:
          Sao chép nội dung sau, thay thế API key của bạn, rồi lưu thành config.yaml trong cùng thư mục:
          yaml
```bash
          captcha_provider: '2captcha'  # Thay bằng 'capsolver' nếu dùng CapSolver
          2CAPTCHA_KEY: 'your_2captcha_api_key_here'
          CAPSOLVER_KEY: 'your_capsolver_api_key_here'
          language: 'vi'  # Thay bằng 'en' nếu muốn dùng tiếng Anh
        Thay your_2captcha_api_key_here hoặc your_capsolver_api_key_here bằng API key thực tế của bạn.
```
  Bước 3: Cài đặt các thư viện cần thiết: 
```bash
  npm install chalk
  npm install axios
  npm install fs
  npm install @2captcha/captcha-solver
  npm install capsolver-npm
  npm install js-yaml
  npm install readline
```
3. Chạy Chương Trình
```bash
  node index1.js
```

