<!--
  Source for the public homepage of HebrewBooks-2026/Hebrewbooks-Releases.
  Copy this file's contents into the README.md of that repository (the file you're
  reading now lives in the SOURCE repo only because GitHub renders the releases
  repo's own README.md on the public landing page).

  After committing, upload the two prerequisite files as assets on a single
  release tagged "prerequisites" on the releases repo, so the download links
  below resolve. Steps in the script's header.
-->

<div align="center">

# ארון הספרים הדיגיטלי

#### גלישה וחיפוש בספריית PDFים עברית, עם תוכן עניינים אינטראקטיבי וחיפוש דקדקני בתוך הספרים

[![הורדה אחרונה](https://img.shields.io/badge/הורדה_אחרונה-blue?style=for-the-badge&logo=github)](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/latest/download/HebrewBooks-stable-Setup.exe)
[![גרסה](https://img.shields.io/github/v/release/HebrewBooks-2026/Hebrewbooks-Releases?style=for-the-badge&label=גרסה)](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/latest)

</div>

---

## 📥 התקנה

### שלב 1 — דרישות מקדימות (פעם אחת)

לפני התקנת התוכנה הראשונה, יש להתקין שני רכיבים שווינדוס לא תמיד כוללת:

#### .NET Desktop Runtime
מאפשר לתוכנה לרוץ כ-WPF .NET.
👉 **[הורדה: windowsdesktop-runtime-10.0.7-win-x64.exe](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/download/prerequisites/windowsdesktop-runtime-10.0.7-win-x64.exe)**
*(לאחר ההורדה, הריצי את הקובץ פעמיים-כפול והמתיני שהמתקין מסתיים — ~30 שניות.)*

#### WebView2 Fixed Version Runtime
מאפשר לתוכנה להציג את ה-PDFים והטקסטים בתוך החלון.
👉 **[הורדה: Microsoft.WebView2.FixedVersionRuntime.147.0.3912.98.x64.cab](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/download/prerequisites/Microsoft.WebView2.FixedVersionRuntime.147.0.3912.98.x64.cab)**
*(אם וינדוס מציעה לפתוח את ה-CAB עם "File Explorer" — לחץ "פתיחה" וב-File Explorer לחץ כפול על הקובץ הראשי שבתוכו.)*

### שלב 2 — התקנת התוכנה
👉 **[הורדה: HebrewBooks-stable-Setup.exe (גרסה אחרונה)](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/latest/download/HebrewBooks-stable-Setup.exe)**

ההתקנה תיצור קיצור ב-Start menu. בהפעלה ראשונה התוכנה תבקש לבחור את התיקייה שבה נמצא כונן הספריה (ה-USB עם תיקיית `App\Katalog.db`).

### שלב 3 — קטלוג הספרים (אופציונלי)
אם אין לך קטלוג קיים, אפשר להוריד את הקטלוג המלא:
👉 **[הורדה: Katalog.db (קטלוג מלא)](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/download/prerequisites/Katalog.db)**

מקם/י את הקובץ ב-`<DataRoot>\App\Katalog.db` (היכן ש-`<DataRoot>` היא התיקייה שבחרת בהפעלה הראשונה).

### גרסה ניידת (ללא התקנה)
למי שמעדיף — קיים גם פורמט portable שלא דורש הרשאות מנהל:
[HebrewBooks-stable-Portable.zip](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/latest/download/HebrewBooks-stable-Portable.zip)

---

## ✨ פיצ׳רים עיקריים

- **חיפוש מהיר ומדויק** בתוכן 60,000+ ספרי PDF (מבוסס dtSearch) + ספרי טקסט מאוצריא
- **תוכן עניינים אינטראקטיבי** לכל ספר — לחץ על סעיף, קופצים לעמוד
- **סינון לפי מאגר** — HebrewBooks / אוצריא / שניהם
- **עריכת מטא-דאטה** — שמות, מחברים, מקומות, נושאים
- **הורדה אוטומטית של ספרים חדשים** מהאתר
- **ייצוא/ייבוא תוכניות עניינים** לשיתוף עם משתמשים אחרים
- **עדכוני תוכנה אוטומטיים** דרך Velopack — בלי להוריד מחדש כל פעם

---

## 🔄 עדכונים אוטומטיים

מהגרסה ההותקנת, התוכנה בודקת מדי הפעלה אם יש גרסה חדשה. ניתן גם להפעיל בדיקה ידנית מ-**הגדרות → עדכוני תוכנה → בדוק עדכונים**. עדכונים מתבצעים דרך מנגנון Velopack (delta packages — בעדכון רגיל מורידים פחות מ-1MB).

---

## 🐛 דיווח באג / יצירת קשר

[פתחי Issue ב-GitHub](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/issues) או שלח מייל ל-**HebrewBooks2026@gmail.com**.

---

## 📜 רישוי

תוכנה לשימוש אישי.
