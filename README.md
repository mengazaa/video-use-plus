# Video-Use-Plus

AI Video Editor + Motion Graphic Designer สำหรับ Claude Code

สร้างวิดีโอแบบมืออาชีพ — ตัดต่อ + Motion Graphic อัตโนมัติ ไม่ต้องมีประสบการณ์ตัดต่อวิดีโอ

## ทำอะไรได้?

| Mode | Input | Output |
|------|-------|--------|
| **A** | URL / หัวข้อ / YouTube / GitHub | วิดีโอ explainer สวยๆ จาก content |
| **B** | คลิปจากกล้อง / screen recording | วิดีโอที่ตัดแล้ว (ตัด dead air, ปรับเสียง, ใส่ subtitle) |
| **B+** | Multicam + ไมค์แยก + Podcast | Sync หลายกล้อง + สลับ angle อัตโนมัติ + mix เสียง |
| **C** | คลิป + เนื้อหาเพิ่ม | คลิปที่ตัดแล้ว + title card + สถิติ + motion graphic (โปร่งใส) |

## วิธีติดตั้ง

### วิธีที่ 1: ลาก folder (ง่ายสุด)

1. Download zip แล้ว unzip
2. ลาก folder `video-use-plus` ไปใส่ `~/.claude/skills/`
3. เปิด Claude Code → พิมพ์ `/video-use-plus`
4. ครั้งแรก Claude จะถามก่อนติดตั้ง dependencies (~5 นาที)
5. พร้อมใช้งาน!

### วิธีที่ 2: ใช้ install prompt

1. เปิดไฟล์ `install-prompt.md` ใน zip
2. Copy ข้อความทั้งหมด
3. Paste ใน Claude Code
4. Claude จะทำทุกอย่างให้

## วิธีใช้

พิมพ์ใน Claude Code:

```
# สร้างวิดีโอจาก URL
ทำวิดีโอจากบทความนี้ https://example.com/article

# สร้างวิดีโอจากหัวข้อ
make a video about AI agents for FB

# ตัดต่อคลิป
ตัดต่อคลิปนี้ให้สวย ~/Movies/recording.mp4

# คลิป + motion graphic (lower-third โปร่งใส ทับบนคลิป)
edit ~/Movies/interview.mp4 and add title card and stats overlay

# Multicam + ไมค์แยก
ตัดต่อ podcast — 2 คน 3 กล้อง 2 ไมค์ ~/Movies/podcast-raw/

# Sync เสียงไมค์กับคลิป
sync ~/Movies/cam.mp4 with ~/Movies/mic.wav
```

## Requirements

- macOS (Windows: planned for v2)
- Claude Code
- ครั้งแรก Claude จะลง dependencies ให้อัตโนมัติ:
  - FFmpeg, Node.js >= 22, Python >= 3.10
  - HyperFrames (HeyGen) — สร้าง motion graphics (custom, auto-install via npx)
  - video-use (browser-use) — ตัดต่อวิดีโอ

## Credits

- [HyperFrames](https://github.com/heygen-com/hyperframes) — Apache-2.0
- [video-use](https://github.com/browser-use/video-use) — MIT

## License

MIT
