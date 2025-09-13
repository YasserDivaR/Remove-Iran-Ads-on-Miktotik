<div align="center">

  <img src="banner.svg" alt="Remove Iran Ads on MikroTik" width="800" />
</div>
  <h1>🚫 Remove Iran Ads on Miktotik</h1>
  <p><strong>یک راه‌حل قدرتمند برای مسدود کردن تبلیغات و ردیاب‌های ایرانی در شبکه (مخصوص روتر میکروتیک)</strong></p>
  
  <div>
    <img src="https://img.shields.io/badge/RouterOS-MikroTik-blue?logo=mikrotik" alt="MikroTik" />
    <img src="https://img.shields.io/badge/DNS-Blocking-green?logo=dns" alt="DNS Blocking" />
    <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License" />
    <img src="https://img.shields.io/badge/Contributions-Welcome-brightgreen" alt="Contributions Welcome" />
  </div>

  <p>این پروژه به شما کمک می‌کند تا تبلیغات داخلی، پاپ‌آپ‌های مزاحم و ردیاب‌های ایرانی (مثل Tapsell, Parspack, Mihanblog و غیره) را در سطح شبکه مسدود کنید بدون نیاز به نصب اپلیکیشن یا روت کردن دستگاه.</p>
</div>

---

## 🌐 خلاصه پروژه

 اسکریپت **Remove Iran Ads on MikroTik** یک اسکریپت آماده برای **روتر میکروتیک (MikroTik RouterOS)** است که با استفاده از **DNS Static**، دامنه‌های تبلیغاتی ایرانی را به `127.0.0.1` هدایت می‌کند و آن‌ها را به‌طور کامل مسدود می‌کند.

- ✅ بدون نیاز به نرم‌افزار روی دستگاه
- ✅ کار در سطح شبکه (همه دستگاه‌ها)
- ✅ مناسب برای خانه، اداره و کافی‌نت
- ✅ به‌روزرسانی دستی آسان
- ✅ پشتیبانی از فارسی و انگلیسی

---

## 🚀 قابلیت‌های اصلی

- 🔇 مسدود کردن تبلیغات درون‌برنامه‌ای (Tapsell, Adsterra)
- 🛑 بستن بنرهای وبلاگ‌های ایرانی (میهن بلاگ، بلاگ اسکای)
- 📵 قطع ارتباط با ردیاب‌های داخلی (Parspack, Irancell)
- 🌐 کار در تمام دستگاه‌ها (موبایل، تبلت، لپ‌تاپ)
- 💾 نیاز به فضای کم و مصرف منابع صفر
- 📝 کامنت‌گذاری شده و قابل ویرایش

---

## 📦 نحوه استفاده

1. به روتر میکروتیک خود وصل شوید (WinBox یا WebFig).
2. به مسیر زیر بروید:
IP → DNS → Static

3. 3. یا مستقیماً در **New Terminal** این اسکریپت را اجرا کنید:

```ros
/ip dns static
/ip dns static add name=adverge.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=yektanet.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=mediaad.org type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=popupdl.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=kaprila.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=sabavision.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=tavoos.net type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=chavosh.org type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=adtrace.io type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=pushe.co type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=sanjagh.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=najva.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=utop.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=vatanclick.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=sorenad.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=pelikan-network.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=yelloadwise.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=ylad.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=ads.karzar.net type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=adexo.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=binoads.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=yektabanner.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=dsp.aparat.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=adengine.telewebion.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=a-banners.divarcdn.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=adsc.beytoote.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=biz-cdn.varzesh3.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=biz.varzesh3.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=metrix.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=intrack.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=affilio.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=usermap.net type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=analyticsdaily.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=trustseal.e-rasaneh.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=bl9.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=analyt.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=sentry.sabaidea.cloud type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=tracker.digikala.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=new-sentry.digikala.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=sentry.theforge.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=analytics.zoomit.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=hadeseh.telewebion.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=sentry.alaatv.com type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=sentry.divar.cloud type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=candidatelogapi.jobvision.ir type=AAAA address=::1 ttl=1w comment="iran-ads"
/ip dns static add name=sentry.mci.dev type=AAAA address=::1 ttl=1w comment="iran-ads"
```
اگر می‌خوای همه رو یک‌دفعه حذف کنی:
```
/ip dns static remove [find comment="iran-ads"]
```

# Fork کن → تغییرات اعمال کن → Pull Request بفرست

📬 ارتباط با من :

📧 ایمیل: YasserDivar@gmail.com

💬 تلگرام: @yasserdivar

🐦 وبسایت: [yasserdivar.ir](http://yasserdivar.ir/)


<div align="center">
<p>ساخته شده با ❤️ برای مردم ایران</p>
  <img src="https://placehold.co/600x100/e11d48/ffffff?text=YasserDivar.ir" alt="YasserDivar.ir" />
</div>
