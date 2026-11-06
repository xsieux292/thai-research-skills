# Thai Research Skills

Skill สำหรับ Claude Code / Claude สำหรับงานเขียนเชิงวิชาการภาษาไทยและอังกฤษ ได้แก่ งานวิจัย บทความวิชาการ วิทยานิพนธ์ รายงานโครงงาน และข้อเสนอโครงการ

| Skill | หน้าที่ |
|---|---|
| `research-reviewer` | ตรวจงานในบทบาทผู้ทรงคุณวุฒิหรือกรรมการสอบ ออกรายงานข้อค้นพบพร้อมระดับความรุนแรง ตำแหน่ง และข้อเสนอแนะ |
| `researcher` | เกลาและแก้งานเขียนให้เป็นภาษาวิชาการ โดยคงความหมาย ข้อมูล และผลการวิจัยเดิม ไม่เติมตัวเลขหรือข้อสรุปที่ไม่มีในต้นฉบับ |

ใช้คู่กันได้: ให้ `research-reviewer` ตรวจก่อน แล้วให้ `researcher` แก้ตามข้อค้นพบ

## การติดตั้ง

**Claude Code (plugin marketplace)**

```
/plugin marketplace add xsieux292/thai-research-skills
/plugin install thai-research-skills@thai-research-skills
```

**ผ่าน skills CLI**

```bash
npx skills add xsieux292/thai-research-skills
```

**คัดลอกเอง**: คัดลอกโฟลเดอร์ใน `skills/` ไปไว้ที่ `~/.claude/skills/`

## ตัวอย่างการใช้

- "ช่วยตรวจบทที่ 3 ของปริญญานิพนธ์นี้หน่อย" → `research-reviewer`
- "ช่วยเกลาบทนำให้เป็นภาษาวิชาการ" → `researcher`
- "แก้ตามข้อค้นพบ R1–R3 ในรายงานรีวิว" → `researcher`

## โครงสร้าง

```
skills/
  research-reviewer/  SKILL.md, references/checklists.md, evals/
  researcher/         SKILL.md, references/{thai-academic-style,section-guide}.md, evals/
```

โฟลเดอร์ `evals/` เป็นชุดทดสอบ skill ใช้รายงานสมมติ (ระบบแจ้งเตือนสต็อกสินค้า IoT) ไม่มีข้อมูลจริง

## License

MIT
