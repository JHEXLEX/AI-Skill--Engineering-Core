# 🤖 Mechatronic & Unreal Engine Custom Skill for Claude

A specialized, context-aware Custom Skill set for **Claude**, designed to assist in **Mechatronics Engineering** calculations and **Unreal Engine 5** game development workflows. 

---

## 🇹🇷 Türkçe Özet / About

Bu depo, **Claude** için özel olarak hazırlanmış; **Mekatronik Mühendisliği** hesaplamaları ve **Unreal Engine 5** oyun geliştirme süreçlerinde size rehberlik eden modüler bir **Custom Skill (Özel Yetenek)** setidir.

### 💡 Öne Çıkan Özellikler ve Yapı
* **Modüler Mimari:**
  * **`SKILL.md`:** Ana kuralları ve orkestrasyon mantığını içerir.
  * **10 Referans Dosyası:** Oyun/UE5 geliştirme (2 dosya), Mekatronik Mühendisliği hesaplama ve prensipleri (6 dosya) ve Genel/Kategori-bağımsız standartlar (2 dosya).
* **Akıllı Tetiklenme:**
  * Claude'a *"Bir proje geliştiriyorum"* veya *"Yeni bir UE5 projesine başlıyorum"* gibi net bir niyet belirttiğinizde otomatik olarak devreye girer.
* **Oturum Kalıcılığı (Session Persistence):**
  * Bir kez tetiklendikten sonra, aynı sohbet penceresi boyunca tekrar komut vermenize gerek kalmadan aktif kalmaya ve kaldığı yerden devam etmeye devam eder.
* **Dil:** Tüm yetenek talimatları ve referans dokümanları **Türkçe** olarak kalibre edilmiştir.

---

## 📌 Features & Architecture

This repository uses a modular, multi-file structure to provide deep domain knowledge without cluttering context windows until needed:

* **`SKILL.md` (Main Core Rules):** Defines the orchestrator logic, trigger conditions, and overall guiding principles for Claude.
* **10 Reference Modules:**
  * 🎮 **Unreal Engine / Game Dev (2 Files):** Blueprint patterns, architecture principles, performance optimization, and game mechanics setup.
  * ⚙️ **Mechatronic Engineering (6 Files):** Engineering calculations, physical system modeling, embedded logic, robotics, and hardware/control theory.
  * 🛠️ **Category-Independent / Utility (2 Files):** General project structures, formatting standards, and cross-domain workflow rules.

---

## ⚡ How It Works (Triggering & Session Persistence)

1. Once installed/configured, the skill remains lightweight until triggered.
2. It automatically activates when you express a clear development intention (e.g., *"Bir proje geliştiriyorum"*, *"Yeni bir UE projesine başlıyorum"*, etc.).
3. **Session Persistence:** Once activated, the context stays active throughout the entire conversation thread — no need to re-trigger or repeat instructions in subsequent prompts within that chat.

---

## 🚀 Installation & Usage

1. Copy or reference the content of `SKILL.md` (along with the `/references` folder) into your **Claude Custom Skills / Instructions** setup or your project's system prompt area.
2. Start a conversation with Claude and declare your project intent (e.g. in Turkish: *"Mekatronik ve UE5 odaklı yeni bir proje geliştiriyorum"*).
3. Claude will load the appropriate reference modules and guide you through engineering calculations, Blueprint/C++ architecture, or system design.

---

## 📄 License & Attribution

Feel free to fork, adapt, and improve this skill set for your own mechatronics and game development workflows!

Created by [JHEXLEX](https://github.com/JHEXLEX).
