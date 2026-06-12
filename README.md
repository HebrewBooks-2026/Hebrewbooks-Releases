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

יש שתי דרכי התקנה — בחר אחת:

> ### 🟢 התקנה אופליין — מומלץ (במיוחד אם נתקלת בבעיות התקנה או רשת)
> קובץ התקנה אחד שכולל **הכל** (.NET 8 + WebView2). אין צורך בדרישות מקדימות ואין צורך בחיבור אינטרנט בזמן ההתקנה. גדול יותר (~280MB) אך פשוט וחסין-תקלות.
> 👉 **[הורדה: HebrewBooks-offline-Setup.exe](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/latest/download/HebrewBooks-offline-Setup.exe)**
> *(לאחר ההתקנה אפשר לדלג ישר לשלב 3 — הקטלוג.)*

או — **התקנה רגילה**: קובץ קטן (~31MB), אך דורשת את הדרישות המקדימות שבשלב 1 וחיבור אינטרנט בזמן ההתקנה.

### שלב 1 — דרישות מקדימות (רק להתקנה הרגילה, פעם אחת)

לפני ההתקנה הרגילה הראשונה יש להתקין שני רכיבים שווינדוס לא תמיד כוללת (ההתקנה האופליין כוללת אותם — דלג על שלב זה אם בחרת בה):

#### .NET Desktop Runtime
מאפשר לתוכנה לרוץ כ-WPF .NET.
👉 **[הורדה: windowsdesktop-runtime-8.0.27-win-x86.exe](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/download/prerequisites/windowsdesktop-runtime-8.0.27-win-x86.exe)**
*(לאחר ההורדה, הרץ את הקובץ בלחיצה כפולה והמתן שהמתקין יסתיים — ~30 שניות. התוכנה מבוססת .NET 8 והיא 32-ביט (x86) — חובה להתקין דווקא את הגרסה הזו, לא x64 ולא גרסה 10.)*

#### WebView2 Runtime
מאפשר לתוכנה להציג את ה-PDFים והטקסטים בתוך החלון.
👉 **[הורדה: MicrosoftEdgeWebView2RuntimeInstallerX64.exe](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/download/prerequisites/MicrosoftEdgeWebView2RuntimeInstallerX64.exe)**
*(הרץ את הקובץ בלחיצה כפולה והמתן שההתקנה תסתיים — ~30 שניות.)*

### שלב 2 — התקנת התוכנה
👉 **[הורדה: HebrewBooks-stable-Setup.exe (גרסה אחרונה)](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/latest/download/HebrewBooks-stable-Setup.exe)**

ההתקנה תיצור קיצור ב-Start menu. בהפעלה ראשונה התוכנה תבקש לבחור את התיקייה שבה נמצא כונן הספריה (ה-USB עם תיקיית `App\Katalog.db`).

### שלב 3 — קטלוג הספרים (אופציונלי)
אם אין לך קטלוג קיים, אפשר להוריד את הקטלוג המלא:
👉 **[הורדה: Katalog.db (קטלוג מלא)](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/download/prerequisites/Katalog.db)**

מקם את הקובץ ב-`<DataRoot>\App\Katalog.db` (היכן ש-`<DataRoot>` היא התיקייה שבחרת בהפעלה הראשונה).

### גרסה ניידת (ללא התקנה)
למי שמעדיף — קיים גם פורמט portable שלא דורש הרשאות מנהל:
[HebrewBooks-stable-Portable.zip](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/latest/download/HebrewBooks-stable-Portable.zip)

### התקנה לכל המשתמשים במחשב (מתקדם — דורש מנהל)
ברירת המחדל היא התקנה **למשתמש הנוכחי בלבד** (עם עדכון אוטומטי). למי שרוצה להתקין פעם אחת **לכל המשתמשים** במחשב (דורש הרשאות מנהל) — יש סקריפט ייעודי:
👉 **[הורדה: install-all-users.ps1](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/releases/download/prerequisites/install-all-users.ps1)**

הרצה ב-PowerShell (הסקריפט יבקש הרשאות מנהל בעצמו):
```powershell
.\install-all-users.ps1                                      # התקנה ל-C:\Program Files\HebrewBooks
.\install-all-users.ps1 -Offline                             # חבילה הכוללת .NET + WebView2 (ללא דרישות מקדימות)
.\install-all-users.ps1 -InstallPath "D:\Apps\HebrewBooks"   # נתיב מוחלט אחר
```
הסקריפט מוריד את הגרסה הניידת האחרונה, פורס אותה למיקום המשותף, ויוצר קיצורים ב-Start menu ובשולחן העבודה לכל המשתמשים. **עדכון:** בהתקנה זו אין עדכון אוטומטי (היא מנוהלת ע"י מנהל) — כשיוצאת גרסה חדשה פשוט מריצים את הסקריפט שוב. ההגדרות והנתונים של כל משתמש נשמרים בנפרד (ב-`%AppData%`) ואינם מושפעים.

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

[פתח Issue ב-GitHub](https://github.com/HebrewBooks-2026/Hebrewbooks-Releases/issues) או שלח מייל ל-**HebrewBooks2026@gmail.com**.

---

## 📜 רישוי

תוכנה לשימוש אישי. ספרי המקור והאינדקסים משווקים בנפרד עם תנאי השימוש שלהם.
