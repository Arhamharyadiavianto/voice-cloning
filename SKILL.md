---
name: voice-cloning
description: Framework rekayasa persona, ekstraksi leksikon, dan kloning gaya bicara/tone (Voice Cloning Architecture). Gunakan saat user memanggil /voice-cloning, /voicecloning, /bikin-voice-cloning, /bikinvoicecloning, atau meminta kloning gaya bahasa, bedah tone of voice dari transkrip/teks, dan pembuatan persona suara/tulisan berbasis 5 Pilar Voice Cloning.
---

# Voice Cloning Engine (/voice-cloning)

Framework rekayasa persona dan kloning tone of voice berbasis 5 Pilar Voice Cloning Architecture. Dirancang untuk mengekstraksi ritme bahasa, spektrum emosi, kamus kata khas, serta logika berpikir seseorang dari raw text atau transkrip lisan agar bisa direplikasi secara presisi tanpa terdengar seperti bot AI (zero AI-slop).

---

## 1. Trigger & Aktivasi

Skill ini aktif ketika:
- User memanggil perintah: `/voice-cloning`, `/voicecloning`, `/bikin-voice-cloning`, `/bikinvoicecloning`.
- User meminta untuk mengkloning gaya bicara seseorang, menduplikasi tone tulisan, atau mengekstrak gaya komunikasi dari sampel postingan, transkrip video/audio, atau obrolan chat.

---

## 2. Minimum Supply Kata & Sampling Standards

Untuk menghasilkan kloning tone yang presisi, gunakan acuan kuantitas sampel berikut:

| Level Kedalaman | Minimum Supply Kata | Bentuk Sampel yang Dibutuhkan | Target Akurasi |
| :--- | :--- | :--- | :--- |
| **Level 1: Basic Vibe** | 300 - 500 kata | 3 - 5 postingan/tweet pendek atau 1 transkrip obrolan singkat. | Menangkap diksi dominan dan panjang kalimat kasar. Masih rentan bocor ke gaya AI standar. |
| **Level 2: Reliable Persona** | 1.500 - 2.500 kata | 10 - 15 draf konten/chat organik + sampel saat ada sedikit friksi/debat. | Nada bicara konsisten, ritme stabil, signature phrase terpasang rapi. Standar ideal untuk copywriting/ghostwriting. |
| **Level 3: Deep Clone** | 5.000+ kata (atau 30 - 45 menit transkrip audio unscripted) | Obrolan santai, debat/konflik, tulisan saat lelah/marah, transkrip podcast tanpa naskah. | Mengunci reasoning path, cadence jeda napas, logika defensif, hingga celetukan spontan tanpa pernah break character. |

**Aturan Leksikon Unik:** Minimal wajib mengekstrak **50 - 100 kosakata/frasa/idiom khas** ke dalam kamus aktif.

---

## 3. The 5 Pillars of Voice Cloning Architecture

Setiap analisis atau pembuatan persona suara/tone wajib mengeksekusi 5 pilar berikut:

### Pilar 1: Core DNA & Archetype Positioning
- **Arketipe Utama:** Tentukan persona dominan (misal: The Chic Strategist, Tough Love Mentor, Sarcastic Cynic, Playful Baddie, Academic Populist).
- **Status & Power Dynamics:** Apakah dia berbicara dari posisi setara (peer-to-peer), posisi atas yang berwibawa/intimidatif (high-status), atau posisi humble-melayani?
- **Vibe Sentral:** 1 kalimat manifesto yang mendefinisikan sikap hidup dan prinsip komunikasinya.

### Pilar 2: Vocabulary & Slang Mining (The Dual Lexicon)
- **Signature Lexicon (Wajib Ada):**
  - 10 - 20 kata/frasa penanda identitas utama (slang lokal, idiom bahasa Inggris, terminologi industri, plesetan khas) ditambah total 50 - 100 kosakata aktif.
  - Partikel percakapan dominan (misal: kan, sih, deh, kok, cuy, bro, bos).
- **Blacklist / Anti-Lexicon (Haram Dipakai):**
  - Kosakata korporat basi atau meta-fluff AI yang orang aslinya tidak akan pernah sebutkan (misal: "Tentu, mari kita selami", "Sobat Cuan", "Menyelami samudera").

### Pilar 3: Emotional & Conflict Dynamics (Kondisi Saat Emosi)
Bagaimana subjek merespons 4 kuadran emosi utama:
1. **Saat Marah / Jengkel:** Apakah meledak-ledak (tough love fakta keras), dingin menampar (deadpan sarcasm), atau defensif-tsundere?
2. **Saat Menghadapi Kritik / Debat:** Apakah membantai dengan kausalitas data, meremehkan dengan analogi pop-culture, atau membalas staccato 1 baris yang membungkam?
3. **Saat Bersemangat / Gembira:** Apakah melempar pujian brutal, antusiasme teknis hiperbolis, atau pura-pura cuek (nonchalant)?
4. **Saat Menghibur / Menenangkan:** Apakah memberi solusi pragmatis tanpa drama, atau validasi empati mendalam?

### Pilar 4: Sentence Structure & Rhythm (Cadence & Breathing)
- **Panjang Kalimat:** Apakah dominan micro-staccato (1 - 2 baris pendek per paragraf) atau flowing narrative (panjang sinematik)?
- **Tanda Baca & Jeda Napas:** Penggunaan elipsis (`...`) untuk jeda berpikir santai, tanda seru (`!`) untuk perintah/keberanian, tanda hubung (`-`) untuk interupsi pikiran.
- **Code-Switching Rules:** Pola perpindahan bahasa (kapan beralih ke bahasa Inggris, apakah hanya untuk istilah teknis atau untuk punchline emosi).

### Pilar 5: Behavioral Anchors & Unique Quirks
- Celetukan spontan, gumaman (hmm, eh, astaga), tawa kecil (chuckle), atau panggilan sapaan selektif kepada lawan bicara.

---

## 4. The 3 Golden Rules (Anti-Slop Protocol)
1. **Rule of Contrast (Anti-Monoton):** Selalu sematkan kontras karakter. Sosok yang sangat logis harus punya selera humor receh/analogi nyeleneh. Sosok yang santai harus bisa bersikap sangat tajam saat prinsipnya diinjak.
2. **Eliminasi Meta-Fluff:** Langsung mulai kalimat pertama dengan konten/argumen tanpa pembuka robotik ("Berikut adalah..." atau "Sebagai seorang X, saya...").
3. **Consistency Under Pressure:** Tetap pertahankan gaya bahasa, diksi khas, dan logika arketipe saat menghadapi pertanyaan jebakan, emosional, atau provokatif.

---

## 5. Output Format saat Skill Dijalankan

Saat user memberikan materi teks/transkrip untuk dikloning, berikan output dengan format:
1. **Persona Summary Card** (Arketipe, Status, Vibe Utama).
2. **Kamus Bahasa & Leksikon** (50 - 100 Signature Vocab, Partikel, Blacklist Vocab).
3. **Matriks Spektrum Emosi** (Respons Marah, Debat, Gembira, Menenangkan).
4. **Pedoman Struktur Kalimat & Ritmika**.
5. **System Prompt / Persona Instruction Siap Pakai** (Instruksi siap tempel agar LLM langsung berbicara dalam suara tersebut).
