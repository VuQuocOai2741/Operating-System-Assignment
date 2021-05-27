# Operating System Assignment

Họ tên sinh viên: Vũ Quốc Oai

MSSV: 20172741

Mã môn học: ET4291

Mã lớp: 124887

Kì: 20202


Repository này chứa các file code đã sửa đổi để hoàn thành các yêu cầu của bài Alarm Clock, Project 1 Synchronization. Các file đã sửa đổi bao gồm:
1. thread.c và thread.h trong "src/threads/"
2. timer.c trong "src/devices"

Các phần code đã thay đổi được đặt trong cặp comments

/* code modified */

/* code modified */

Cụ thể các phần đã thay đổi code bao gồm
1. Trong "src/threads/thread.c"
- Line 206: khởi tạo cho biến time_left_to_sleep
- Line 325-336: định nghĩa hàm sleeping_time_decrease

2. Trong "src/threads/thread.h"
- Line 103: khai báo biến time_left_to_sleep
- Line 140: khai báo hàm sleeping_time_decrease

3. Trong "src/devices/timer.c"
- Line 105-118: chỉnh sửa hàm timer_sleep()
- Line 203: gọi đến hàm thread_foreach (sleeping_time_decrease, NULL) với hàm sleeping_time_decrease được định nghĩa trong "src/threads/thread.c"


Hầu hết các nguồn tài liệu tham khảo trong quá trình làm đề tài là các nguồn online. Các nguồn tham khảo bao gồm:
- Trang web chính thức của Stanford: https://web.stanford.edu/class/cs140/projects/pintos/pintos_2.html#SEC25

- Các tài liệu để hiểu rõ về ngắt: https://www.youtube.com/watch?v=rnGVincwk30
                                   https://www.youtube.com/watch?v=V1TJ6b6_EjM
                                   https://www.youtube.com/watch?v=KqgMGZyiLnU
                                   
- Các tài liệu để hiểu rõ hơn về tiến trình và luồng: https://www.youtube.com/watch?v=exbKr6fnoUw
                                                      https://www.youtube.com/watch?v=LOfGJcVnvAk
                                                      
- Các tài liệu để hiểu rõ về Process Synchronization problems: https://www.youtube.com/watch?v=BSX1YEoCVgA
                                                               https://www.youtube.com/watch?v=LRiN3DJdskA
                                                               https://www.youtube.com/watch?v=s8_ZxcG7Jco&list=PLbu9W4c-C0iAGUc7dQlqXIsXkGnHMaTEz
                                                               
- Các tài liệu để hiểu rõ hơn về vai trò của ngắt timer: https://www.youtube.com/watch?v=PtTVe0zfg_M
                                                         https://www.youtube.com/watch?v=m5_pFID-f-M
                                                         
- Tài liệu để hiểu rõ về cách debug trong Pintos: https://www.youtube.com/watch?v=4C8J6jLPJPc

- Ngoài các tài liệu tham khảo nêu trên, tài liệu tham khảo chính gồm các slides bài giảng và các notes trong quá trình học trên lớp
                                                        
Phần mô tả code được sửa đổi cũng như ý tưởng chung được trình bày chi tiết trong báo cáo. 
