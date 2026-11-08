# فرآوریار — نسخه تحت وب | FaravariYar — Web Edition

<div dir="rtl">

**فرآوریار** ابزار آنلاین اطلاعات پروژه، انتخاب تجهیزات و محاسبات فرآوری مواد معدنی است — بازنویسی تحت وبِ اپلیکیشن دسکتاپ فرآوریار (PySide6). این نسخه **یک فایل HTML خودکفا** است؛ بدون نصب، بدون سرور و بدون وابستگی خارجی. کافی است `index.html` را در مرورگر باز کنید یا آن را با **GitHub Pages** میزبانی کنید.

</div>

**FaravariYar** is the web edition of the FaravariYar desktop toolkit (PySide6) for mineral-processing project data, equipment selection and calculations. It ships as **one self-contained `index.html`** — no install, no server, no external dependencies. Open the file in any modern browser, or host it free with **GitHub Pages**.

---

## ✨ امکانات | Features

<div dir="rtl">

- **ورود کاربران** با سطوح دسترسی ۱ تا ۵ (ادمین، مدیر، کارشناس، متفرقه، مهمان) — حساب‌های پیش‌فرض: `admin/admin` (ادمین اصلی) و `user/1` (کارشناس)
- **اطلاعات پروژه (INF)** — شناسنامه پروژه، ماده معدنی (عیار، چگالی، رطوبت، F80)، مهندس، سایت و ساعت کاری
- **انتخاب تجهیزات (EQP)** — کاتالوگ کامل تجهیزات فرآوری با پارامترهای قابل ویرایش
- **طراحی مدار (CRD)** — بوم تعاملی: جای‌گذاری تجهیز، اتصال جریان با درگ، ۹ نوع جریان رنگی (دوغاب، آب، هوای ابزار دقیق و…)، ویژگی هر تجهیز (ضریب خردایش، بازیابی و ضریب پرعیارسازی فلوتاسیون)، زوم و جابه‌جایی بوم
- **نمودار بلوکی BFD** — واحدهای اصلی فرآیند؛ واحدهای انتخابی، جعبه‌ابزار صفحه «طراحی مدار» را فیلتر می‌کنند؛ خروجی PNG
- **موازنه جرم جریان‌ها (MBT)** — تناژ از خوراک (جمع در ادغام، تقسیم مساوی در انشعاب)، آب از رطوبت و جریان‌های آب، عیار با مدل فلوتاسیون، دانه‌بندی با ضریب خردایش، درصد جامد خودکار؛ خروجی CSV
- **لیست تجهیزات (EQL)** با ستون‌های مدل/مشخصات/وزن/توان و خروجی CSV
- **شرح فرآیند (PRD)** — تولید خودکار متن از استریم‌های مدار + ویرایش آزاد
- **کدگذاری (COD)** — الگوی کد (ناحیه / اختصار / شماره / توالی)، جدول‌های ناحیه و اختصار قابل ویرایش، تخصیص کد بخش‌به‌بخش به تجهیزات مدار
- **مطالعات آزمایشگاهی (LAB)** — ۹ بخش با فرم کامل و جدول نتایج
- **محاسبات و سایزینگ (CAL)** — موازنه جرم دو محصول، حداقل جرم نمونه، توان آسیا (باند)، حجم سلول فلوتاسیون، قطر تیکنر، تعداد صفحات فیلتر پرس
- **مدارک مهندسی (ENG)** — لیست MDL + جدول دیسیپلین‌های استاندارد
- **مشاوران (CON)**، **نرم‌افزارها (SOF)**، **شرکت‌های معدنی (CMP)**، **کتابخانه مدل‌ها (LIB)**
- **پنل مدیریتی (ADM)** — مدیریت کاربران، حالت مهمان با سقف ورود و زمان جلسه، گزارش فعالیت با خروجی CSV
- **دو زبانه (فارسی/انگلیسی)** با چرخش کامل RTL/LTR، **تم روشن/تیره**، **۶ تم رنگی** و انتخاب فونت — ذخیره‌شده برای هر کاربر
- **ذخیره‌سازی محلی** در حافظه مرورگر (localStorage) + **پشتیبان‌گیری/بازگردانی JSON** و خروجی‌های CSV و PNG

</div>

English: bilingual FA/EN interface (full RTL), light/dark theme, 6 accent palettes, per-user preferences, login with 5 access levels and a guest mode, browser-local persistence with JSON backup/restore, CSV & PNG exports.

## 🚀 اجرا | Run

<div dir="rtl">

**محلی:** فایل `index.html` را باز کنید (دابل‌کلیک کافی است).

</div>

**Local:** just open `index.html` — everything (fonts included) is inside the file.

### 🌐 انتشار رایگان با GitHub Pages | Deploy on GitHub Pages

1. این پوشه را در یک مخزن گیت‌هاب قرار دهید — فایل‌ها باید در **ریشه مخزن** باشند (`index.html` کنار `README.md`):
   ```bash
   git init
   git add .
   git commit -m "FaravariYar web edition"
   git branch -M main
   git remote add origin https://github.com/<USERNAME>/<REPO>.git
   git push -u origin main
   ```
2. در گیت‌هاب: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / `(root)` → Save**
3. پس از یک تا دو دقیقه، برنامه روی `https://<USERNAME>.github.io/<REPO>/` در دسترس است.

(English: push these files to a repository root, then enable Pages from `main / (root)` — no build step is needed.)

## 🔑 حساب‌های پیش‌فرض | Default accounts

| حساب | رمز | سطح | توضیح |
|---|---|---|---|
| `admin` | `admin` | ۱ — ادمین اصلی | همه منوها + پنل مدیریتی + شرکت‌ها/کتابخانه |
| `user` | `1` | ۳ — کارشناس | کاربر عادی |
| `guest` | (از پنل ادمین) | ۵ — مهمان | پس از فعال‌سازی در پنل مدیریتی؛ با سقف ورود و زمان جلسه |

<div dir="rtl">

⚠️ **امنیت:** این نسخه کاملاً سمتِ کلاینت است؛ رمزها هش می‌شوند ولی احراز هویت واقعی سروری نیست. برای استفاده عمومی، صفحه Pages را خصوصی (private) نگه دارید یا رمزها را تغییر دهید.

</div>

⚠️ **Security note:** this is a fully client-side app; passwords are hashed but there is no server-side authentication. Change the default passwords and treat stored data as local to each browser.

## 💾 داده‌ها کجا ذخیره می‌شوند؟ | Where is the data?

<div dir="rtl">

همه چیز در `localStorage` مرورگرِ همان دستگاه ذخیره می‌شود (کلید `faravariyar_web_v1`). پاک کردن حافظه مرورگر = پاک کردن داده‌ها. برای انتقال پروژه بین دستگاه‌ها از دکمه‌های **پشتیبان‌گیری/بازگردانی JSON** در دیالوگ «پروژه‌ها» استفاده کنید.

</div>

Everything lives in the browser's `localStorage`. Use the **JSON backup / restore** buttons in the “Projects” dialog to move data between devices or browsers.

## 🔄 تفاوت‌ها نسبت به نسخه دسکتاپ | Differences from the desktop app

| ویژگی | دسکتاپ (PySide6) | وب |
|---|---|---|
| ذخیره‌سازی | SQLite داخلی | localStorage مرورگر |
| خروجی‌ها | Excel/CSV/DXF/PPTX/PNG | CSV / PNG / JSON |
| صفحات 3D و P&ID | فعال (v0.9) | جای‌نگه‌دار («نسخه بعد») |
| صفحات چندگانه مدار و فلش‌های بین‌صفحه‌ای | دارد | ندارد (نسخه بعد) |
| دسترسی مدیر/کارشناس به پروژه‌ها | تخصیص دقیق | همه پروژه‌ها برای همه سطوح قابل‌نویس دیده می‌شود |
| لوگوهای شرکت‌ها | فایل PNG | فقط نام‌ها |

## 🗂 ساختار مخزن | Repository layout

```
index.html    ← کل برنامه (HTML + CSS + JS + فونت‌ها در یک فایل)
.nojekyll     ← GitHub Pages فایل را دست‌نخورده سرو می‌کند
LICENSE       ← MIT
README.md     ← همین راهنما
```

## 🛠 فناوری | Tech

<div dir="rtl">

جاوااسکریپت خالص (بدون هیچ کتابخانه یا build)؛ رابط دو زبانه با متغیرهای CSS؛ بوم طراحی با SVG + DOM؛ موازنه جرم پورت‌شده از `app/modules/balance.py` دسکتاپ؛ فرمول‌ها از `app/modules/calcs.py`. فونت **وزیرمتن** (SIL OFL 1.1) و **بی‌تیتر** داخل فایل embed شده‌اند تا متن فارسی همیشه درست نمایش داده شود؛ فونت‌های بی‌نازنین/بی‌زر/بی‌میترا در صورت نصب بودن روی سیستم استفاده می‌شوند.

</div>

Vanilla HTML/CSS/JS — no framework, no build step, no network calls. The mass-balance engine is a direct port of the desktop `balance.py`; formulas follow `calcs.py`. Vazirmatn (SIL OFL 1.1) and B Titr are embedded as base64 so Persian renders everywhere; B Nazanin / B Zar / B Mitra are used when installed locally.

## 📄 مجوز | License

MIT — see `LICENSE`. Fonts keep their own licenses (Vazirmatn: SIL OFL 1.1).
