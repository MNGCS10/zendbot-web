zendbot website v1 — ไฟล์พร้อม deploy Cloudflare Pages

ไฟล์:
  index.html  = หน้าแรก (Hub + 3 โซน)
  shelf.html  = มุมของพร้อมใช้ (SHELF)
  rent.html   = ระบบเช่าใช้ (RENT)
  forge.html  = สร้างให้เฉพาะธุรกิจ (FORGE)
  _redirects  = config Cloudflare

วิธี deploy Cloudflare Pages:
  ทางที่ 1 (ลากไฟล์ตรง):
    1. Cloudflare Dashboard > Workers & Pages > Create > Pages > Upload assets
    2. ลากไฟล์ทั้งหมดในโฟลเดอร์นี้ขึ้นไป
    3. Deploy
  ทางที่ 2 (ผ่าน GitHub):
    1. push ไฟล์ขึ้น repo (เช่น zendbot-web)
    2. Pages > Connect to Git > เลือก repo
    3. Build command: (เว้นว่าง), Output dir: /
    4. Deploy

เชื่อม domain:
  Pages project > Custom domains > zendbot.co (domain อยู่ Cloudflare แล้ว = คลิกเดียว)

ก่อน go-live:
  - ใส่ LINE_OA_URL ในทุกไฟล์ (ตัวแปรใน <script> ท้ายไฟล์) เมื่อ setup LINE OA เสร็จ
