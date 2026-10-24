
##  node --version
- :מה הפקודה עושה
מציגה איזה גרסה מותקנת על המחשב
- :תוצאה
 v24.21.0
- עבד
 כן
- מה שיניתי
 כלום
- :אומת
  מותקן וניתן להריץ אותו

## npm install
-:מה הפקודה עושה
מורידה ומתקינה את הספריות שהפרויקט צריך
-עבד
כן
לא שיניתי כלום!
הופיעו אזהרות: 4 פגיעויות (1 moderate, 1 high, 2 critical), ואזהרה על esbuild@0.28.2. לא טיפלתי בהן כי הן לא מנעו את המשך ההרצה.

## npm test
-:מה הפקודה עושה
מריצה את בדיקות הקוד האוטומטיות של הפרויקט ובודקת שההתנהגות הקיימת עובדת כמצופה
-:הכלי שמריץ את הבדיקות
vitest
-:תוצאה
Test Files  1 passed (1)
Tests  5 passed (5)
-:עבד
כן, כל חמש הבדיקות עברו
-:קובץ הבדיקות
tests/event-api.test.ts
הבדיקות שרצו:
1. requires a demo photographer identity
2. lists only events belonging to the requested photographer
3. does not return another photographer's event
4. allows a client to submit a selection for their own gallery
5. does not let a client access a different client's gallery
-:מה שיניתי
כלום
-:מה אומת
הבדיקות הקיימות עוברות
-:מה לא אומת
בפלט לא הופיעה בדיקה של שינוי שם אירוע

## npm run typecheck
-:מה הפקודה עושה
בודקת שסוגי הנתונים בקוד תואמים זה לזה, בלי להריץ את המערכת ובלי ליצור קבצים
-:הפקודה שרצה בפועל
tsc --noEmit
-:תוצאה
לא הודפסו שגיאות אחרי השורה של הפקודה
-:עבד
כן.
-:מה שיניתי
כלום.
-:מה אומת
בדיקת הטיפוסים הסתיימה בלי שגיאות
-:מה לא אומת
לא נבדק איך המערכת מתנהגת בזמן ריצה. את זה בודקות הבדיקות והרצת השרת

## npm run dev

- מה הפקודה עושה:  
  מפעילה את שרת הפיתוח של המערכת ומשאירה אותו פועל

- הפקודה שרצה בפועל:  
  `tsx watch src/server.ts`

- תוצאה:
  `Event Photo API listening on http://localhost:3000`

- עבד:  
  כן, השרת עלה

- מה ניסיתי בדפדפן: 
  `http://localhost:3000`

- מה הופיע: 
  שגיאת 404 — הנתיב `/` לא נמצא.

- מה שיניתי:  
  הוספתי לכתובת את הנתיב `/health`:  
  `http://localhost:3000/health`

- תוצאה בבדיקה הנוספת:  
  `Status OK`

- מה אומת:  
  השרת עלה, והנתיב `/health` החזיר `Status OK`.

- מה לא אומת:  
  לא נבדקו כל נתיבי ה־API, ולא נבדקה האפשרות לשנות את שם האירוע.



