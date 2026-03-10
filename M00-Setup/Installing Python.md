# 01 — Install Python
### 🐍 Python Development | MCC BSIT 2526

[← Back to Setup Overview](./README.md)

---

Python is the programming language this entire course runs on. We need version **3.10 or higher**.

---

## 🪟 Windows

1. Go to 👉 [https://www.python.org/downloads/](https://www.python.org/downloads/)
2. Click the big yellow **"Download Python 3.x.x"** button
3. Run the downloaded `.exe` file
4. ⚠️ **CRITICAL — Before clicking anything else:**  
   Check the box that says **"Add Python to PATH"** at the bottom of the first screen

   ```
   ┌─────────────────────────────────────────┐
   │  Install Python 3.x.x                   │
   │                                         │
   │  ○ Install Now                          │
   │  ○ Customize installation               │
   │                                         │
   │  ☑ Add Python to PATH   ← CHECK THIS   │
   └─────────────────────────────────────────┘
   ```

   > ❌ If you skip this, Python will not work in the terminal and you will need to reinstall.

5. Click **"Install Now"**
6. Wait for the installation to finish
7. Click **Close**

### Verify

Open **Command Prompt** (search for `cmd` in the Start menu) and type:

```
python --version
```

Expected output:
```
Python 3.12.x
```

---

## 🍎 macOS

macOS may have an older Python pre-installed. We install the latest version separately.

1. Go to 👉 [https://www.python.org/downloads/](https://www.python.org/downloads/)
2. Click **"Download Python 3.x.x"**
3. Open the downloaded `.pkg` file
4. Follow the installer — click **Continue** and **Agree** through all steps
5. Click **Install** and enter your Mac password if prompted

### Verify

Open **Terminal** (search with Spotlight: `Cmd + Space`, type `Terminal`) and run:

```bash
python3 --version
```

Expected output:
```
Python 3.12.x
```

> 💡 On macOS, always type `python3` — not `python`. This is normal.

---

## 🐧 Linux (Ubuntu / Debian)

Most Linux systems already have Python. Check first:

```bash
python3 --version
```

**If you see Python 3.10 or higher** — you're done, skip to the next guide.

**If it's older or not found:**

```bash
sudo apt update
sudo apt install python3 python3-pip -y
```

### Verify

```bash
python3 --version
pip3 --version
```

Both should return version numbers with no errors.

---

## ❌ Common Issues

**"python is not recognized" (Windows)**  
You missed the "Add to PATH" checkbox. Uninstall Python from Control Panel, then reinstall and make sure to check it.

**"command not found: python3" (macOS/Linux)**  
Run `sudo apt install python3` (Linux) or reinstall from python.org (macOS).

**Wrong version showing (e.g. Python 2.7)**  
You have an old version. Install the latest from python.org — the new one will be used alongside the old one.

---

➡️ **Next:** [Install VS Code](./02-Install-VSCode.md)****
