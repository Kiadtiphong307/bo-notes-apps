# Project Requirement Document (PRD)

## Project Name
BoNotesApps

## Problem
ผู้ใช้หลายคนมีความต้องการจดบันทึกรายละเอียดรายวัน เช่น งานที่ต้องทำ, ไอเดีย, เป้าหมาย หรือเหตุการณ์สำคัญ
แต่ไม่มีระบบที่ช่วยจัดระเบียบและเตือนให้กลับมาดูในเวลาที่เหมาะสม ทำให้เกิด “การลืม” หรือ “ละเลย” สิ่งที่จดไว้
BoNotesApps จะเป็นตัวช่วยบันทึกพร้อมระบบแจ้งเตือน เพื่อสนับสนุน productivity และ goal tracking ของผู้ใช้ คล้ายๆ 
mini-game เป็ดจดบันทึกประจำวัน
## Users
-บุคคลทั่วไป	        คนที่ต้องการจดบันทึกไอเดีย, งาน, เป้าหมายรายวัน
-นักเรียน / นักศึกษา	 ใช้เพื่อ track การเรียน, บันทึกงาน, สรุปบทเรียน
-คนทำงาน	         สำหรับการวางแผนงาน, ประชุม, To-Do
-ผู้ฝึกตนเอง	        ใช้ติดตามพฤติกรรม เช่น อ่านหนังสือ, ลดน้ำหนัก, ฝึกภาษา ฯลฯฯ
## Core Features
-บันทึกโน้ต พร้อมรายละเอียด เช่น หัวข้อ, เนื้อหา, วันที่
-จัดหมวดหมู่โน้ต เช่น งาน, เป้าหมาย, ส่วนตัว
-ระบบแจ้งเตือน (Reminders) เพื่อเตือนโน้ตตามเวลาที่กำหนด
-ค้นหาโน้ตย้อนหลัง ตาม keyword หรือหมวดหมู่
-Daily/Weekly Goals ระบบจดเป้าหมาย และ track ความสำเร็จ
-(Optional) Sync/Backup กับ cloud หรือ local storage
## Success Criteria
-ผู้ใช้สามารถสร้าง จัดการ และค้นหาโน้ตได้อย่างราบรื่น
-ผู้ใช้ได้รับการแจ้งเตือนตามเวลาที่ตั้งไว้
-ผู้ใช้มี Engagement กลับมาใช้ซ้ำ (เช่น 3 วัน/สัปดาห์ขึ้นไป)
-ระบบมี UX/UI ที่เข้าใจง่าย ใช้งานได้แม้ไม่เคยใช้แอปจดโน้ตมาก่อน
-ข้อมูลไม่สูญหาย (มีระบบสำรองหรือ export)
## Project Structure 
vibe-bo-notes-apps/
├── frontend/               
│   ├── pages/
│   ├── components/
│   └── composables/
├── backend/                
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   └── main.go
├── database/               
├── mobile/                 
├── public/                 
├── docs/                   
├── docker-compose.yml
└── .env
## Packages/Tech Stack
-Frontend	Nuxt version 3
-styling    Tailwind CSS version 3.17
-Backend	Go (Fiber) version 2.0
-Database	MySQL	version 8.0
-Notification Fibase
-Vesion control Git
-localStorage API   
## Milestones / Tasks
-วิเคราะห์ & ออกแบบ UI/UX	Wireframe, Flow, Moodboard
-Setup Project	Init Repo, Docker, CI/CD	
-พัฒนา Core Function: Note + Reminder	CRUD Notes, Set Reminder	
-ระบบเป้าหมาย Daily/Weekly	Tracker UI, Logic, Animation	
-ระบบแจ้งเตือนแบบ real-time หรือ push	Firebase Cloud Messaging	
-(Optional) Cloud Sync และ Export/Import Notes	Supabase / Firebase Store
-Testing & QA	Unit + E2E Tests	
-Deploy & Launch	Live Preview + Feedback Loop	
## References
-Google Keep 
-Notion 
-Todoist 
-Duolingo 
-RealWorld Example App 
