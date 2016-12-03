# final_part_1
1.	การที่ใช้ Agile Method ไม่มีอะไรที่เหมือนกับ Waterfall Model เลยแต่ Waterfall Model ก็ยังเป็นวิธีการพัฒนาระบบที่ใช้กันอยู่ค่อนข้างแพร่หลาย 
ซึ่งวิธีนี้จะมีลำดับขั้นตอนที่ตายตัว เริ่มตั้งแต่รวบรวมข้อมูล กำหนดความต้องการของผู้ใช้ วิเคราะห์ทางเลือก ออกแบบ เขียนโปรแกรม ทดสอบระบบและสุดท้ายทำการติดตั้งระบบ 
โดยแต่ละส่วนของขั้นตอนดังกล่าวจะถือเป็นตัววัดความก้าวหน้าของงาน ปัญหาสำคัญของ Waterfall Model คือ ขั้นตอนของการพัฒนาที่ไม่ยืดหยุ่นเพราะตัวงานจะแบ่งเป็นช่วงๆ
แบบตายตัว ทำให้มีข้อผูกมัดตั้งแต่เริ่มโครงงานและไม่สามารปรับเปลี่ยนความต้องการผู้ ใช้ได้ หมายความว่าการพัฒนาโดยใช้ Waterfall Model นั้น ไม่เหมาะกับงานที่ความต้องการ
ของผู้ใช้เข้าใจยากและมีแนวโน้มว่าจะเปลี่ยนแปลงตลอดเวลา ในทางกลับกัน Agile Method จะแบ่งงานออกเป็นส่วนย่อยๆ แล้วค่อยๆ ทดสอบไปเรื่อยๆทุกสัปดาห์หรือทุกสองสัปดาห์ 
ทั้งนี้จะเน้นสร้างส่วนย่อยที่สุดของงานทั้งหมดที่สามารถใช้งานได้ทีละชิ้น เพื่อให้ส่งมอบได้รวดเร็วและทำการปรับปรุงเพิ่มเติมอย่างต่อเนื่องตลอดช่วงเวลาของโครงงาน 
ดังนั้น การใช้ Agile ไม่ใช่เรื่องผิด เป็นเรื่องดีด้วยซ้ำที่เราได้ทำตามแบบที่ลูกค้าต้องการ ถ้าไม่มีลูกค้าเราก็ไม่มีงาน 

2.	Git และ Github กับ centralized อย่าง CVS หรือ SVN มีการใช้งานในรูปแบบที่แตกต่างกัน ก็คือ Git เป็น distributed version control system ที่เราสามารถแยก 
version control ออกเป็น repo ย่อยๆได้ แต่ละ repo ย่อยก็สามารถทำ versioning ของตัวเองได้อีกที (เป็น local repo ที่ไม่เกี่ยวกับ remote repo เลย) 
ส่วน SVN นั้นเป็น centralized version control system คือ version ทั้งหมดจะถูกเก็บที่ remote repo ดังนั้น version ของทุกคนในทีมก็จะตรงกันทั้งหมด 
ไม่มี local repo ประเด็นนี้ก็เลยทำให้ Git สามารถทำงานแบบ offline ได้ คือ clone repo มาแล้วจะแก้ไขโค้ดแล้ว commit ไปยัง local repo ก่อนได้ ส่วน SVN นั้น 
ทุกครั้งที่ commit นั้นต้องไปอัพเดท version กับ server (commit ไปยัง SVN server) ถ้า offline อยู่ หรือเชื่อมต่อกับ server ไม่ได้ ก็จะไม่สามารถ commit ได้ 
ด้วยการทำงานที่แตกต่างกัน ก็ขึ้นอยู่กับคนที่เลือกใช้งานมากกว่าว่าถนัดที่จะใช้อะไร ให้เหมาะสมกับงานที่ทำ

3.	Code 
git branch feature1
git add '*.txt'
git commit -m "I just added new two pages on create feature1"
git push origin <branch>

4.	ในการพัฒนา software ส่วนใหญ่ต้องทำงานเป็นทีมนั่นคือต้องมีคนทำงานร่วมกันมากกว่า 1 คนต้องทำงานบน source code ชุดเดียวกัน 
ดังนั้นมีบ่อยครั้งที่ทำการแก้ไข source code เดียวกัน พร้อม ๆ กัน ส่งผลให้เกิดปัญหา คือ Merge conflict อย่างแน่นอน แต่การแก้ไข Merge conflict นั้น
ก็ทำได้ง่ายๆมากเลยนะ เพียงแค่เราคุยกันในเรื่องที่ควรจะคุยกันมากขึ้น ต้องรู้และเข้าใจก่อนว่าที่มาที่ไปของปัญหามันคืออะไรกันแน่แล้วแก้ไขด้วยกัน

