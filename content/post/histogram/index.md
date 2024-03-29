---
weight: 100
title: "ההיסטוגרמה - כל מה שרציתם לדעת ועוד קצת"
#title_align: "left"
summary: "דיון מעמיק בהיסטוגרמה, איך היא עובדת בדיוק ומה אפשר ללמוד ממנה"
date: 2020-09-01
draft: false

authors: 
  - admin

profile: false

# taxonomies
categories: 
  - "מושגים"

# tags:
#   - "Photos"
#   - "Game"
#   - "React"
#   - "Python"
#   - "New"

featured: true

---


בכל המצלמות המקצועיות וברוב כלי העריכה, כמו לייטרום ופוטושופ, קיימת אפשרות להציג היסטוגרמה של התמונה.
במצלמות Mirrorles ובמצלמות DSLR במצב Live View, ניתן אפילו לעשות זאת בזמן אמת, לפני שמצלמים את התמונה.
שימוש נכון בהיסטוגרמה, הן בשטח, בזמן הצילום, והן בשלב עיבוד התמונה, יכולים לעזור בשיפור משמעותי של התוצאה הסופית. 
  
<br/>

# מה זו היסטוגרמה?
למי שהספיק לשכוח את החומר מהתיכון נזכיר שהיסטוגרמה, במובן הכללי, היא גרף שמראה קשר בין שני משתנים כלשהם.
למשל הקשר בין הטמפרטורה הממוצעת לחודש בשנה, בירושלים:
{{< chart data="chart" >}}
  
<br/>

# מה זו היסטוגרמה בצילום?
בתחום הצילום, ההיסטוגרמה היא גרף שמציג את כמות הפיקסלים בתמונה בדרגות הבהירות שונות.
ציר ה-X (האופקי) מייצג את רמת הבהירות וציר ה-Y (האנכי) מייצג את כמות הפקסלים בתמונה. לכן, בצד השמאלי של ההיסטוגרמה
יוצגו הפיקסלים הכהים ביותר וככל שנלך ימינה על ציר ה-X ייוצגו פיקסלים בהירים יותר ויותר עד לפיקסלים הבהירים ביותר
שיוצגו בקצה הימני של ההיסטוגרמה. ככל שיש יותר פיקסלים באותה רמת בהירות כך הקו המשורטט יהיה גבוה יותר. לדוגמא:  

| {{< figure src="milkyway.jpg" width=300 >}} {{< figure src="milkyway-hist-bw.png" width=300 title="תמונה 1" >}}	|	{{< figure src="iceland.jpg" width=300 >}} {{< figure src="iceland-hist-bw.png" width=300 title="תמונה 2" >}}	|
|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|

תמונה 1 צולמה בלילה, רוב הפיקסלים הם כהים, לכן גרף ההיסטוגרמה מציג פיסגה בגרף בצד שמאל, שכזכור מייצג פיקסלים כהים.
תמונה 2 צולמה בסופת שלג באיסלנד ובה רוב הפיקסלים הם בהירים ולכן יש פסגה בגרף בצד ימין של ההיסטוגרמה.

{{% callout note %}}
חשוב לציין שהיסטוגרמות יכולות להיות קיצוניות, כמו בדוגמאות האלה, ועדיין להיות תקינות לחלוטין כיוון שהן משקפות נאמנה את הסצינה. 
{{% /callout %}}
  
<br/>

# מה אפשר ללמוד מההיסטוגרמה?
בעת הצילום יש להיסטוגרמה שני שימושים עיקריים:  
השימוש הראשון הוא מניעת [קטימה](#קטימה---clipping) (Clipping) לא רצויה  של האזורים הבהירים והכהים בסצינה.
[הטווח הדינמי](/dictionary#טווח-דינמי---dynamic-range) של כל מצלמה הוא מוגבל לכן סצינות עם קונטרסט גבוה, כמו תמונות נוף באור יום, עלולות לחרוג מהטווח הזה.
כאשר מתרחשת קטימה, כל הגוונים הבהירים, שמחוץ לטווח הדינמי, ירשמו כלבנים לגמרי, ובאופן שקול, הגוונים הכהים, שמחוץ לטווח הדינמי, ירשמו כשחורים לגמרי.
כיוון שהמידע הזה לא נרשם לקובץ התמונה אין אפשרות להחזיר אותו בשלב העריכה והוא אובד לנצח. קטימה באופן כללי, ובפרט של הגוונים הבהירים,
נוטה לפגוע באיכות התמונה ולכן חשוב להמנע ממנה ככל האפשר. מצבים בהם מתרחשת קטימה יוצגו בהיסטוגרמה כקפיצה בקצוות הגרף.
לדוגמה:
|  {{< figure src="horses-dark.jpg" width="800" >}} {{< figure src="horses-dark-hist.png" width="800"  title="תמונה 1" >}} | {{< figure src="horses-light.jpg" width="800" >}} {{< figure src="horses-light-hist.png" width="800" title="תמונה 2" >}} |
|:------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------:|

הסצנה שבצילום חורגת ממגבלות הטווח הדינמי של המצלמה. תמונה 1 נחשפה עבור האזורים הבהירים ביותר בשמיים (העננים) אבל אז האזורים הכהים,
כמו ראש הסוס, יצאו שחורים לגמרי ואיבדו את המידע שהיה בהם, ניתן לראות זאת לפי הקו הדק הצמוד לקצה השמאלי של ההיסטוגרמה.
לעומת זאת, תמונה 2 נחשפה עבור האזורים הכהים של הסצנה. בתמונה זו ניתן לראות את כל הפרטים באזורים הכהים אבל האזורים הבהירים
נקטמו ואיבדו מידע, ניתן לראות זאת לפי הפסגה הצמודה לצד הימני של ההיסטוגרמה.
<a name="dybamic_range_exceeded"></a>
  
חשוב להבין שבכל סצנה שבה הניגודיות חורגת מהטווח הדינמי של החיישן אין דרך להמנע מקטימה ע"י שינוי הגדרות החשיפה. 
ניתן בכל זאת להתגבר על מגבלות הטווח הדינמי בכמה שיטות:

1. לצלם מספר חשיפות עם נתונים שמתאימים לאזורים הבהירים והכהים של התמונה (Bracketing) ולחבר אותן אח"כ בשלב העריכה.
   כל המצלמות המקצועיות וחצי מקצועיות מאפשרות לבצע Bracketing אוטומטי וזו הגישה המועדפת עלי כיוון שהיא אוספת את כל המידע מהסצנה
   ומאפשרת לערוך את התמונה אח"כ בכל דרך שנבחר. אפשר לראות את תוצאת החיבור בהמשך המאמר. החסרונות של שיטה זו הם שהיא מתאימה בעיקר לסצינות סטטיות,
   בהן אין תנועה בין תמונה לתמונה, וכדי לקבל תוצאה מושלמת כדאי לצלם עם חצובה. אבל החיסרון העיקרי שהיא דורשת עבודת עריכה יותר מאומצת.
2. להשתמש בפילטר כהה מדורג Graduated Neutral Density / GND. פילטרים מסוג זה הם כהים בחלקם העליון ושקופים בחלקם התחתון.
   כיוון שהאזורים הבהירים הם בדרך כלל בשמיים הפילטר מכהה אותם ובכך מקטין את הטווח הדינמי של הסצנה ומאפשר למצלמה לקלוט את כולו.
   החסרונות של שיטה זו הם רבים, ראשית מדובר בציוד יקר וכבד למדי, סט של פילטרים עם התושבת יכול לשקול כחצי קילו ולעלות כמה אלפי שקלים.
   שנית, המעבר בין האזור הכהה, בין אם הוא חד או מדורג, הוא תמיד ישר אבל הטבע בדר"כ לא משתף פעולה וכמעט תמיד יש איזה הר או עץ שבולט עמוק לתוך השמיים.
   שלישית והכי חשוב, כיוון שהפילטר מקטין את הטווח הדינמי של הסצנה, בפועל מתרחש אובדן מידע ביחס למידע הקיים בסצנה המקורית.
3. בחירה מושכלת איזה קצה של הטווח הדינמי לקטום. בדר"כ עדיף לקטום את הכהים ובסצנות בהן הניגודיות גדולה רק במעט מהטווח של החיישן זה יכול להספיק.

השימוש השני מתאים לסצינות בהן הניגודיות קטנה מהטווח הדינמי ומטרתו לאסוף מידע רב ככל הניתן מהסצנה לצורך עריכה אח"כ.
לשם כך ניתן להשתמש בטכניקה שנקראת חשיפה לימין (Expose To The Right) או ETTR בקיצור ועליה [נרחיב במאמר נפרד](/post/ettr/).
<br/>  
  
# היסטוגרמה צבעונית
לצורך הפשטות, בכל הדוגמאות שלמעלה הצגתי את ההיסטוגרמה המונוכרומטית, שמתייחסת רק לרמות הבהירות הכלליות של התמונה ומתעלמת מהצבעים.
בתמונה צבעונית קיימות למעשה שלוש היסטוגרמות שונות, אחת לכל אחד מצבעי היסוד. ברוב המצלמות ותוכנות העריכה הן מוצגות אחת על גבי השניה בדיאגרמה אחת.
בהיסטוגרמה כזו כל אחד מצבעי היסוד מיוצג בעזרת ההיסטוגרמה בצבע שלו ואזורי חפיפה מיוצגים ע"י סכום הצבעים. לדוגמה:
|  {{< figure src="horses-comp.jpg" width="800" >}} {{< figure src="horses-comp-hist.png" width="800" >}} | {{< figure src="color-wheel.png" width="800" title="סכומי הצבעים" >}} |
|:-------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------:|
  
<br/>

# כשההיסטוגרמה משקרת
אני מקווה שמי שהגיע עד כאן השתכנע שההיסטוגרמה היא כלי חשוב ושימושי לכל צלם, ובפרט לצלמי טבע ונוף, הבעיה היחידה היא שהיא משקרת... טוב לא ממש אבל קצת כן...  

### ההיסטוגרמה לא לינארית
מההסברים שלמעלה יהיה סביר להניח שההיסטוגרמה היא לינארית, כלומר לכל אחת מרמות הבהירות האפשריות יש קו
אנכי בהיסטוגרמה שמייצג כמה פיקסלים יש בתמונה באותה רמת בהירות. בפועל זה לא המצב.

#### בציר ה-Y
הגובה של הקווים מייצג כמה פיקסלים ישנם בתמונה באותה רמת בהירות. זה נכון אבל הסקלה של ציר ה-Y מותאמת באופן דינמי לעמודה הגבוהה ביותר.
לכן, בכל היסטוגרמה, תמיד תהיה לפחות עמודה אחת שנוגעת בקצה העליון. כל שאר העמודות מחושבות באופן יחסי לאותה עמודה.
כלומר, גובה העמודות בהיסטוגרמה משמעותי רק ביחס לעמודות האחרות באותה היסטוגרמה ואי אפשר ללמוד כלום מהשוואת גבהים בין שתי הסטוגרמות שונות.

#### בציר ה-X
כאן המצב הרבה יותר מסובך.  
כזכור המצלמה מקודדת כל פיקסל בעזרת שלושה ערכים המודדים את הבהירות של אחד משלושת צבעי היסוד RGB. 
לצורך הדיון נניח שהמצלמה מקודדת כל צבע בעזרת 8 ביטים של מידע המאפשרים לייצג 256=2<sup>8</sup> רמות של בהירות.
כמו כן חיישן המצלמה מודד אור באופן לינארי, כלומר אם פיקסל A בהיר פי שתיים מפיקסל B אז ערכו המספרי של פיקסל A יהיה כפול מפיקסל B.
באופן אינטואיטיבי היינו מצפים שההיסטוגרמה תורכב מ-256 עמודות, אחת לכל רמת בהירות באופן לינארי שתואם את האופן בו החיישן קולט את האור.
אם זה היה המצב אז אם היינו לוקחים תמונה עם פיסגה בקצה הימני של ההיסטוגרמה, באזור של רמת בהירות 255, ומורידים ממנה f-stop אחד,
כלומר חותכים את רמת הבהירות שלה בחצי, היינו מצפים שההיסטוגרמה תזוז לאמצע, לאזור של רמת בהירות 128. ואם היינו מורידים תחנת צמצם נוספת היינו מצפים שהפסגה תזוז לאזור ה-64 וכן הלאה.   
השירטוט הבא מדגים את הנקודות בהן היינו מצפים לראות פסגות של ההיסטוגרמה עבור סידרת תמונות בהפרשי חשיפה של f-stop אחד, אם ההיסטוגרמה היתה לינארית:
{{< chart data="linear-hist" >}}

הדוגמה שלמטה מראה שלא זה מה שקורה:

<div class="table-grey table-headless table-borderless" ></div>

| x | y |
|:---------------:|:-------------------:|
| {{< figure src="white-wall-1.jpg" width="300" >}} | {{< figure src="white-wall-1-hist.png" width="300" >}} |
| {{< figure src="white-wall-2.jpg" width="300" >}} | {{< figure src="white-wall-2-hist.png" width="300" >}} |
| {{< figure src="white-wall-3.jpg" width="300" >}} | {{< figure src="white-wall-3-hist.png" width="300" >}} |
| {{< figure src="white-wall-4.jpg" width="300" >}} | {{< figure src="white-wall-4-hist.png" width="300" >}} |
| {{< figure src="white-wall-5.jpg" width="300" >}} | {{< figure src="white-wall-5-hist.png" width="300" >}} |
| {{< figure src="white-wall-6.jpg" width="300" >}} | {{< figure src="white-wall-6-hist.png" width="300" >}} |
| {{< figure src="white-wall-7.jpg" width="300" >}} | {{< figure src="white-wall-7-hist.png" width="300" >}} |
| {{< figure src="white-wall-8.jpg" width="300" >}} | {{< figure src="white-wall-8-hist.png" width="300" >}} |
  
<br/>  
  
כל התמונות בסדרה הן תמונות של אותו קיר לבן עם אותה תאורה וההבדל היחיד ביניהן הוא שינוי חשיפה של תחנת צמצם אחת בין כל זוג תמונות. כפי שניתן לראות, הגרף לא זז במידה שניתן היה לצפות ובנוסף גם הצורה של הפסגה משתנה, כך שהיא צרה בקצוות של ההיסטוגרמה ורחבה יותר באמצע. הסיבה לכך היא שההיסטוגרמה לא משקפת את הנתונים הגולמיים שנקלטו ע"י החיישן ונרשמו לקובץ ה-Raw אלא את הנתונים של קובץ ה-JPEG שנוצר לפי ההגדרות הנוכחיות של המצלמה. קובץ ה-JPEG אינו מכיל ייצוג פשוט של ערכי הבהירות אלא ערכים שעברו תיקון גמא (Gamma Correction). בתהליך הזה הנתונים הגולמיים שהחיישן מדד עוברים "תיקון" שמתאים לדרך בה בני אדם קולטים בהירות. בלי להכנס למה בדיוק עושה תיקון הגמא[^1] אפשר להגיד בקצרה שבסופו של התהליך המרחק בין תחנת צמצם אחת לבאה אחריה בהיסטוגרמה הוא פחות או יותר קבוע, כפי שאכן מודגם בסדרת התמונות שלמעלה.  

### מגבלות ה-JPEG
חיישנים מודרניים מקודדים את המידע שהם אוספים, המשקף את הטווח הדינמי, בעזרת 14 ביטים לכל צבע בכל פיקסל. כלומר, עבור כל אחד משלושת צבעי היסוד, החיישן מסוגל להבחין ב-2<sup>14</sup> שהם 16,384 דרגות בהירות, זה גם המידע שנשמר בקובץ ה-Raw. קבצי JPEG לעומת זאת מוגבלים ל-8 ביטים לכל צבע יסוד בכל פיקסל שהם 256 דרגות בהירות. בנוסף לכך ה-JPEG משקף גם את ה-Picture style / Creative style (כל יצרן קורא לזה אחרת) שנבחר במצלמה, כמו Portrait או Landscape. הפרופילים האלו, ביחד עם המגבלות הנובעות  עלולים להגדיל את הניגודיות עוד יותר 

{{% callout warning %}}
חשוב לציין שהמצלמה תשתמש בקובץ ה-JPEG להצגת ההיסטוגרמה אפילו אם ההגדרות הן שלא לשמור קובץ JPEG בכלל. אין דרך למנוע זאת.  
כתוצאה ממגבלות פורמט ה-JPEG, ומההמרות שקובץ ה-Raw עובר כדי להפוך ל-JPEG, עלול לקרות מצב שההיסטוגרמה תראה Clipping למרות שבפועל, בקובץ ה-Raw, הכל בסדר ולא התרחשה קטימה.  
כדי להמנע מכך ככל הניתן חשוב לבחור ב-Picture style עם קונטרסט נמוך ככל האפשר. במצלמות בהן ניתן לשלוט על הפרמטרים של ה-Picture style רצןי להגדיר Custom style עם הקונטרסט הנמוך ביותר שניתן להגדיר (בפרט אם ניתן להגדיר קונטרסט שלילי כדאי להשתמש בן). במצלמות בהן זה לא אפשרי ניתן לבחור בפרופיל Neutral. הגדרות אלו יעזרו לצמצם את המקרים בהם נקבל "התראת שווא" מההיסטוגרמה אבל בכל מקרה, לפחות בעיני, עדיפה התראה שווא על המצב ההפוך בו מתרחשת קטימה ללא התראה.
{{% /callout %}}


[^1]: מאמר בנושא בעתיד



