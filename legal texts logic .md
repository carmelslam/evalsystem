**📁 LEGAL TEXTS VAULT - FINAL REPORT VARIANTS**

---

### 🔰 Final Report Types

All report types share the same core structure. They differ only in:

1. **The text block used at the end of the report.**
2. **Extra input fields required to complete that block.**

#### ✅ Current Types:

* חוות דעת פרטית (Private) – default and most common
* חוות דעת גלובאלי (Global)
* חוות דעת טוטלוסט (Total Loss)
* מכירה מצבו הניזוק (Sold in Damaged Condition)
* אומדן (Estimate Report – **optional** intermediary, not final)

  * אומדן ראשוני - אובדן להלכה (Estimate Loss of Use)
  * אומדן ראשוני - טוטלוס (Estimate Total Loss)

Each of these types has a dedicated explanatory/legal text stored in this vault and retrieved dynamically during generation.

---

### 📦 Text Storage Format (Vault)

```json
{
  "private": {
    "title": "חוות דעת פרטית",
    "text": "(to be filled later)"
  },
  "global": {
    "title": "חוות דעת גלובאלי",
    "text": "בהתאם לבקשה סיכמנו את חוות דעתנו בטרם קבלת חשבנות התיקון, (גלובאלי).\n\nהערכת הנזקים אינה כוללת נזקים בלתי נראים מראש העלולים להתגלות במהלך פירוק.\n\nמחירי החלפים נבדקו על ידינו בתוכנת מולטיקט חלפים.\n\nערך הרכב המצויין לעיל בהתאם למחירון ואינו מתייחס למקוריות הרכב בעבר וארוע תאונתי.\n\nמאחר ובעלי הרכב מעוניין בתיקון רכבו בכוחות עצמו, ובתאום עם בעלי הרכב. התביעה הנ\"ל נסגירה על בסיס גלובאלי בסך %שווי_פיצוי% ש\"ח כולל מע\"מ. את הרכב יתקנו הבעלים בכוחות עצמם.\n\nחוות דעתינו כוללת סעיף י\"ע בשיעור %ירידת_ערך%% מערך הרכב המצויין לעיל בגין הפגיעה באירוע הנדון.\n\nאושר מע\"מ בהתאם לפסקי דין רלוונטיים.\n\nהערכתנו מתייחסת לנזקים כפי שהוצגו בפנינו, ולנסיבות המקרה כפי שתוארו לנו ע\"י בעל הרכב אשר לדבריו.\n\nלטענת בעל הרכב %מספר_מוקדים% מוקדי הנזק מאירוע הנדון.\n\nאנו מערכים שהיית הרכב במוסך לצורך תיקונים בכ %ימי_מוסך% ימים."
  },
  "total_loss": {
    "title": "חוות דעת טוטלוסט",
    "text": "חוות דעתינו בוצעה בטרם בוצעו התיקונים בפועל ואינה כוללת את הנזקים הסמויים בשלב זה של הבדיקה.\n\nבהתאם לבדיקתנו הנזק ברכב הדון הינו מעל 60% מערך הרכב, ובהתאם לתקנות התעבורה סעיף 9 לצו הפיקוח על המצרכים והשירותים סעיף ב, הוכרז הרכב הנ\"ל כניזוק ב \"אובדן גמור (טוטאלוס)\".\n\nמאחר וערך הנזק הראשוני הינו מעל 60% מערך הרכב הנ\"ל, ואין כל כדאיות כלכלית ו/או בטיחותית בתיקון הרכב, לכן הרכב הוכרז כניזוק ב \"אובדן גמור (טוטאלוס)\" ויועד לפירוק בלבד.\n\nרשיון הרכב בוטל על ידי משרדינו בהתאם להנחיית משרד התחבורה.\n\nשרידי הרכב לפירוק הוערכו על ידינו בסך %שווי_שרידים% ש\"ח.\n\nמחירי החלפים נבדקו על ידינו בתוכנת מולטיקט חלפים.\n\nאנו ממלצים לפצות את המבוטח על בסיס אובדן גמור (טוטאלוס).\n\nרשיון הרכב בצירוף טופס 587 נשלח למשרד הרישוי. שרדי הרכב נשארו בידי המבוטח לפירוק בלבד.\n\nבדיקותינו העלו כי מספר השלדה אשר נבדק על ידנו ברכב תואם רישיון הרכב."
  },
  "damaged_sale": {
    "title": "מכירה מצבו הניזוק",
    "text": "בהתאם לבקשה סיכמנו את חוות דעתנו בטרם תיקון הרכב, זאת בהתייחסות לעוצמת הפגיעה נמכר הרכב במצבו הניזוק.\n\nהרכב נמכר ע\"י בעליו.\n\nהרכב במצבו הניזוק נמכר בסך %מחיר_מכירה% ש\"ח, %שיטת_תשלום%. מצורף זיכרון דברים בין שני הצדדים, והעברת בעלות.\n\nערך הרכב המצוין לעיל בהתאם למחירון ואינו מתייחס למקוריות הרכב בעבר ואירוע תאונתי.\n\nמחירי החלפים נבדקו על ידינו בתוכנת מולטיקט חלפים.\n\nהערכת הנזקים אינה כוללת נזקים בלתי נראים מראש העלולים להתגלות במהלך הפירוק.\n\nמצו\"ב צילום זיכרון דברים בגין מכירת הרכב.\n\nירידת ערך צפויה לרכב הנ\"ל %ירידת_ערך%% מערך הרכב הנ\"ל באירוע הנדון.\n\nאנו מערכים את משך שהיית הרכב במוסך לצורך תיקונים ב / כ %ימי_מוסך% ימי עבודה."
  },
  "estimate_אובדן_להלכה": {
    "title": "אומדן ראשוני - אובדן להלכה",
    "text": "ערך הרכב המצויין לעיל בהתאם למחירון ואינו מתייחס למקוריות הרכב בעבר וארוע תאונתי.\n\nהצעה זו אינה סופית ויתכן שינויים במהלך תיקון הרכב.\n\nהערכתנו מתייחסת לנזקים כפי שהוצגו בפנינו, ולנסיבות המקרה כפי שתוארו לנו ע\"י בעל הרכב אשר לדבריו.\n\nקוד דגם רישיון הרכב נבדק בהתאם לטבלת המרה של לוי יצחק ונמצא %קוד_דגם%.\n\nאחוז הנזק ברכב הנ\"ל הוא %אחוז_נזק% מערך הרכב.\n\nהצעה זו אינה כוללת נזקים בלתי נראים מראש העלולים להתגלות במהלך פירוק ו/או תיקון.\n\nלהערכתינו ירידת ערך צפויה כ %ירידת_ערך% מערך הרכב הנ\"ל מאירוע הנדון.\n\nלטענת בעל הרכב %מוקדי_נזק% מוקדי הנזק מאירוע הנדון.\n\nלאור היקף הנזקים אנו ממלצים לסלק את התביעה הנ\"ל על בסיס \"אובדן להלכה\" ללא תיקון בפועל.\n\nלהערכתינו זמן השהייה במוסך לצורך תיקון %ימי_מוסך% ימי עבודה."
  },
  "estimate_טוטלוס": {
    "title": "אומדן ראשוני - טוטלוס",
    "text": "חוות דעתינו מתבצעת בטרם תיקונים בפועל ואינה כוללת נזקים סמויים.\n\nבהתאם לבדיקה הנזק ברכב מוערך ביותר מ-60% מערך הרכב, ומשכך הרכב מסווג כטוטלוס.\n\nערך הרכב המחושב לפי מחירון לוי יצחק: %שווי_רכב%.\n\nשווי השרידים: %שווי_שרידים%.\n\nניכוי ירידת ערך: %ירידת_ערך%\n\nהערכת נזקים מבוססת על הנתונים שנמסרו ע\"י בעל הרכב, אשר לדבריו.\n\nהצהרה: אני החת"מ: ירון כיוף, תעודת שמאי מס' 1097. הנני נותן את חוות דעתי זו במקום עדות בשבועה בבית משפט. הדין של חוות דעת זו הוא כדין עדות בשבועה."
  }
}
```

This structure allows:

* Editing directly via `dev_text_modular`
* Dynamic placeholder filling (e.g. %דגם%, %שווי%, %ירידת ערך%)
* Multiple report generation in one session (if multiple types selected)

---

### 📥 Data Input Points by Source

| Field                            | Source                   | Notes                                   |
| -------------------------------- | ------------------------ | --------------------------------------- |
| Depreciation %                   | Depreciation UI          | Shared across all types                 |
| Value drop %                     | Estimate UI / Final UI   | Used by estimate, global, damaged\_sale |
| Sale price                       | Final UI                 | Used by damaged\_sale only              |
| Days in garage                   | Final UI                 | Used by global, damaged\_sale           |
| Compensation (פיצוי)             | Final Report Calculation | Legal field                             |
| Total damage + VAT               | Final Report Calculation | Always required                         |
| Damage percentage                | Final Report Calculation | Used in summary block                   |
| Car value for gross damage + VAT | Final Report Calculation | Used in most types                      |
| Report generation type(s)        | Final Report UI          | User can select 1-4 types               |
| Estimate Report edits            | Estimate Module          | Override draft unless invoice present   |

---

### 🧠 Estimate Report Module

* Optional step.
* Triggered manually after draft.
* Edits to any fields become new "truth" unless overwritten later.
* Shares same field structure.
* Lives in its own UI/module.
* Contains two types: אומדן ראשוני - אובדן להלכה, אומדן ראשוני - טוטלוס

---

### 📘 Dev\_Text\_Modular (Admin Bank)

* Central directory of all report type texts.
* Admin UI will:

  * List available types.
  * Allow editing title and content block.
  * Highlight required placeholders.

---

### ⚙️ Final Report Generator Logic

1. User selects report type(s) → required fields shown
2. System collects values from meta (including estimate/invoice if present)
3. System fills text vault anchor block accordingly
4. Report(s) are generated in parallel (PDF/DOC)
5. Each report uses same core layout + specific legal text

---

### 🛠️ Notes

* All texts are kept in **Hebrew** in vault.
* Changes to any text version take effect globally in next report.
* Estimate logic is completely isolated but affects downstream data.
* Each report type has a clear audit trail.

---

Ready to connect to generation logic and add override backdoor when requested.
