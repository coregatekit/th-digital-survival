# th-digital-survival 🇹🇭🇹🇭🇹🇭

โปรเจ็กต์นี้มุ่งที่จะรวมคู่มือ/แนวทางปฏิบัติในกรณีที่มีกลุ่มคนที่ต้องการสื่อ และรับรู้ข่าวสารด้วยวิธีที่ปลอดภัยจากภัยคุกคามต่างๆ รวมถึงการคุกคามโดยกลุ่มมาเฟีย อันธพาล หรือเจ้าหน้าที่รัฐที่ปฏิบัติหน้าที่นอกขอบเขตที่กฎหมายอนุญาต และดำเนินงานที่ไม่สอดคล้องกับปฏิญญาสากลว่าด้วยสิทธิมนุษยชน (ที่ประเทศไทยได้ลงนาม)

ในเมื่อหน้าต่าง ประตูในบ้าน ไม่ได้มีไว้เพื่อให้ทำสิ่งที่ผิดกฎหมาย ทางเราเชื่อว่าการใช้อุปกรณ์ดิจิทัลทั้งหลายควรได้รับการป้องกันเสมือนหน้าต่าง ประตู ด้วยเช่นเดียวกัน

*สิ่งที่โปรเจกต์จะไม่ทำคือชี้วิธีการในการฝ่าฝืนกฎหมาย อำนาจศาล หรืออำนาจชอบธรรมของเจ้าหน้าที่รัฐในการทำงาน*

## แนวทาง

การพัฒนาข้อมูลชุดนี้จะเกิดขึ้นในที่เปิดเผย ผ่าน Github แฃะการสื่อสารหลักๆสำหรับเฟสแรกจะเกิดขึ้นผ่าน Issues tracker กับแอพ Telegram (โหลดแล้วคลิกลิ้งค์ได้เลย https://t.me/joinchat/AgGs0ho9O29vjYsB0WvFig) ใครๆก็สามารถเข้ามามีส่วนร่วมเป็นอาสาสมัครและเสนอความคิดเห็นได้ ถึงแม้ว่าคุณสนใจแต่ไม่มีประสบการณ์และคิดว่าฝีมือไม่ถึง ไม่เป็นไรครับ เรายินดีต้อนรับการเข้ามามีส่วนร่วมของคุณ

## โปรเจกต์ต้องการอาสาสมัครดังนี้

* ผู้เชี่ยวชาญทางด้าน infosec
* นักเขียนสำหรับคู่มือ
* นักแปลสำหรับ คู่มือ แอพ บทความต่าง จากภาษาอังกฤษเป็นภาษาไทย
* คนทำกราฟฟิก อัดวีดีโอ ทำ voiceover เพื่อให้เข้าใจง่าย
* คนที่จะช่วยทดสอบและยืนยันความถูกต้องของคู่มือ
* คนที่ช่วยด้านการประชาสัมพันธ์

## ข้อมูลเบื้องต้น

![xkcd-crypto-th](https://user-images.githubusercontent.com/3682634/75450354-39a5df00-59a1-11ea-8c72-59ec66ec6133.png)\
ที่มา: [xkcd: Security](https://www.xkcd.com/538/)

ภาพแรก เราจะเห็นว่าในจินตนาการของนักต่อสู้ ผู้ร้ายสองคนกำลังคุยกัน เขาได้จับตัวประกันมาและจะถอดรหัสที่ปกป้องแลปทอปของตัวประกัน แต่ทำไม่ได้เพราะใช้รหัสแบบ 4096 บิท ตัวประกันปลอดภัย ภาพสอง เอาเข้าจริงๆถ้าเจอแลปทอปที่ลงรหัสไว้ ผู้ร้ายจะเอาประแจมาทุบหัวจนกว่าตัวประกันจะเปิดเผยรหัสผ่าน

อย่าลืมนะครับว่าถ้าคุณหรือเพื่อนๆ กำลังจะเผชิญกับคนที่ยินดีที่จะใช้ความรุนแรง คุณต้องตัดสินใจเอาเองว่าสิ่งที่คุณกำลังจะทำอยู่นั้น คุ้มกับการเจ็บตัวหรือไม่

### ไอพี (IP Address)

คอมพิวเตอร์ทุกเครื่องในอินเตอร์เน็ตจะมีที่อยู่ไอพี (IP Address) ที่ใช้ในการรับส่งข้อมูล อยากให้ทุกคนลองเข้าไปดูที่  https://whatismyipaddress.com/ เห็นตัวเลข IPV6 กับ IPV4 ไหมครับ เช่น IPv6: 2345:1234:bc81:3a0f:74be:fbbd:8c35:4821 IPv4: 184.22.234.55 ลองเปิดหน้านี้จากอุปกรณ์หลายตัวกับการเชื่อมต่อหลายประเภทดูครับ (เช่น wifi หรือ 4g ฯลฯ) แล้วคุณจะเห็นที่อยู่ของตัวเองในอินเตอร์เน็ต ส่วนอีฝั่งนึง ถ้าเข้าไปที่ https://www.dnslookup.com แล้วใส่ www.google.com เข้าไป ก็จะเห็นไอพีของปลายทางเหมือนกัน เวลาคอมพิวเตอร์ของเรากับคอมพิวเตอร์ปลายทางสื่อสารกัน ก็จะใช้ไอพีในการสื่อสาร

ทีนี้หนึ่งในปัญหาที่เจอคือผู้ให้บริการอินเตอร์เน็ตทั้งหลาย รวมถึงร้านกาแฟ องค์กร สถาบัน ฯลฯ จะมีการเก็บข้อมูลว่าไอพีไหน ใครใช้ เมื่อไหร่ แม้กระทั่งในอีเมลก็จะมีไอพีพ่วงอยู่ ฉะนั้นสิ่งที่เกิดขึ้นก็คือถ้าคุณได้รับข้อความเข้ามาในกลุ่มไลน์ แล้วข้อความนั้นมีลิ้งค์พ่วงอยู่ ถ้าคุณคลิ๊กลิ้งค์เข้าไป เจ้าของเว็บไซท์ก็จะรู้ว่ามีใครจากไอพีอะไร เข้ามาทำธุรกรรม หรือเข้าไปอ่านหน้าอะไรกันแน่
