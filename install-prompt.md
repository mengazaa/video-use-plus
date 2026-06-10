# Video-Use-Plus Install Prompt

Copy ข้อความด้านล่างทั้งหมด แล้ว paste ลงใน Claude Code:

---

ช่วยติดตั้ง Video-Use-Plus skill ให้หน่อยครับ ทำตามขั้นตอนนี้:

1. สร้าง folder ~/.claude/skills/video-use-plus/
2. Download SKILL.md จาก https://raw.githubusercontent.com/mengazaa/video-use-plus/main/SKILL.md แล้ว save ไว้ที่ ~/.claude/skills/video-use-plus/SKILL.md
3. ตรวจสอบ dependencies ที่ต้องการ (node >= 20, python3 >= 3.10, ffmpeg, pnpm, uv, yt-dlp)
4. แสดงสรุปว่าอะไรขาดบ้าง แล้วถามว่าจะติดตั้งไหม
5. ถ้าตกลง ให้ลง dependencies ตามที่ SKILL.md ระบุ
6. สร้าง config file ที่ ~/.video-use-plus/config.json
7. ทดสอบว่า html-video doctor ผ่าน
8. บอกว่าพร้อมใช้งาน พิมพ์ /video-use-plus เพื่อเริ่มสร้างวิดีโอ
