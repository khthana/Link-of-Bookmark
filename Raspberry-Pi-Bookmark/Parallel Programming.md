Parallel Programming
Credit : Sittisak Sakamornlertsakul

สองสามอาทิตย์ที่ผ่านมา อารมณ์อยากเรียนรู้ Parallel Programming ของผมก็พุ่งถึงขีดสุด จึงได้รวบรวม Rpi ที่มีอยู่มาประกอบกันเป็น Cluster Computer ขึ้นมา โดยมี Master หนึ่งตัว และ Nodes อีกสามตัว บอกตรงๆครับ ไม่เคยรู้เรื่อง Parallel Programming มาก่อนเลย แต่พอมาเล่นจริงๆ ปรากฏว่ามันง่ายกว่าที่คิดมากครับ ใครที่สนใจ ผมแนะนำขั้นตอนง่ายๆดังนี้เลยครับ
1. ดูคลิปสองอันนี้เพื่อประกอบเครื่องและ Setup ครับ

https://www.youtube.com/watch?v=1R0UgIgcb5g
https://www.youtube.com/watch?v=lHmFRlETTcQ

หมายเหตุ ในขั้นตอนการติดตั้ง MPI นั้นไม่จำเป็นต้องไป Compile ตามคลิปครับ เดี๋ยวนี้มันมีมาให้เรียบร้อย ถ้าใช้ Raspbien Jessie ก็ให้ใช้คำสั่งเดียว จบเลย sudo apt-get install python-mpi4py (อะไรชีวิตจะสะดวกปานนั้น)

2. เมื่อมีเครื่องพร้อมรบแล้วก็ทำความเข้าใจ Parallel Programming ด้วยเพจนี้เลยครับ ไม่ยาวมากแต่ปูความเข้าใจได้เลย http://www.meccanismocomplesso.org/…/cluster-e-programmazi…/
ในข้อสอง ตัวอย่างสุดท้ายในการคำนวณหาค่า Pi ผมรองรันดู ถ้าใช้ Node เดียว เวลาที่ต้องใช้ในการประมวลผล ประมาณ 265 วินาที แต่ถ้าใช้ 3 Nodes นี่เหลือแค่ 90 วินาที เรียกว่าลดเวลากันเห็นๆ ถ้ามีหลายๆตัวต่อกันนี่ มันเป็น Super Computer ได้จริงๆเลยครับ งานวิจัยที่ต้องมีการคำนวนโหดๆน่าเอาไปใช้มากครับ
ส่วนใครที่จะต่อยอดจริงๆจังๆ ก็ควรอ่านตรงนี้เพิ่มเติมครับ เป็น Tutorial จาก นาซ่าครับ https://www.nccs.nasa.gov/tutorials/mpi_tutorial/
