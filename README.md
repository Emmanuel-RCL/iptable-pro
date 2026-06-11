<div align="center">

# 🚀 RCL-IPtable Pro

### مدیریت حرفه‌ای، هوشمند و تعاملی فوروارد پورت‌های TCP/UDP در لینوکس

![Supported OS](https://img.shields.io/badge/OS-Ubuntu%20%7C%20Debian%20%7C%20AlmaLinux%20%7C%20RockyLinux-blue)

![Bash Version](https://img.shields.io/badge/Shell-Pure_Bash_4.0%2B-4EAA25?logo=gnu-bash\&logoColor=white)

![Root Required](https://img.shields.io/badge/Requires-Root-red)

مدیریت دستی `iptables` و خطر پاک شدن قوانین Docker؟

**RCL-IPtable Pro** اینجا است تا با یک رابط کاربری ساده و تعاملی، فورواردینگ پورت‌ها را برای چندین سرور مقصد، به امن‌ترین و سریع‌ترین شکل ممکن انجام دهد.

</div>

---

## ✨ ویژگی‌های کلیدی

* 🛡️ **ایمنی فوق‌العاده بالا**

  * استفاده از زنجیره اختصاصی `RCL_IPTABLE`
  * عدم تداخل با Docker، KVM، Virtualizor و فایروال پیش‌فرض سیستم

* 🌐 **مسیریابی چندگانه (Multi-Server)**

  * پشتیبانی از `TCP`
  * پشتیبانی از `UDP`
  * پشتیبانی هم‌زمان از `TCP + UDP`

* 🤖 **کشف هوشمند شبکه**

  * تشخیص خودکار اینترفیس اصلی
  * تشخیص خودکار MTU

* ⚡ **بهینه‌سازی شبکه**

  * فعال/غیرفعال‌سازی BBR
  * فعال/غیرفعال‌سازی FQ Queue
  * فعال/غیرفعال‌سازی MSS Clamping

* 📡 **مانیتورینگ زنده**

  * مشاهده تعداد Packetها
  * مشاهده میزان ترافیک عبوری
  * بروزرسانی خودکار

* 🩺 **Health Check**

  * بررسی قوانین DNAT
  * بررسی قوانین FORWARD
  * بررسی دسترسی سرور مقصد

* 🔄 **پایداری پس از ریبوت**

  * ذخیره خودکار تنظیمات
  * بارگذاری خودکار پس از راه‌اندازی مجدد

* 💾 **Backup & Restore**

  * تهیه نسخه پشتیبان
  * بازیابی کامل تنظیمات

* 🎯 **Conflict Detection**

  * تشخیص پورت‌های تکراری
  * پیشنهاد جایگزینی خودکار

---

## 🖥️ سیستم‌عامل‌های پشتیبانی‌شده

| توزیع       | نسخه‌های تست‌شده |
| ----------- | ---------------- |
| Ubuntu      | 22.04, 24.04     |
| Debian      | 11, 12           |
| AlmaLinux   | 8, 9             |
| Rocky Linux | 8, 9             |

---

## ⬇️ نصب و راه‌اندازی

اسکریپت به‌صورت خودکار نصب شده و به یک دستور سراسری در سیستم تبدیل می‌شود.

دستورات زیر را با دسترسی `root` اجرا کنید:

```bash
# Download Script
curl -Ls https://raw.githubusercontent.com/Emmanuel-RCL/iptable-pro/main/iptable-pro.sh -o iptable-pro.sh

# Make Executable
chmod +x iptable-pro.sh

# Run Installer
bash iptable-pro.sh
```

> پس از اولین اجرا، اسکریپت در مسیر `/usr/local/bin/rcl-iptable` نصب می‌شود و از این پس تنها کافی است دستور زیر را اجرا کنید:

```bash
rcl-iptable
```

---

## 🎮 نحوه استفاده

پس از نصب:

```bash
rcl-iptable
```

منوی تعاملی باز می‌شود و می‌توانید:

* افزودن Route جدید
* ویرایش Route
* حذف Route
* مانیتورینگ زنده
* تهیه Backup
* بازیابی Backup
* فعال‌سازی بهینه‌سازی‌های شبکه

را تنها با چند کلیک انجام دهید.

---

## ⚠️ هشدار ایمنی

* این اسکریپت فقط برای مدیریت Port Forwarding طراحی شده است.
* زنجیره‌های اصلی سیستم را Flush نمی‌کند.
* قبل از استفاده در محیط Production، تست در محیط آزمایشی توصیه می‌شود.
* اجرای برنامه نیازمند دسترسی `root` است.

---

## 📜 License

این پروژه تحت مجوز MIT منتشر شده است.

```text
MIT License
```

---

<div align="center">

Made with ❤️ by Emmanuel-RCL

</div>
