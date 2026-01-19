# 1
a/
- ```cd /``` dùng để chuyển thư mục hiện tại về tới thư mục / (root)

<img width="446" height="111" alt="image" src="https://github.com/user-attachments/assets/3ae3b088-3b13-46f6-97af-d65047f3947f" />

- sau khi dùng ```cd etc```, ```cd sysconfig```, ```cd networking```. Khi đó ta đang ở thư mục ```/etc/sysconfig/networking```.


<img width="599" height="53" alt="image" src="https://github.com/user-attachments/assets/5fc4cd97-3a7b-4e46-8c3c-299a8c2c4f3c" />

- sử dụng đường dẫn tuyệt đối ```cd /etc/sysconfig/network-screpts``` để di chuyển tới đường đãn thư mục đó
- ```..``` là thư mục cha của thư mục hiện tại, vậy ```../..``` là thư mục cha của cha của thư mục hiện tại ( jf4 là ông của thư mục hiện tại =)))) )
- sử dụng ```cd ../..``` để quay lại thư mục etc theo đường dẫn


<img width="346" height="160" alt="image" src="https://github.com/user-attachments/assets/f8af92a0-2836-4064-a847-ea30b29015ae" />


- ```~``` là đường dẫn tắt tới thư mục home trong user hiện tại sử dụng
- ```cd ~``` là 1 cách nhanh để trở về thư mục home
- ```cd ~Student``` là chuyển tới thu mục ```home``` của user ```student```, yêu cầu p có quyền truy cập mới có thể truy cập được thư mục home của các user khác

b/

<img width="452" height="157" alt="image" src="https://github.com/user-attachments/assets/b8beeffb-1ae1-4b02-b081-3e31d32ff375" />

c/

<img width="641" height="123" alt="image" src="https://github.com/user-attachments/assets/fd91dd2d-e616-4a26-b490-fa65a124746c" />

d/

<img width="643" height="209" alt="image" src="https://github.com/user-attachments/assets/66fa01e6-dc05-4423-9569-ec5b30165656" />

- ```wc``` ở thư mục ```/usr/bin/```
- ```ip``` ở thư mực ```/usr/sbin```

e/

<img width="648" height="153" alt="image" src="https://github.com/user-attachments/assets/8ab8d27e-64ac-48fb-9fb4-0952267f97e8" />

- lần đầu sử dụng ```which systemd``` out put sẽ là không thể tìm thấy ```systemd``` vì thư mục này vẫn chưa có trong PATH để lệnh ```which``` có thể tìm thấy

- ```PATH=$PATH:/usr/lib/systemd``` dùng để nối thêm đường đãn vào PATH, sau đó lệch ```which systemd``` có thể hoạt động

# 2

a/

<img width="643" height="376" alt="image" src="https://github.com/user-attachments/assets/08022fbf-9934-47ea-9df7-b61548c8f11a" />

- size của 4 file vừa tạo đều = 0

b/

<img width="599" height="203" alt="image" src="https://github.com/user-attachments/assets/c56fc015-5838-4a44-8461-2d90e36f7855" />

- sử dụng ```cp FILES/*.txt ~``` để copy file có đuôi .txt từ thư mục ```FILES``` ở user Student về thư mục ```home```

  <img width="648" height="206" alt="image" src="https://github.com/user-attachments/assets/e7d112a3-7a5f-494c-b363-0d722b0f8d9e" />

- sử dụng ```cp ~Student/FILES/DUMMY-DIRECTORY/directory2/* .``` để cp tất cả thư mục trong đường dẫn về thư mục hiện tại (home)

c/

- đề bài yêu cầu ta tạo 2 file ```aa1.abC```, ```aa10.bBC``` trong đó ```aa1.abC``` có kí tự ```hi```
- sau đó ```ls -l``` trả về kết quả size của file chứ kí tự là 3 byte còn size của file còn lại là 0 byte

<img width="644" height="109" alt="image" src="https://github.com/user-attachments/assets/74834974-aeed-45b7-960b-900293c423eb" />

- di chuyển tới đường đẫn ở 2b và tạo 2 file trắng có tên ý hệt, trờ về thư mục chứa 2 file ban đầu và sử dụng lệch ```cp -i``` để copy 2 fiel mới tạo ghi đè vào 2 file ban đầu
- option ```-i``` cảu lệch cp là option hỏi nếu sảy ra trường hợp file được copy tới trùng với file có sẵn 

<img width="659" height="192" alt="image" src="https://github.com/user-attachments/assets/c906c554-ba45-484e-b22c-8b2d7d544296" />

- khi nhập ```n``` là để từ chối việc ghi đè file, vì vậy sau khi sử dụng ```ls -l``` 2 file vẫn có size ban đầu
- nhưng khi nhập ```y``` là đồng ý ghi đè file

d/

<img width="662" height="178" alt="image" src="https://github.com/user-attachments/assets/7f198cbe-cfd5-4d2f-a3a6-1c3ea8252e06" />

- lệch ```cp -r``` dùng để copy toàn bộ thư mục và file trong thư mục đường đãn tới đích

e/

<img width="585" height="300" alt="image" src="https://github.com/user-attachments/assets/fe259dbe-37d7-4b0e-abb9-f553d897504c" />

- ```mv DUMMY-DIRECTORY temp2``` dùng để đổi tên thư mục ```DUMMY_DIRECTORY``` thành ```temp2```
- ```mv temp2 ..``` dùng để di chuyển thư mục temp2 tới thư mục cha của thư mục hiện tại
- mv có 2 các sử dụng 1 là đổi tên 2 là di chuyển

g/










