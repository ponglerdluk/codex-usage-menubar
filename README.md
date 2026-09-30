# Codex Usage Menu Bar

แอพแสดงโควตา Codex ที่เหลือใน Menu Bar: หัวข้อ 5H / WEEK อยู่เหนือเปอร์เซ็นต์ ไม่มีกราฟ ตัวเล็กและระยะห่างกระชับ ไม่แสดงใน Dock อัปเดตทุก 3 นาทีและหลังตื่นจาก Sleep ชี้เมาส์ดูเวลา Reset และคลิกเปิดเมนู Refresh / เลือก Codex / Privacy / Quit

รองรับ **Apple Silicon (arm64) เท่านั้น**, macOS **13 Ventura ขึ้นไป** ไม่รองรับ Intel โควตานี้เป็นของ Codex ไม่ใช่ทุกโมเดลใน ChatGPT และขึ้นกับสิทธิ์บัญชีของผู้ใช้

## ดาวน์โหลดไฟล์ไหน

สำหรับ Mac ชิป Apple Silicon (M1 ขึ้นไป) และ macOS 13 Ventura ขึ้นไป ให้โหลด **Codex-Usage-arm64.dmg** จาก [ลิงก์ดาวน์โหลดรุ่นล่าสุด](https://github.com/ponglerdluk/codex-usage-menubar/releases/latest/download/Codex-Usage-arm64.dmg)

บนหน้า Releases ให้เปิดหัวข้อ Assets แล้วคลิกชื่อไฟล์นี้ ไม่ต้องโหลด Source code, appcast.xml หรือ ZIP สำหรับการติดตั้งทั่วไป ไฟล์ ZIP เป็นตัวเลือกสำหรับคนที่ต้องการแตกไฟล์เอง

## ติดตั้งทีละขั้น

1. รอดาวน์โหลดเสร็จ แล้วเปิด Finder → Downloads (รายการดาวน์โหลด) หรือคลิกไฟล์ในรายการดาวน์โหลดของเบราว์เซอร์
2. ดับเบิ้ลคลิก **Codex-Usage-arm64.dmg** เพื่อเปิดดิสก์ติดตั้ง
3. ในหน้าต่างดิสก์ติดตั้ง ลาก **Codex Usage.app** ไปที่โฟลเดอร์ **Applications** หาก macOS ขออนุญาตคัดลอก ให้ยืนยันด้วยบัญชีผู้ดูแลระบบ หากมีรุ่นเก่า ให้ปิดเฉพาะ Codex Usage ผ่านเมนู Quit แล้วเลือก Replace เพื่อแทนรุ่นเก่า ไม่ต้องปิด ChatGPT/Codex หลัก
4. เปิด Finder → Applications แล้วดับเบิ้ลคลิก **Codex Usage** จากตำแหน่งนี้ อย่าใช้งานแอพจากดิสก์ติดตั้งโดยตรง
5. เมื่อเปิดสำเร็จจะเห็น **5H / WEEK** และเปอร์เซ็นต์ที่ Menu Bar ด้านบน แอพนี้ไม่มีหน้าต่างหลักและไม่แสดงไอคอนใน Dock
6. กลับไป Finder กดปุ่ม Eject ข้างดิสก์ Codex Usage หลังคัดลอกเสร็จแล้ว สามารถลบไฟล์ DMG ใน Downloads ได้ โดยตัวแอพยังอยู่ใน Applications

## ถ้าดับเบิ้ลคลิกแล้ว macOS บล็อก

รุ่นนี้ sign แบบ **ad-hoc** และ **ยังไม่ได้ notarize** จึงอาจขึ้นว่า Apple ไม่สามารถตรวจสอบแอพ หรือไม่สามารถยืนยันผู้พัฒนาได้ ให้ทำขั้นตอนต่อไปนี้เฉพาะเมื่อดาวน์โหลดจาก GitHub ของ ponglerdluk และเชื่อถือไฟล์นี้

1. ในกล่องคำเตือน เลือก **Done / OK / Cancel** ตามปุ่มที่มี อย่าเลือก Move to Trash หากต้องการติดตั้งต่อ
2. คลิกเมนู Apple  มุมซ้ายบน → **System Settings (การตั้งค่าระบบ)**
3. เลือก **Privacy & Security (ความเป็นส่วนตัวและความปลอดภัย)** แล้วเลื่อนลงไปที่ส่วน Security
4. หาข้อความว่า **Codex Usage** ถูกบล็อก แล้วคลิก **Open Anyway (เปิดต่อไป)**
5. หากระบบถาม ให้ยืนยันด้วย Touch ID หรือรหัสผ่านบัญชี Mac ของตัวเอง แล้วกด **Open** ในกล่องยืนยัน
6. ตรวจ Menu Bar ด้านบนอีกครั้ง ครั้งต่อไปเปิดจาก Applications ตามปกติได้

ถ้าไม่พบ Open Anyway ให้ลองเปิด Codex Usage จาก Applications อีกครั้ง แล้วกลับมาหน้า Privacy & Security ทันที ตัวเลือกนี้แสดงหลังจากพยายามเปิดแอพ หากเครื่องขององค์กรไม่อนุญาตให้เปิด ให้ติดต่อผู้ดูแลเครื่อง

หากคำเตือนระบุว่าพบมัลแวร์หรือแอพจะทำให้เครื่องเสียหาย ให้หยุดและแจ้งผู้แจก หากระบุว่าไฟล์เสียหาย ให้ดาวน์โหลดใหม่และตรวจ SHA-256 ก่อน ไม่ใช้วิธีลบ quarantine หรือปิด Gatekeeper ทั้งระบบ

อ้างอิง: [คำแนะนำ Apple สำหรับแอพที่ไม่ผ่านการยืนยัน](https://support.apple.com/en-gb/102445)

## เตรียม Codex และบัญชีของตัวเอง

Codex Usage เป็นตัวแสดงโควตา ไม่ได้รวม Codex หรือบัญชีของผู้แจก ทุกคนต้องติดตั้ง Codex ของ OpenAI และลงชื่อเข้าใช้ **บัญชี ChatGPT ของตัวเอง** ก่อน

- หากติดตั้งแอพ Codex/ChatGPT ที่มี Codex CLI อยู่แล้ว ให้เปิดแอพนั้นและลงชื่อเข้าใช้ จากนั้นเปิด Codex Usage
- หากยังไม่มี Codex CLI ให้ติดตั้งตาม [เอกสารทางการ](https://learn.chatgpt.com/docs/codex/cli) แล้วรัน `codex login` ใน Terminal เพื่อทำขั้นตอนลงชื่อเข้าใช้ ไม่ต้องส่งรหัสผ่านหรือ API key ให้ผู้แจก
- หาก Menu Bar แสดง `--` ให้คลิกเพื่ออ่านข้อความผิดพลาด หากขึ้น Codex not found ให้เลือก **Choose Codex executable…** แล้วเลือกแอพ Codex/ChatGPT ใน Applications ที่มี Codex CLI หรือเลือก executable `codex` ที่ติดตั้งไว้ สำหรับ CLI ใช้ `command -v codex` ใน Terminal เพื่อหาไฟล์ แล้วกด Command+Shift+G ในหน้าต่างเลือกไฟล์เพื่อใส่ตำแหน่งนั้น
- หลังลงชื่อเข้าใช้หรือเลือกตำแหน่งแล้ว คลิก Menu Bar → **Refresh**

## ให้เปิดเองทุกครั้งที่ล็อกอิน Mac

แอพยังไม่มีสวิตช์ Launch at Login ในเมนู ให้ตั้งผ่าน macOS หลังติดตั้งใน Applications และเปิดครั้งแรกได้สำเร็จแล้ว

1. คลิก Apple  → **System Settings** → **General (ทั่วไป)**
2. เลือก **Login Items & Extensions** หรือ **Login Items** ตามรุ่น macOS
3. ในหัวข้อ **Open at Login (เปิดเมื่อล็อกอิน)** คลิกปุ่ม **+**
4. เลือก **Applications → Codex Usage.app** แล้วคลิก **Open / Add**
5. ตรวจว่ามี **Codex Usage** อยู่ในรายการ Open at Login ครั้งต่อไปเมื่อเข้าสู่บัญชี Mac แอพจะเปิดที่ Menu Bar เอง

ถ้าจะยกเลิก ให้กลับมาหน้าเดียวกัน เลือก Codex Usage แล้วกด **−** ไม่ต้องเปลี่ยนการล็อกอินอัตโนมัติของบัญชี Mac และไม่ต้องเพิ่มแอพจาก Downloads หรือดิสก์ DMG

อ้างอิง: [คำแนะนำ Apple เรื่องเปิดแอพตอนล็อกอิน](https://support.apple.com/en-au/guide/mac-help/-mh15189/mac)

ตรวจไฟล์ ZIP ใน Terminal จากโฟลเดอร์ที่เก็บ ZIP และไฟล์ SHA256SUMS.txt:

```sh
shasum -a 256 -c SHA256SUMS.txt
```

แพ็กเกจไม่มี credentials, ข้อมูลบัญชี, logs หรือไฟล์ส่วนตัว ไม่รวม Codex CLI; ทุกคนต้องติดตั้งและลงชื่อเข้าใช้เอง ตัว utility ไม่อ่านไฟล์ credential โดยตรง Codex จัดการ authentication และติดต่อ OpenAI เอง utility เก็บเฉพาะ path executable ที่เลือกใน UserDefaults ของผู้ใช้

## ซอร์สและการทดสอบ

ใช้ Apple Silicon และ Swift 5.9+ เพื่อ build: `bash build.sh` สร้าง Release arm64 และ sign แบบ ad-hoc
`bash test-core.sh` รันทดสอบ UsageCore เดิมทั้ง 3 กรณีด้วย standalone assertion runner ไม่ต้องมี XCTest; หากติดตั้ง Xcode เต็ม สามารถรัน `swift test --arch arm64` ได้ด้วย

รุ่นแจกนี้ build และทดสอบบน Apple Silicon แล้ว ตรวจ architecture, ลายเซ็น และแตก ZIP ทดสอบสิทธิ์ executable แล้ว แต่เครื่องมีเฉพาะ Command Line Tools จึงรัน XCTest ไม่ได้ ใช้ standalone runner แทน ยังไม่ได้ทดสอบบนเครื่องเพื่อน, macOS 13 จริง, การเปิดไฟล์ที่ติด quarantine หลังดาวน์โหลด หรือหน้าตาจริงใน Light/Dark Mode ทุกสภาพแวดล้อม

ซอร์สโค้ดใช้ MIT LICENSE; โลโก้ที่ผู้จัดทำส่งมาเป็นทรัพย์สินของเจ้าของสิทธิ์เดิมและไม่อยู่ภายใต้ MIT แอพนี้เป็น utility ส่วนตัว ไม่ใช่แอพทางการของ OpenAI

## อัปเดตในแอพ (ตั้งแต่ 1.1.0)

คลิก Menu Bar → Check for Updates… แล้วเลือกดาวน์โหลดและติดตั้ง แอพใช้ Sparkle 2.10.0 ตรวจลายเซ็น Ed25519 ก่อนแตกไฟล์และติดตั้ง อัปเดตผ่าน GitHub Releases แบบ Public ไม่ต้องลงชื่อเข้าใช้ GitHub ไม่มีการตรวจหรือดาวน์โหลดอัตโนมัติ

รุ่นเก่าที่ไม่มีเมนูนี้ต้องติดตั้ง 1.1.0 ด้วยตนเองหนึ่งครั้ง รุ่นนี้ยังใช้ ad-hoc signing และยังไม่ได้ notarize ตามคำเตือนด้านบน Sparkle ใช้สิทธิ์เขียน Applications หรืออาจขอรหัสผ่านผู้ดูแลระบบตามสิทธิ์เครื่อง

Sparkle ใช้ใบอนุญาตของตัวเอง ดู Vendor/Sparkle-LICENSE (รวมไว้ในแอพที่แจกด้วย)
