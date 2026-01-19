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

f/

<img width="590" height="125" alt="image" src="https://github.com/user-attachments/assets/e1d3a1b3-01a4-43ca-97c9-1295ef2d28f1" />

- giả sử mình đang ở folder ```temp``` mà muốn di chuyển tới ```temp2``` ta có thể sử dụng ```cd ../temp2```

<img width="419" height="93" alt="image" src="https://github.com/user-attachments/assets/9f144d97-d1a6-4055-895b-e60c246fa620" />

- có thể thấy ```mv``` không thể thay đổi hàng loạt được, ```*.txt``` được hiểu là file đích đến chứ k phải là mẫu đổi tên

  <img width="419" height="54" alt="image" src="https://github.com/user-attachments/assets/7efcc67f-856a-4396-9682-bb208534f5bd" />

- nhưng khi dùng tên file cụ thể thì ```mv ``` có thể hoạt động đúng yêu cầu

g/

<img width="617" height="170" alt="image" src="https://github.com/user-attachments/assets/428edfd3-69a5-4969-972a-400e1562bc47" />

- sau khi rời khỏi folder chứ ```sales.txt``` đã copy về thì mình sẽ không thể xóa được file đó vì hệ thống không thể xóa 1 file mà k có ở thư mục đang ở được, có thể vào thư mục chứ file để xóa hoặc sử dụng đường dẫn tuyệt đối

  <img width="376" height="121" alt="image" src="https://github.com/user-attachments/assets/665e829f-25a7-4115-9998-0e1b08a45205" />

- ```rm *.dat``` sẽ xóa toàn bộ file chứ đuôi ```.dat``` chứ trong thư mục đó

h/

<img width="379" height="123" alt="image" src="https://github.com/user-attachments/assets/90eeadfb-97c7-4109-93c1-68592bc4950a" />

- sau khi trả lời là n thì file sẽ không bị xóa
- để ```rm``` luôn có thể dùng option ```-i``` ta có thể tạo ```alias rm='rm -i'``` để có thể sử dụng vĩnh viễn ta có thể thêm dòng này vào ```~/.bashrc```

<img width="413" height="108" alt="image" src="https://github.com/user-attachments/assets/7a787a4b-0c13-4c9d-b3fd-99f4c787be0a" />

i/

<img width="376" height="124" alt="image" src="https://github.com/user-attachments/assets/151cb595-1b26-4857-820a-532c62ed8d98" />

- ```rm``` không thể xóa được thư mục, để xóa đc thư mục ta cần dùng lệnh ```rm dir```

<img width="513" height="38" alt="image" src="https://github.com/user-attachments/assets/3134afe0-fe7e-4a41-bb2c-fbe64630b35b" />

- ```rmdir``` chỉ có thể xóa file rỗng, để xóa được folder ```directory2``` ta cần xóa hết file trong thư mục trước, sử dụng ```rm *``` để xóa hết file trong 1 thư mục

<img width="526" height="175" alt="image" src="https://github.com/user-attachments/assets/e98ce7cd-8101-4dcf-b6df-1b3b880237fb" />

<img width="613" height="246" alt="image" src="https://github.com/user-attachments/assets/76ce9770-e62b-491a-b636-ec5f615a30c3" />

- sử dụng ```rm -r``` có thể xóa thư mục và toàn biij file con, folder con trong thư mục đó

j/

<img width="641" height="376" alt="image" src="https://github.com/user-attachments/assets/74883e8f-f6c0-4e30-a7c1-265f982fc15f" />

- thư mục ```new``` chỉ chiếm 6 bytes vì là thư mục rỗng, các quyền của thư mục giống hầu hết các thứ mục trong ảnh vì đều đc user tạo ra, có thể sẽ có trường hợp khác quyền khi thư mục đc tạo bởi các user được cấp quyền khác nhau

k/

<img width="495" height="145" alt="image" src="https://github.com/user-attachments/assets/23a87c0f-f8fe-42c1-8d20-5b0e06513386" />

- sử dụng ```mv + wildcard``` để di chuyển các file tới thư mục new

# 3

a/ 

- ```cat passwd``` dùng để dọc hết toàn bộ nội dung trong file

<img width="600" height="416" alt="image" src="https://github.com/user-attachments/assets/21ea2dab-af3a-48a2-8852-09a5a3d91904" />

- ```head passwd``` sẽ hiển thị 10 dòng đầu trong file

<img width="398" height="212" alt="image" src="https://github.com/user-attachments/assets/207972ab-7577-4951-9d0b-edb1085f4cd3" />

- ```tail passwd``` sẽ hiển thị 10 dòng cuối

<img width="655" height="194" alt="image" src="https://github.com/user-attachments/assets/564fba9e-f7af-4584-b688-92411ed4d375" />

b/

- ```taill -c 100 passwd``` sẽ hiển thị 100 byte cuối cùng trong file

<img width="647" height="171" alt="image" src="https://github.com/user-attachments/assets/fcc7fcad-a1c9-4573-bd81-004c8a8c5acf" />

- ```head -n 5 passwd``` dùng để đọc 5 dòng đầu của file

<img width="418" height="119" alt="image" src="https://github.com/user-attachments/assets/19306866-f392-403d-9fa5-0763c5c4ba42" />

c/

- ```head -n -10 passwd``` hiển thị toàn bộ file trừ 10 dòng cuối
- ```tail -c +100 passwd``` hiển thị file bắt đầu thừ byte thứ 100 trở đi

d/

- để in ra toàn bộ file từ dòng 6 trở đi ta sử dụng ```tail -n +6 passwd```

e/

<img width="433" height="243" alt="image" src="https://github.com/user-attachments/assets/deb931da-526a-4dfc-b687-82f98582daa5" />

- ```file a*``` sẽ trả lại các file bắt đầu từ ký tự ```a``` và loại file của các file đó

<img width="500" height="260" alt="image" src="https://github.com/user-attachments/assets/ac65a22b-6e1f-45af-9900-316d699f4385" />

- tương tự ```file a*``` nhưng khi thêm option ```-i``` vào thì output thay vì in ra các loại file để có thể đọc hiểu thì option sẽ in ra file sử dụng nội dung gì 

# 4

a/

<img width="482" height="294" alt="image" src="https://github.com/user-attachments/assets/0abdb12a-36f3-4f11-b0e6-2c62ad19412d" />

- ```cmp temp1.txt temp2.txt``` dùng để so sánh sự khác nhau giữa 2 file , khi này output chỉ ra tại dòng thứ 2 đã sai lệch nhau

<img width="481" height="108" alt="image" src="https://github.com/user-attachments/assets/8ceadbbf-6501-42fa-a2f6-019dbfebb6cf" />

- tương tự vầy nhưng ```diff``` sẽ chỉ trực tiếp sự khác nhau

b/

<img width="518" height="324" alt="image" src="https://github.com/user-attachments/assets/53202f7d-b750-4db1-9053-384b55ed2fb1" />

- em cũng không hiểu rõ tại sao join lại không hoạt động

<img width="481" height="121" alt="image" src="https://github.com/user-attachments/assets/b33a976d-83ae-4339-88b8-54501a1b50b2" />
 
# 5

a/

<img width="626" height="151" alt="image" src="https://github.com/user-attachments/assets/bd37e01b-493d-474a-a42a-cc7669c7c1e9" />

- cốt thứ 2 trong đó là số hard link trỏ tới file đó

<img width="662" height="137" alt="image" src="https://github.com/user-attachments/assets/f0ae0d2a-be83-4ec4-aff4-4749de96a192" />

- ```cat addresses``` có thể đọc file từ đường dẫn tới ```addresses.txt``` nhwung do em chưa ghi gì =)))))

b/

<img width="663" height="154" alt="image" src="https://github.com/user-attachments/assets/8e02da32-d8d4-4266-bdaf-a59349440529" />

c/

<img width="665" height="360" alt="image" src="https://github.com/user-attachments/assets/e7ce44fe-4568-4fde-b98f-5ad771d2948c" />








