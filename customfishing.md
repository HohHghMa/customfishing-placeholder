# 🎣 CustomFishing — คู่มือ PlaceholderAPI & การตั้งค่า

เอกสารรวบรวม Placeholder ทั้งหมดของปลั๊กอิน CustomFishing สำหรับนำไปใช้งานร่วมกับ **PlaceholderAPI (PAPI)** เช่น บน Scoreboard, TAB, Holograms, DeluxeMenus และ Chat Formatting

> **Identifier หลัก:** `ctf`  
> รูปแบบการเรียกใช้งาน: `%ctf_<placeholder>%`  
> หากใส่แล้วไม่แสดงผลหรือขึ้นเป็นข้อความเดิม ให้พิมพ์คำสั่ง: `/papi reload`

---

## 1. 🐟 กิจกรรมปลาหมอคางดำ (Blackchin Event)

หมวดหมู่ Placeholder สำหรับติดตามสถานะกิจกรรมปลาหมอคางดำ

| Placeholder | รายละเอียด / หน้าที่ | ตัวอย่างผลลัพธ์ |
| :--- | :--- | :--- |
| `%ctf_blackchin_status%` | สถานะกิจกรรม (ข้อความธรรมดา) | `กำลังดำเนินกิจกรรม` / `ปิดอยู่` |
| `%ctf_blackchin_status_colored%` | สถานะกิจกรรมพร้อมรหัสสี (`§a` / `§c`) | `§aกำลังดำเนินกิจกรรม` / `§cปิดอยู่` |
| `%ctf_blackchin_active%` | ตรวจสอบว่ากิจกรรมกำลังจัดอยู่หรือไม่ | `true` หรือ `false` |
| `%ctf_blackchin_time%` | เวลาที่เหลือกิจกรรม (รูปแบบ `mm:ss`) | `04:59`, `00:30` |
| `%ctf_blackchin_time_left%` | *เหมือนกับ `%ctf_blackchin_time%`* | `04:59` |
| `%ctf_blackchin_time_seconds%` | เวลาที่เหลือเป็นจำนวนวินาที | `299`, `30` |
| `%ctf_blackchin_seconds_left%` | *เหมือนกับ `%ctf_blackchin_time_seconds%`* | `299` |
| `%ctf_blackchin_duration%` | ระยะเวลากิจกรรมทั้งหมดที่ตั้งไว้ (หน่วยนาที) | `15` |
| `%ctf_blackchin_species%` | ชนิดปลาเป้าหมายของกิจกรรม | `blackchin_tilapia` |
| `%ctf_blackchin_bossbar%` | สถานะการเปิดใช้งาน BossBar ในกิจกรรม | `true` หรือ `false` |
| `%ctf_blackchin_world%` | ชื่อ World ที่จัดกิจกรรม | `world` |
| `%ctf_blackchin_in_region%` | ตรวจสอบว่าตัวผู้เล่นยืนอยู่ในเขตกิจกรรมหรือไม่ | `true` หรือ `false` |

---

## 2. 🎣 สเตตัสเบ็ดตกปลาในมือ (Held Fishing Rod Stats)

ดึงข้อมูลสเตตัสของคันเบ็ดที่ผู้เล่นกำลังถืออยู่ในมือหลัก (Main Hand) แบบ Real-time

| Placeholder | รายละเอียด / หน้าที่ | ตัวอย่างผลลัพธ์ |
| :--- | :--- | :--- |
| `%ctf_rod_plus%` | ระดับการตีบวกของคันเบ็ด | `+0`, `+3`, `+10` |
| `%ctf_rod_damage%` | โบนัสดาเมจตกปลาของคันเบ็ด | `0`, `5.0`, `12.5` |
| `%ctf_rod_hp_bonus%` | โบนัสพลังชีวิตเบ็ด (HP Bonus) | `0`, `10` |
| `%ctf_rod_control%` | ค่าการควบคุมปลา (Rod Control) | `0`, `15` |
| `%ctf_rod_luck%` | ค่าโชคของเบ็ด (Rod Luck) | `0`, `5` |

---

## 3. ⭐ เลเวลและยศตกปลา (Fishing Level & Rank)

ข้อมูลความคืบหน้า EXP, เลเวล, และยศตกปลาของผู้เล่น

| Placeholder | รายละเอียด / หน้าที่ | ตัวอย่างผลลัพธ์ |
| :--- | :--- | :--- |
| `%ctf_level%` | เลเวลตกปลาของผู้เล่น | `12` |
| `%ctf_level_icon%` | ไอคอนเลเวล | `[Lv.12]` |
| `%ctf_rank%` | รหัสยศ / Tier การตกปลา | `novice`, `expert` |
| `%ctf_rank_name%` | ชื่อแสดงยศการตกปลา | `นักตกปลาฝึกหัด` |
| `%ctf_xp%` | EXP ตกปลาของเลเวลปัจจุบัน | `240` |
| `%ctf_required_xp%` | EXP ที่ต้องใช้เพื่อขึ้นเลเวลถัดไป | `1000` |
| `%ctf_xp_to_next%` | EXP ที่ยังขาดอยู่ | `760` |
| `%ctf_total_xp%` | EXP สะสมทั้งหมดของผู้เล่น | `5320` |
| `%ctf_progress_percent%` | เปอร์เซ็นต์ความคืบหน้าเลเวล (%) | `24.0%` |

---

## 4. 🐉 เวิลด์บอสตกปลา (World Boss Fishing)

ข้อมูลบอสตกปลาโลก และสถิติการต่อสู้ของผู้เล่น

| Placeholder | รายละเอียด / หน้าที่ | ตัวอย่างผลลัพธ์ |
| :--- | :--- | :--- |
| `%ctf_worldboss_active%` | มีบอสตกปลาเกิดอยู่หรือไม่ | `true` หรือ `false` |
| `%ctf_worldboss_phase%` | เฟสของบอส (ตัวเลข) | `1`, `2` |
| `%ctf_worldboss_phase_name%` | ชื่อเฟสของบอส | `Phase 1` |
| `%ctf_worldboss_hp%` | เลือดปัจจุบันของบอส | `3500` |
| `%ctf_worldboss_maxhp%` | เลือดสูงสุดของบอส | `10000` |
| `%ctf_worldboss_hp_percent%` | เปอร์เซ็นต์เลือดบอส | `35.0%` |
| `%ctf_worldboss_time_left%` | เวลาที่เหลือของบอส (รูปแบบ `mm:ss`) | `08:45` |
| `%ctf_worldboss_time_left_seconds%` | เวลาที่เหลือของบอส (วินาที) | `525` |
| `%ctf_worldboss_participants%` | จำนวนผู้เล่นที่เข้าร่วมสู้บอส | `8` |
| `%ctf_worldboss_my_damage%` | ดาเมจที่ตัวเราทำต่อบอส | `1250` |
| `%ctf_worldboss_my_catches%` | จำนวนครั้งที่ตัวเราตก/ดึงบอสสำเร็จ | `14` |
| `%ctf_worldboss_my_rank%` | อันดับดาเมจของตัวเรา | `2` |
| `%ctf_worldboss_top_name_<1-10>%` | ชื่อผู้เล่นท็อปดาเมจอันดับ 1-10 | `%ctf_worldboss_top_name_1%` |
| `%ctf_worldboss_top_damage_<1-10>%` | ดาเมจของผู้เล่นอันดับ 1-10 | `%ctf_worldboss_top_damage_1%` |
| `%ctf_worldboss_top_catches_<1-10>%` | จำนวนครั้งตกของผู้เล่นอันดับ 1-10 | `%ctf_worldboss_top_catches_1%` |

---

## 5. 🏆 อันดับกิจกรรมการแข่งขัน (Competition Leaderboards)

| Placeholder | รายละเอียด / หน้าที่ | ตัวอย่างผลลัพธ์ |
| :--- | :--- | :--- |
| `%ctf_topeventname_fish_<1-10>%` | ชื่อผู้เล่นที่ตกปลาได้มากที่สุดอันดับ 1-10 | `%ctf_topeventname_fish_1%` |
| `%ctf_topevent_fish_<1-10>%` | จำนวนปลาที่ตกได้ของอันดับ 1-10 | `%ctf_topevent_fish_1%` |
| `%ctf_topeventname_monster_<1-10>%` | ชื่อผู้เล่นที่ตกมอนสเตอร์ได้มากที่สุดอันดับ 1-10 | `%ctf_topeventname_monster_1%` |
| `%ctf_topevent_monster_<1-10>%` | จำนวนมอนสเตอร์ที่ตกได้ของอันดับ 1-10 | `%ctf_topevent_monster_1%` |

---

## 6. ⚙️ แท็กที่ใช้ในไฟล์คอนฟิก (Internal Config Placeholders)

แท็กสำหรับนำไปตกแต่งข้อความในไฟล์ `blackchin_event.yml`:

| Tag | คำอธิบาย | ตัวอย่าง |
| :--- | :--- | :--- |
| `{duration}` | ระยะเวลากิจกรรมทั้งหมดเป็นนาที | `15` |
| `{minutes}` | จำนวนนาทีที่เหลือ | `5` |
| `{seconds}` | จำนวนวินาทีที่เหลือ | `30` |
| `{time}` | เวลาที่เหลือในรูปแบบ `mm:ss` | `05:00`, `00:30` |

---

## 7. 💡 ตัวอย่างการนำไปใช้งาน (Examples)

### ตัวอย่าง: ใส่ใน Scoreboard
```yaml
Lines:
  - "&e&l[ กิจกรรมปลาหมอคางดำ ]"
  - "&7สถานะ: %ctf_blackchin_status_colored%"
  - "&7เวลาที่เหลือ: &f%ctf_blackchin_time%"
  - "&7อยู่ในพื้นที่: &a%ctf_blackchin_in_region%"
  - ""
  - "&a&l[ สเตตัสเบ็ด ]"
  - "&7ระดับ: &e%ctf_rod_plus%"
  - "&7ดาเมจ: &c+%ctf_rod_damage%"
  - "&7โชค: &b+%ctf_rod_luck%"
```

### ตัวอย่าง: ใส่ใน TAB / NameTag
```yaml
header:
  - "&bตกปลาเลเวล: &e%ctf_level% &7(&f%ctf_progress_percent%&7)"
  - "&6กิจกรรมปลาหมอ: %ctf_blackchin_status_colored% &7(&f%ctf_blackchin_time%&7)"
```

---

## 8. 👑 คำสั่งจัดการเลเวลสำหรับ Admin (Level Admin Commands)

รองรับการใช้งานทั้งในเกม (Player) และคอนโซลเซิร์ฟเวอร์ (Console / RCON / Web Store):

| คำสั่ง | สิทธิ์ (Permission) | คำอธิบาย | ตัวอย่างการใช้งาน |
| :--- | :--- | :--- | :--- |
| `/ctf level info [ผู้เล่น]` | ทุกคน / Admin | ดูเลเวล, ยศ, EXP ปัจจุบัน, และ % ความคืบหน้า | `/ctf level info Steve` |
| `/ctf level set <ผู้เล่น> <เลเวล>` | `customfishing.admin` | กำหนดเลเวลตกปลาของผู้เล่นโดยตรง | `/ctf level set Steve 10` |
| `/ctf level add <ผู้เล่น> <จำนวน>` | `customfishing.admin` | เพิ่มเลเวลตกปลาให้ผู้เล่น | `/ctf level add Steve 2` |
| `/ctf level remove <ผู้เล่น> <จำนวน>` | `customfishing.admin` | ลดเลเวลตกปลาของผู้เล่น | `/ctf level remove Steve 1` |
| `/ctf level setxp <ผู้เล่น> <EXP>` | `customfishing.admin` | กำหนดค่า EXP ของเลเวลปัจจุบัน | `/ctf level setxp Steve 500` |
| `/ctf level addxp <ผู้เล่น> <EXP>` | `customfishing.admin` | เพิ่ม EXP (หากครบจะ Level Up อัตโนมัติ) | `/ctf level addxp Steve 250` |
| `/ctf level removexp <ผู้เล่น> <EXP>` | `customfishing.admin` | ลด EXP (หากติดลบจะ De-level ลงอัตโนมัติ) | `/ctf level removexp Steve 100` |
| `/ctf level reset <ผู้เล่น>` | `customfishing.admin` | รีเซ็ตเลเวลและ EXP กลับเป็น 1 (0 XP) | `/ctf level reset Steve` |

---

## 9. 🌐 ระบบภาษาและการปรับแต่งข้อความ (`locale.yml`)

ปลั๊กอิน CustomFishing ได้รับการอัปเกรดระบบข้อความเป็น **Modular Localization System** เต็มรูปแบบ โดยจัดเก็บข้อความทั้งหมดไว้ที่ไฟล์:
📁 `plugins/CustomFishing/locale.yml`

> 💡 **การอัปเกรดอัตโนมัติ (Seamless Migration):**  
> หากเซิร์ฟเวอร์ของคุณมีไฟล์ `msg.yml` เดิมอยู่แล้ว ปลั๊กอินจะดึงข้อมูลข้อความภาษาไทยเดิมทั้งหมดมาใส่ใน `locale.yml` อัตโนมัติ พร้อมทั้งเสริมคีย์คำสั่งใหม่ (Admin commands, Level, Rod, WorldBoss, Area) ให้ครบ 100% โดยไม่ต้องพิมพ์ใหม่เลยแม้แต่จุดเดียว!

### หมวดหมู่ข้อความใน `locale.yml`:

| หมวดหมู่ (Category) | คีย์หลัก | คำอธิบายสิ่งที่ปรับแต่งได้ |
| :--- | :--- | :--- |
| **Admin & Commands** | `command.*` | ข้อความแจ้งเตือนคำสั่ง reload, ไม่มีสิทธิ์, เริ่ม merge config, ล้าง Display Entity |
| **ระบบเลเวล** | `level.*` | ข้อความคำสั่ง `/ctf level`, เพิ่ม/ลด/รีเซ็ตเลเวล, แจ้งเตือนผู้เล่นเมื่อถูกเปลี่ยนเลเวล |
| **สเตตัสและคันเบ็ด** | `rod.*` | ข้อความคำสั่ง `/ctf rod`, การ enchant/setstat, แจ้งเตือนให้ถือคันเบ็ด |
| **กิจกรรมปลาหมอคางดำ** | `blackchin.*` | คำสั่งเริ่ม/หยุดกิจกรรม, ตั้งจุด Pos1-2, สลับเปิด/ปิด Bossbar, ดูสถานะ Help |
| **เวิลด์บอสตกปลา** | `boss.*` | คำสั่งเสกบอส, สั่งเริ่ม/หยุด, ดูสเตตัสเลือดและเวลาบอส |
| **โซนตกปลา & เลเวลขั้นต่ำ** | `area.*` | คำสั่ง `/ctf setarea`, `/ctf createarea`, ข้อความ Action Bar เตือนเมื่อเลเวลไม่ถึง |
| **มินิเกมตกปลา** | `minigame.*` | หลอด Action Bar, แรงดึงสายเบ็ด (Tension), ทิศทางเอียง (Tilt), ข้อความตอนตกติดหรือหลุด |
| **ระดับความหายาก** | `rarities.*` | ชื่อและรหัสสีของปลาแต่ละเกรด (Common, Uncommon, Rare, Epic, Legendary, Mythic, Exotic) |
| **เมนู GUI ทั้งหมด** | `gui.*` | เมนูหลัก, หน้ารวมปลา (Collection), ตีบวกเบ็ด (Upgrade), จุดตกของรางวัล (ItemSpot) |
| **การแข่งขันตกปลา** | `event.*` | ข้อความ Broadcast แจ้งเตือนรอบแข่งปลา/มอนสเตอร์, นับถอยหลัง, และสรุปผลท็อปอันดับ |
| **จุดตกของรางวัล** | `itemspot.*` | ข้อความประกาศเมื่อจุดของรางวัลเกิด และเตือนเมื่อใกล้หมดเวลา |
| **โฮโลแกรมบอร์ด** | `holograms.*` | หัวตารางและรูปแบบบรรทัดแสดงผลบนโฮโลแกรม Leaderboard |

### วิธีแก้ไขและอัปเดตภาษาในเกม:
1. เปิดไฟล์ `plugins/CustomFishing/locale.yml` ด้วย Text Editor
2. แก้ไขข้อความ สี Hex (`&#rrggbb`), ตัวหนา (`&l`), หรือ Emoji ได้ตามต้องการ
3. บันทึกไฟล์ และพิมพ์คำสั่งในเซิร์ฟเวอร์:
   ```bash
   /ctf reload
   ```
   *ข้อความทั้งหมดในเซิร์ฟเวอร์จะอัปเดตเป็นภาษาใหม่ทันทีโดยไม่ต้องรีสตาร์ตเซิร์ฟเวอร์!*


