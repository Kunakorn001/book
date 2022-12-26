# Remote Database

1.ให้เราตั้งค่า SQL Service Agen ในเครื้องที่เราจะให้การ Remote โดยมีวิธีการเข้าดังนี้\
1.1กด ปุ่มWindow \
1.2 เลือกFolder Microsoft SQL Server 2019 \
1.3จากนั้นเข้าไปที่ SQL Server 2019 Configuration

![](<../../.gitbook/assets/image (19).png>)

2.เมื่อเราเปิด SQL Server 2019 Configuration  แล้วกดเข้าไปที่ SQL Server Service&#x20;

![](<../../.gitbook/assets/image (79).png>)

3.จากนั้นให้เราคลิกขวาที่ SQL Service Agen แล้วกด Start&#x20;

![](<../../.gitbook/assets/image (39).png>)

4.จากนั้นให้เราไปกำหนด ip สำหรับ ใช้รีโหมด โดยให้เราเข้าไปที่ SQL Server Network Configuration ->Protocols for Test2 -> TCP/IP&#x20;

![](<../../.gitbook/assets/image (70).png>)

5.จากนั้น ให้เรากดเข้าไปเพื่อเปิดการใช้งาน

![](<../../.gitbook/assets/image (48).png>)

6.จากนั้นให้เราเลือกไปที่เมนู IP Address  เพื่อกำหนด Port  หรืออะไรซักอย่างเนี่ยแหละที่จะทำให้เราสามารถ Remote ได้ โดยต้องกำหนดPort เป็น 1433 และ กด Enabled

![](<../../.gitbook/assets/image (12).png>)

7.จากนั้นเราจะทำการConnect ip ระหว่างเครื่องที่จะทำการ Remote เข้าไป กับ เครื่องที่เป็นเครื่อง Remote โดยให้เราเปิด CMD ขึ้นมาทั้งสองเครื่อง และพิมพ์ (ipconfig)เพื่อเป็นการเช็ค IP ของทั้งสองเครื้อง จากนั้น เมื่อทราบ ip แล้วให้ทำการพิมพ์คำสั่ง \
(ping ตามด้วยIPจากอีกเครื้องแล้วตามด้วย -t)

![](<../../.gitbook/assets/image (60).png>) ![](<../../.gitbook/assets/image (23).png>)

8.เมื่อเราทำการ Connect ip เสร็สแล้วให้เปิด SQL Management ในเครื้องที่เราจะทำการ Remote ขึ้นมา&#x20;

![](<../../.gitbook/assets/image (25).png>)

9.ถัดมาในส่วนของ Server Name ให้เราใส่ IP ของเครื่องที่เราจะทำการ Remote เข้าไป จากนั้นก็ใส่ Username กับPassword แล้วกด Connect&#x20;

![](<../../.gitbook/assets/image (64).png>)

10.เท่านี้ก็เป็นอันเสร็สสิ้น การ Remote

![](<../../.gitbook/assets/image (16).png>)
