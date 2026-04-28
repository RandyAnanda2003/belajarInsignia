# Prompt Writing Skill

Skill ini membantu AI menghasilkan prompt berkualitas tinggi menggunakan framework RISEN dan prinsip one-shot prompting.

## Framework RISEN

RISEN adalah framework untuk menulis prompt yang efektif:

- **R**ole (Peran): Definisikan peran atau identitas AI
- **I**nstructions (Instruksi): Berikan instruksi yang jelas dan spesifik
- **S**teps (Langkah): Uraikan langkah-langkah yang harus diikuti
- **E**nd Goal (Tujuan Akhir): Jelaskan hasil yang diinginkan
- **N**arrowing (Penyempitan): Batasi scope dan berikan konteks spesifik

## Prinsip One-Shot Prompting

One-shot prompting memberikan satu contoh konkret untuk memandu AI memahami format dan gaya output yang diinginkan.

## Cara Menggunakan Skill Ini

Ketika pengguna meminta untuk membuat prompt, ikuti struktur berikut:

### 1. Role (Peran)

```
Anda adalah [peran spesifik dengan keahlian tertentu].
```

**Contoh:**

- "Anda adalah seorang software architect berpengalaman dengan keahlian dalam sistem terdistribusi."
- "Anda adalah content writer profesional yang ahli dalam copywriting persuasif."
- "Anda adalah data scientist dengan spesialisasi machine learning dan analisis prediktif."

### 2. Instructions (Instruksi)

```
Tugas Anda adalah [instruksi utama yang jelas dan actionable].
```

**Prinsip instruksi yang baik:**

- Gunakan kata kerja aktif (analisis, buat, tulis, evaluasi, bandingkan)
- Spesifik dan terukur
- Hindari ambiguitas
- Satu instruksi utama per prompt

**Contoh:**

- "Tugas Anda adalah menganalisis kode berikut dan mengidentifikasi potensi bottleneck performa."
- "Tugas Anda adalah menulis artikel blog 800 kata tentang best practices keamanan API."

### 3. Steps (Langkah-langkah)

```
Ikuti langkah-langkah berikut:
1. [Langkah pertama]
2. [Langkah kedua]
3. [Langkah ketiga]
...
```

**Prinsip langkah yang efektif:**

- Urutan logis dan kronologis
- Setiap langkah jelas dan dapat dieksekusi
- Maksimal 5-7 langkah untuk menghindari kompleksitas berlebihan
- Gunakan sub-langkah jika diperlukan

**Contoh:**

```
Ikuti langkah-langkah berikut:
1. Baca dan pahami konteks kode yang diberikan
2. Identifikasi pola-pola yang berpotensi menyebabkan masalah performa
3. Prioritaskan temuan berdasarkan dampak terhadap performa
4. Berikan rekomendasi perbaikan untuk setiap temuan
5. Sertakan contoh kode untuk implementasi rekomendasi
```

### 4. End Goal (Tujuan Akhir)

```
Output akhir yang diharapkan adalah [deskripsi hasil yang spesifik dan terukur].
```

**Prinsip end goal yang baik:**

- Jelaskan format output (list, paragraf, tabel, kode, dll)
- Tentukan panjang atau ukuran jika relevan
- Sebutkan elemen-elemen yang harus ada
- Berikan kriteria kualitas jika perlu

**Contoh:**

- "Output akhir adalah laporan dalam format markdown dengan 3 bagian: (1) Ringkasan eksekutif, (2) Temuan detail dengan code snippets, (3) Rekomendasi prioritas."
- "Output akhir adalah fungsi Python yang telah dioptimasi dengan kompleksitas waktu O(n log n) atau lebih baik, lengkap dengan docstring dan unit tests."

### 5. Narrowing (Penyempitan)

```
Konteks dan batasan:
- [Batasan 1]
- [Batasan 2]
- [Konteks spesifik]
```

**Prinsip narrowing yang efektif:**

- Batasi scope untuk menghindari output yang terlalu luas
- Berikan konteks domain atau industri
- Sebutkan constraint teknis (bahasa pemrograman, framework, versi)
- Tentukan audience atau use case
- Hindari topik atau pendekatan tertentu jika perlu

**Contoh:**

```
Konteks dan batasan:
- Fokus pada aplikasi Node.js dengan Express.js
- Target audience adalah developer mid-level
- Hindari solusi yang memerlukan perubahan arsitektur besar
- Prioritaskan solusi yang dapat diimplementasikan dalam 1-2 hari
- Gunakan TypeScript untuk semua contoh kode
```

## One-Shot Example Template

Setelah struktur RISEN, berikan satu contoh konkret:

```
## Contoh Input dan Output

**Input:**
[Contoh input yang representatif]

**Output yang Diharapkan:**
[Contoh output yang menunjukkan format, gaya, dan struktur yang diinginkan]
```

## Template Lengkap

```
# [Judul Prompt]

## Role
Anda adalah [peran spesifik dengan keahlian].

## Instructions
Tugas Anda adalah [instruksi utama yang jelas].

## Steps
Ikuti langkah-langkah berikut:
1. [Langkah 1]
2. [Langkah 2]
3. [Langkah 3]
4. [Langkah 4]
5. [Langkah 5]

## End Goal
Output akhir yang diharapkan adalah [deskripsi hasil spesifik dengan format].

## Narrowing
Konteks dan batasan:
- [Batasan 1]
- [Batasan 2]
- [Konteks 3]
- [Constraint 4]

## One-Shot Example

**Input:**
[Contoh input]

**Output yang Diharapkan:**
[Contoh output lengkap]
```

## Best Practices

### DO (Lakukan):

✅ Gunakan bahasa yang jelas dan tidak ambigu
✅ Berikan contoh konkret dalam one-shot example
✅ Spesifik tentang format output yang diinginkan
✅ Batasi scope dengan jelas di bagian Narrowing
✅ Gunakan bullet points dan numbering untuk struktur yang jelas
✅ Test prompt dengan berbagai input untuk memastikan konsistensi
✅ Iterasi dan perbaiki berdasarkan hasil

### DON'T (Hindari):

❌ Instruksi yang terlalu umum atau abstrak
❌ Terlalu banyak langkah (>7) yang membingungkan
❌ Kontradiksi antara instruksi dan end goal
❌ Asumsi tentang pengetahuan yang tidak dinyatakan
❌ Prompt yang terlalu panjang (>1000 kata tanpa alasan kuat)
❌ Multiple tasks dalam satu prompt tanpa prioritas jelas
❌ Mengabaikan konteks atau constraint penting

## Contoh Prompt Lengkap

### Contoh 1: Code Review Prompt

````
# Code Review untuk API Endpoint

## Role
Anda adalah senior backend engineer dengan 10+ tahun pengalaman dalam membangun RESTful APIs yang scalable dan secure.

## Instructions
Tugas Anda adalah melakukan code review menyeluruh terhadap API endpoint yang diberikan dan memberikan feedback konstruktif.

## Steps
Ikuti langkah-langkah berikut:
1. Analisis struktur dan organisasi kode
2. Evaluasi error handling dan edge cases
3. Periksa keamanan (authentication, authorization, input validation)
4. Assess performa dan potensi bottleneck
5. Review readability dan maintainability
6. Berikan rating 1-10 untuk setiap aspek
7. Prioritaskan rekomendasi perbaikan (Critical, High, Medium, Low)

## End Goal
Output akhir adalah code review report dalam format markdown dengan struktur:
- Executive Summary (2-3 kalimat)
- Detailed Findings (per kategori dengan rating)
- Prioritized Recommendations (dengan contoh kode)
- Overall Score dan kesimpulan

## Narrowing
Konteks dan batasan:
- Fokus pada Node.js/Express.js endpoints
- Asumsikan production environment dengan high traffic
- Prioritaskan security dan performance issues
- Gunakan industry best practices (OWASP, REST standards)
- Berikan contoh kode dalam TypeScript

## One-Shot Example

**Input:**
```javascript
app.get('/users/:id', async (req, res) => {
  const user = await db.query('SELECT * FROM users WHERE id = ' + req.params.id);
  res.json(user);
});
````

**Output yang Diharapkan:**

# Code Review Report

## Executive Summary

Endpoint memiliki critical security vulnerability (SQL injection) dan tidak memiliki error handling. Memerlukan perbaikan segera sebelum production.

## Detailed Findings

### Security: 2/10 ⚠️ CRITICAL

- **SQL Injection vulnerability**: Query menggunakan string concatenation
- **No authentication**: Endpoint tidak memverifikasi user identity
- **No authorization**: Tidak ada pemeriksaan akses

### Error Handling: 1/10 ⚠️ CRITICAL

- Tidak ada try-catch block
- Tidak ada validasi input
- Tidak ada handling untuk user not found

### Performance: 5/10

- Query SELECT \* tidak efisien
- Tidak ada caching mechanism
- Tidak ada pagination

### Code Quality: 4/10

- Tidak ada type safety
- Tidak ada logging
- Tidak ada documentation

## Prioritized Recommendations

### CRITICAL (Fix Immediately)

1. **Fix SQL Injection**

```typescript
app.get("/users/:id", async (req, res) => {
  const user = await db.query("SELECT * FROM users WHERE id = $1", [
    req.params.id,
  ]);
});
```

2. **Add Error Handling**

```typescript
app.get("/users/:id", async (req, res, next) => {
  try {
    const userId = parseInt(req.params.id);
    if (isNaN(userId)) {
      return res.status(400).json({ error: "Invalid user ID" });
    }
    // ... rest of code
  } catch (error) {
    next(error);
  }
});
```

[... dst]

## Overall Score: 3/10

Endpoint memerlukan refactoring signifikan sebelum production-ready.

```

```

### Contoh 2: Content Writing Prompt

````
# Blog Post Writer untuk Technical Topics

## Role
Anda adalah technical content writer yang ahli dalam menjelaskan konsep kompleks dengan cara yang mudah dipahami untuk developer mid-level.

## Instructions
Tugas Anda adalah menulis blog post yang engaging dan informatif tentang topik teknis yang diberikan.

## Steps
Ikuti langkah-langkah berikut:
1. Buat outline dengan 3-5 section utama
2. Tulis introduction yang menarik dengan hook yang kuat
3. Kembangkan setiap section dengan:
   - Penjelasan konsep
   - Code examples yang praktis
   - Real-world use cases
4. Tambahkan visual aids (diagram, flowchart) jika perlu
5. Tulis conclusion dengan key takeaways
6. Sertakan references dan further reading

## End Goal
Output akhir adalah blog post 1000-1500 kata dalam format markdown dengan:
- Engaging title dan meta description
- Clear structure dengan headers (H2, H3)
- Minimal 3 code examples dengan syntax highlighting
- 1-2 diagram atau visual representation
- Actionable takeaways di akhir

## Narrowing
Konteks dan batasan:
- Target audience: Developer dengan 2-5 tahun pengalaman
- Tone: Professional tapi conversational
- Hindari jargon tanpa penjelasan
- Fokus pada practical applications, bukan teori murni
- Gunakan contoh dari real-world projects
- Sertakan best practices dan common pitfalls

## One-Shot Example

**Input:**
Topic: "Understanding JavaScript Closures"

**Output yang Diharapkan:**

# Mastering JavaScript Closures: A Practical Guide

*Meta: Learn how JavaScript closures work with practical examples and real-world use cases. Understand scope, memory, and common patterns.*

## Introduction

Pernahkah Anda bertanya-tanya mengapa function dalam JavaScript bisa "mengingat" variable dari outer scope-nya? Jawabannya adalah closures - salah satu konsep fundamental yang membuat JavaScript powerful namun sering membingungkan.

Dalam artikel ini, kita akan membongkar misteri closures dengan pendekatan praktis. Anda akan belajar tidak hanya *apa* itu closures, tapi *kapan* dan *mengapa* menggunakannya dalam real-world applications.

## What Are Closures?

Closure adalah kombinasi dari function dan lexical environment di mana function tersebut dideklarasikan. Sederhananya: function yang memiliki akses ke variable dari outer scope-nya, bahkan setelah outer function selesai dieksekusi.

```javascript
function createCounter() {
  let count = 0; // Private variable

  return function() {
    count++;
    return count;
  };
}

const counter = createCounter();
console.log(counter()); // 1
console.log(counter()); // 2
console.log(counter()); // 3
````

[... artikel lengkap dengan sections lainnya ...]

## Key Takeaways

✅ Closures memungkinkan data encapsulation dan private variables
✅ Gunakan closures untuk factory functions dan module pattern
✅ Hati-hati dengan memory leaks dalam loops
✅ Closures adalah foundation untuk banyak JavaScript patterns modern

## Further Reading

- [MDN: Closures](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures)
- "You Don't Know JS: Scope & Closures" by Kyle Simpson

```

```

## Kapan Menggunakan Skill Ini

Aktifkan skill ini ketika pengguna:

- Meminta bantuan membuat prompt untuk AI
- Ingin meningkatkan kualitas prompt yang sudah ada
- Memerlukan template untuk prompt engineering
- Bertanya tentang best practices dalam prompt writing
- Ingin membuat prompt untuk use case spesifik (code review, content writing, data analysis, dll)

## Adaptasi untuk Berbagai Use Cases

### Technical Tasks (Code, Architecture, DevOps)

- Role: Spesifik tentang tech stack dan seniority level
- Steps: Fokus pada metodologi dan best practices
- Narrowing: Constraint teknis sangat penting (versions, compatibility)
- Example: Harus include working code

### Creative Tasks (Writing, Design, Marketing)

- Role: Emphasize style dan audience understanding
- Steps: Include brainstorming dan iteration
- Narrowing: Tone, brand voice, target demographic
- Example: Show desired style dan format

### Analytical Tasks (Data Analysis, Research, Strategy)

- Role: Domain expertise dan analytical frameworks
- Steps: Structured analysis methodology
- Narrowing: Data sources, constraints, assumptions
- Example: Complete analysis dengan insights

### Educational Tasks (Tutorials, Documentation, Explanations)

- Role: Teaching ability dan audience awareness
- Steps: Pedagogical approach (simple to complex)
- Narrowing: Prior knowledge level, learning objectives
- Example: Complete lesson dengan exercises

## Troubleshooting Prompts

Jika prompt tidak menghasilkan output yang diinginkan:

1. **Output terlalu umum** → Perkuat Narrowing dan berikan contoh lebih spesifik
2. **Output tidak konsisten** → Perjelas Steps dan End Goal
3. **Output tidak sesuai format** → Perbaiki One-Shot Example dengan format yang lebih detail
4. **Output terlalu pendek/panjang** → Spesifik tentang length di End Goal
5. **Output miss the point** → Review Instructions dan pastikan task jelas

## Iterasi dan Improvement

Prompt engineering adalah proses iteratif:

```
Version 1 → Test → Analyze gaps → Version 2 → Test → Refine → Final
```

Untuk setiap iterasi:

- Document apa yang tidak bekerja
- Identify bagian RISEN mana yang perlu diperbaiki
- Test dengan multiple inputs
- Gather feedback dan adjust
