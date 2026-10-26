# מכירות — KPI לנציג שטח

שלושה כרטיסי KPI ב‑RTL בעיצוב SAP Horizon, כל אחד 450×320 עם רקע לבן. כל קובץ עצמאי — נפתח ישירות בדפדפן.

| קובץ | תוכן |
| --- | --- |
| `InsightsKPI.html` | תובנות: קצב מכירות, הפסד מכירות פוטנציאלי, לקוחות באיחור (לחיצה → Account List) |
| `SalesForecastKPI.html` | מד מכר מול תחזית + % עמידה + פער; אייקון דריל / דאבל‑קליק פותח פירוט לפי נקודות מכירה |
| `VisitKPI.html` | סטטוס ביקורים (8/5/3) + קצב נדרש ליום; אייקון דריל → Visit List |

## ניווט

הדריל ב‑VisitKPI וב‑InsightsKPI שולח `postMessage` לחלון האב:

```js
{ operation: "navigation", params: { routingKey: "visit" | "account", viewType: "list" } }
```

הניווט פועל רק כשהכרטיס מוטמע בדף שמאזין להודעה.

כל הערכים הם נתוני הדגמה.
