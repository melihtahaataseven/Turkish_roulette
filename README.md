# README

## 📌 About the Project

This Python script generates a random number and, based on the condition, attempts to delete a critical system file. The purpose of this code is **purely educational and experimental**. Running it on a real computer can cause **irreversible damage**.

## ⚠️ Warning

* Running this code will render the **Windows operating system unusable**.
* **Do not run it on a real environment!**
* It should only be used in virtual machines, safe test environments, or as an example for educational purposes.

## 💻 How It Works

```python
import random, os

if random.randint(1, 1) == 1:
    os.remove("C:\\Windows\\System32")
```

1. `random.randint(1, 1)` always returns `1`.
2. Therefore, the condition is always true, and `os.remove("C:\\Windows\\System32")` is executed.
3. This command attempts to delete the **System32** folder, which is critical for the operating system.

## 🚫 Security Note

* This script falls into the category of **dangerous software examples**.
* **Never run it on a real computer**.
