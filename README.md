# Quran 15 Lines — Majeedia Mushaf

**Author:** MAKTAB-e-ASHRAF  
**Format:** 15 Lines per page  
**Total Pages:** 624  
**Total Paras (Juz):** 30  

---

## 📦 Repository Structure

This repository contains **30 zip files**, one per Para (Juz) of the Holy Quran.

| File | Para | Pages | Page Range |
|------|------|-------|------------|
| `parah_01.zip` | Para 1 — اَلٓمٓ | 21 | 001–021 |
| `parah_02.zip` | Para 2 — سَيَقُوۡلُ | 21 | 022–042 |
| `parah_03.zip` | Para 3 — تِلۡكَ الرُّسُلُ | 21 | 043–063 |
| `parah_04.zip` | Para 4 — لَنۡ تَنَالُوا | 21 | 064–084 |
| `parah_05.zip` | Para 5 — وَالۡمُحۡصَنَاتُ | 21 | 085–105 |
| `parah_06.zip` | Para 6 — لَا يُحِبُّ اللّٰهُ | 21 | 106–126 |
| `parah_07.zip` | Para 7 — وَاِذَا سَمِعُوۡا | 21 | 127–147 |
| `parah_08.zip` | Para 8 — وَلَوۡ اَنَّنَا | 21 | 148–168 |
| `parah_09.zip` | Para 9 — قَالَ الۡمَلَاُ | 21 | 169–189 |
| `parah_10.zip` | Para 10 — وَاعۡلَمُوۡۤا | 21 | 190–210 |
| `parah_11.zip` | Para 11 — يَعۡتَذِرُوۡنَ | 21 | 211–231 |
| `parah_12.zip` | Para 12 — وَمَا مِنۡ دَآبَّةٍ | 21 | 232–252 |
| `parah_13.zip` | Para 13 — وَمَاۤ اُبَرِّئُ | 21 | 253–273 |
| `parah_14.zip` | Para 14 — رُبَمَا | 21 | 274–294 |
| `parah_15.zip` | Para 15 — سُبۡحٰنَ الَّذِىۡۤ | 21 | 295–315 |
| `parah_16.zip` | Para 16 — قَالَ اَلَمۡ | 21 | 316–336 |
| `parah_17.zip` | Para 17 — اِقۡتَرَبَتۡ | 21 | 337–357 |
| `parah_18.zip` | Para 18 — قَدۡ اَفۡلَحَ | 21 | 358–378 |
| `parah_19.zip` | Para 19 — وَقَالَ الَّذِيۡنَ | 21 | 379–399 |
| `parah_20.zip` | Para 20 — اَمَّنۡ خَلَقَ | 21 | 400–420 |
| `parah_21.zip` | Para 21 — اُتۡلُ مَاۤ اُوۡحِىَ | 21 | 421–441 |
| `parah_22.zip` | Para 22 — وَمَنۡ يَّقۡنُتۡ | 21 | 442–462 |
| `parah_23.zip` | Para 23 — وَمَالِىَ | 21 | 463–483 |
| `parah_24.zip` | Para 24 — فَمَنۡ اَظۡلَمُ | 21 | 484–504 |
| `parah_25.zip` | Para 25 — اِلَيۡهِ يُرَدُّ | 21 | 505–525 |
| `parah_26.zip` | Para 26 — حٰمٓ | 21 | 526–546 |
| `parah_27.zip` | Para 27 — قَالَ فَمَا خَطۡبُكُمۡ | 21 | 547–567 |
| `parah_28.zip` | Para 28 — قَدۡ سَمِعَ اللّٰهُ | 21 | 568–588 |
| `parah_29.zip` | Para 29 — تَبٰرَكَ الَّذِىۡ | 21 | 589–609 |
| `parah_30.zip` | Para 30 — عَمَّ | 15 | 610–624 |

---

## 🖼️ Image Format Inside Each Zip

Each zip contains JPEG images named by **global page number**:

```
parah_01.zip
  ├── 001.jpg   ← Page 1  of the Quran
  ├── 002.jpg   ← Page 2
  ├── ...
  └── 021.jpg   ← Page 21

parah_02.zip
  ├── 022.jpg   ← Page 22
  ├── ...
  └── 042.jpg   ← Page 42
```

- **Image size:** 1030×1387 pixels (JPEG, RGB)
- **Cover page (001.jpg):** 1792×2371 pixels (higher resolution title page)
- **File size per zip:** ~2 MB

---

## 📱 Android App Integration

This repository is used by the **NoorAlHuda** Android Quran App.

### Raw Download URL Pattern
```
https://raw.githubusercontent.com/YOUR_USERNAME/quran_15_lines/main/parah_01.zip
https://raw.githubusercontent.com/YOUR_USERNAME/quran_15_lines/main/parah_02.zip
...
```

### How the App Loads Pages
1. App downloads `parah_NN.zip` on demand
2. Extracts JPEG images to internal storage: `filesDir/quran_15/pNN/`
3. Displays page images in the reader view

### Para Start Pages (for `QuranType.java`)
```java
new int[]{
      1, 22, 43, 64, 85,106,127,148,169,190,
    211,232,253,274,295,316,337,358,379,400,
    421,442,463,484,505,526,547,568,589,610
}
```

---

## ⬆️ How to Upload to GitHub

### Option A — GitHub Web (Easiest)
1. Create a new repo: `github.com/YOUR_USERNAME/quran_15_lines`
2. Set visibility: **Public**
3. Click **Add file → Upload files**
4. Drag all 30 `.zip` files + `README.md`
5. Click **Commit changes**

### Option B — Git CLI
```bash
git init quran_15_lines
cd quran_15_lines
cp /path/to/parah_*.zip .
cp /path/to/README.md .
git add .
git commit -m "Add 15-line Quran (Majeedia Mushaf) - 624 pages, 30 Para zips"
git remote add origin https://github.com/YOUR_USERNAME/quran_15_lines.git
git push -u origin main
```

### Option C — GitHub CLI
```bash
gh repo create quran_15_lines --public --clone
cd quran_15_lines
cp /path/to/parah_*.zip .
cp /path/to/README.md .
git add . && git commit -m "Initial upload: 15-line Quran 30 paras"
git push
```

> ⚠️ **Large File Warning:** Each zip is ~2 MB. Total repo = ~63 MB.
> GitHub allows up to 100 MB per file and 1 GB per repo — you're well within limits.

---

## ✅ Verified
- Source: `Quran_15_Lines.pdf` (MAKTAB-e-ASHRAF, 624 pages)
- All 624 pages extracted and accounted for
- Para boundaries match `QuranType.LINES_15.parahStart[]` in the Android app
