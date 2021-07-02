'Duckiebots in the Duckietown' จากหุ่นยนต์เป็ดน้อยขับเคลื่อนแบบสองล้อราคาถูก ควบคุมด้วยบอร์ด Raspberry Pi ไปสู่การเรียนรู้ด้าน 'ปัญญาประดิษฐ์และหุ่นยนต์' ในระดับมหาวิทยาลัย
‍‍‍
Duckietown 'เมืองของเป็ด' (http://duckietown.mit.edu/) เป็นชื่อของแพลตฟอร์ม (Platform) ที่มีจุดเริ่มต้นจากชั้นเรียนที่มหาวิทยาลัย MIT (Massachusetts Institute of Technology) สำหรับการเรียนรู้ด้านหุ่นยนต์ (Robotics) การมองเห็นของเครื่องจักร (Computer Vision) ปัญญาประดิษฐ์ (AI) เพื่อการพัฒนายานยนต์ไร้คนขับ (Self-Driving Cars)

‍‍‍

โครงการนี้เริ่มต้นในปีค.ศ. 2016 ปัจจุบันได้มีการจัดตั้ง Duckietown Foundation (https://www.duckietown.org/) มาดูแล เพื่อเผยแพร่ความรู้ต่อสาธารณะ และมีการนำเนื้อหาไปสอนในชั้นเรียนระดับมหาวิทยาลัยชั้นนำของโลก มากกว่า 10 แห่ง ทั้งในทวีปอเมริกาเหนือ ยุโรป และเอเชีย
(https://www.duckietown.org/instructors/classes)
‍‍‍
แพลตฟอร์มประกอบด้วยสองส่วน คือ

▫️ 'Duckietowns' เป็นสถานที่หรือสนามจำลอง เพื่อให้หุ่น Duckiebots หลาย ๆ ตัววิ่งไปตามถนน มีขอบถนน เส้นแบ่งช่องทาง มีป้ายจราจร (เช่น ใช้ QR code) หรือสิ่งกีดขวาง เป็นต้น

▫️ 'Duckiebots' เป็นหุ่นยนต์เคลื่อนที่ได้ราคาถูก (mobile robots)
‍‍‍‍‍‍ ‍‍- ใช้บอร์ด Raspberry Pi 3 เป็นตัวประมวลผลหลัก
‍‍‍‍‍‍ ‍‍- เชื่อมต่อผ่าน Wi-Fi ได้
‍‍‍‍‍‍ ‍‍- ใช้กล้อง (Raspberry Pi camera module + Fisheye lens) เป็นกล้องมองด้านหน้า (forward-facing camera) ซึ่งเป็นเซนเซอร์ชนิดเดียวเท่านั้น ดังนั้นจึงต้องใช้การประมวลผลภาพในการนำทาง (Vision-based navigation)
‍‍‍‍‍‍ ‍‍- ใช้บอร์ด Adafruit DC motor HAT (for DC motors) สำหรับขับมอเตอร์ไฟฟ้ากระแสตรง 1 คู่
- บอร์ด Adafruit 16­-Channel PWM / Servo HAT / External DC Power Supply
‍‍‍‍‍‍ ‍‍- ใช้แหล่งพลังงานไฟฟ้าจาก 5V USB Powerbank
‍‍‍‍‍‍ ‍‍- ใช้ระบบปฏิบัติการ Raspbian + ROS support (Robotics Operating System) สำหรับเขียนโปรแกรมควบคุมหุ่นยนต์ และสามารถเขียนโปรแกรมด้วยภาษา Python
‍‍‍‍‍‍ ‍‍- สามารถใช้ซอฟต์แวร์ด้าน Machine Learning เช่น PyTorch, Caffe, Tensorflow หรือใช้งานกับอุปกรณ์ Intel Movidius Neural Compute Stick ได้เช่นกัน
‍‍‍‍‍‍ ‍‍
ผู้เรียนสามารถจำลองการทำงานในสิ่งแวดล้อมเสมือนแบบ 3 มิติ โดยใช้ซอฟต์แวร์ RVIZ for ROS (http://wiki.ros.org/rviz) ซึ่งเป็น Open Source
‍‍‍‍‍‍ ‍‍
Duckietown มีกิจกรรมแข่งขันอย่างเช่น AI Driving Olympics ที่มีโจทย์ให้หุ่นยนต์วิ่งไปตามลู่วิ่งหรือถนน (Lane following) การหลบหลีกสิ่งกีดขวาง (Obstacle avoidance) การนำทางจากจุดหนึ่งไปสู่อีกจุดหนึ่ง (Point-to-point navigation) ไปจนถึงโจทย์ที่ยากขึ้น เช่น การทำงานร่วมกันของฝูงหุ่นยนต์ (Coordination of a vehicle fleet)
‍‍‍‍‍‍ ‍‍
เอกสารบนเว็บไซต์ (http://duckietown.mit.edu/materials.html) ก็มีให้ศึกษาได้เต็มที่ เช่น สอนประกอบหุ่นยนต์ สอนการลง Raspbian-based Duckbot image (duckiebot-RPI3 -> Raspbian ROS) การสอนใช้คำสั่ง Linux และติดตั้งโปรแกรมและตั้งค่าให้ระบบ การเขียนโปรแกรมด้วยภาษา Python เป็นต้น
‍‍‍‍‍‍ ‍‍
แม้ว่าเนื้อหาการเรียนรู้ของ Duckietown จะดูเหมาะสำหรับระดับมหาวิทยาลัย แต่การให้เยาวชนเห็นความเชื่อมโยง เริ่มต้นจากการเริ่มใช้หุ่นยนต์ราคาไม่แพงในลักษณะนี้ การติดตั้งซอฟต์แวร์ตามขั้นตอนและใช้งานเบื้องต้น เพื่อใช้เป็นสื่อการเรียนรู้ต่อไปในระดับมหาวิทยาลัยได้ ถือว่าน่าสนใจไม่น้อยเลย
‍‍‍‍‍‍ ‍‍ ‍‍‍‍‍‍
References / Credit
- Duckietown

🔗 https://www.duckietown.org/
- Duckietown Documentation

🔗 http://docs.duckietown.org/
- Paper: "Duckietown: an Open, Inexpensive and Flexible Platform for Autonomy Education and Research"

🔗 http://www.mit.edu/~hangzhao/papers/duckietown.pdf