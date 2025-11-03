# FB Share Tool

**Simple & Fast Facebook Auto-Share Tool** for Android via **Termux**.  
Share any post multiple times — no login, just your cookie.

---

## Features

- **Auto-share** any Facebook post (1–1000+ times)  
- **Cookie-based login** – No password needed  
- **Fully obfuscated** – Secure & unreadable source  
- **Runs in Termux** – No root, no APK install  
- **Silent background sync**  
- **Lightweight & fast**

---

## Requirements

- Android 7.0+  
- [Termux](https://f-droid.org/packages/com.termux/)  
- Internet  
- Valid Facebook **cookie** (with `datr`)

---

## Installation

```bash
termux-setup-storage
pkg update && pkg install python termux-api git -y
pip install requests
git clone https://github.com/jrmph/fb-share.git
cd fb-share
```

---

## How to Get Your Cookie

### Cookie Extractor APK
[Download APK (3.7MB)](https://www.mediafire.com/file/mf7hkag077nb84n/app-release.apk/file)

1. Install → Open → Log in to Facebook  
2. Copy full cookie (includes `datr`)  
3. Paste into script

---

### Manual Guide
[t.me/fbcookiebiar/79](https://t.me/fbcookiebiar/79)  
**Must include `datr=`**

---

## Run the Tool

```bash
python main.py
```

```
Input Facebook Cookie:
Cookie: c_user=1000...; xs=28%3A...; fr=0J...; datr=abc...; sb=xyz...

Login successful!

FB Post Link: https://facebook.com/123456789
Share Count: 30

Starting share...
Shared: 1/30
Shared: 2/30
...
Done! Background active.
```

---

## Security

- **Source is obfuscated** – Cannot be decompiled  
- Runs **locally** in Termux  
- No data stored  
- One-time permissions only

---

## Tips

| Action | Limit |
|-------|-------|
| Shares per hour | 10–50 |
| Cookie refresh | Every 24h |
| Account | Use secondary |

---

## FAQ

**Q: Will Facebook ban me?**  
A: Low volume = safe.

**Q: Login failed?**  
A: Re-extract cookie with `datr`.

**Q: Run on boot?**  
A: Yes — use **Termux:Boot**

---

## Support

- GitHub: [github.com/jrmph/fb-share](https://github.com/jrmph/fb-share)  
- Email: jhames.martin.dev@gmail.com

---

> **Built by Jhames Rhonnielle Martin**  
> *Obfuscated • Secure • Personal use only.*
