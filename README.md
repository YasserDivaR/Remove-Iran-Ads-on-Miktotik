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

  <p>این پروژه به شما کمک می‌کند تا تبلیغات داخلی، پاپ‌آپ‌های مزاحم و ردیاب‌های ایرانی (مثل Tapsell, Parspack, Mihanblog و غیره) را در سطح شبکه مسدود کنید — بدون نیاز به نصب اپلیکیشن یا روت کردن دستگاه.</p>
</div>

---

## 🌐 خلاصه پروژه

 اسکریپت **Remove Iran Ads on Miktotik** یک اسکریپت آماده برای **روتر میکروتیک (MikroTik RouterOS)** است که با استفاده از **DNS Static**، دامنه‌های تبلیغاتی ایرانی را به `127.0.0.1` هدایت می‌کند و آن‌ها را به‌طور کامل مسدود می‌کند.

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
add name=ads.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=adspayamak.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.payamak-panel.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=adspopup.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=adserv.parspack.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=adserve.parsiblog.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.irancell.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=adsl.tci.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.mihanblog.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ad.mihanblog.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.blogsky.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ad.blogsky.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.parsijoo.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ad.saba.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.samsung.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=adserv.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=adnetwork.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=adnet.biz type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=irads.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=adclick.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=clickads.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=advertising.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=adserv.parsiblog.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=adserver.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"

# ----------------------------
# ردیاب‌های ایرانی
# ----------------------------
add name=analytics.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=stats.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=stat.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=track.parspack.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=click.parspack.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=counter.mihanblog.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=hit.mihanblog.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=visit.b92.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"

# ----------------------------
# تبلیغات درون‌برنامه‌ای (مثل Tapsell)
# ----------------------------
add name=ads.tapsell.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=tapsell.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.tapsellplus.ir type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=tapsell.net type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=adsterra.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.adsterra.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.supersonicads.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.revcontent.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.exoclick.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.popads.net type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=cdn.adtrue.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.adtrue.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
add name=ads.midas-network.com type=A address=127.0.0.1 ttl=1w comment="iran-ads"
```
اگر می‌خوای همه رو یک‌دفعه حذف کنی:
```
/ip dns static remove [find comment="iran-ads"]
```

# Fork کن → تغییرات اعمال کن → Pull Request بفرست

📬 ارتباط با من :

📧 ایمیل: YasserDivar@gmail.com

💬 تلگرام: @yasserdivar

🐦 وبسایت: yasserdivar.ir


<div align="center">
<p>ساخته شده با ❤️ برای مردم ایران</p>
  <img src="https://placehold.co/600x100/e11d48/ffffff?text=YasserDivar.ir" alt="YasserDivar.ir" />
</div>
