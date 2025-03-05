# 🚀 Disposable & Dangerous Email Domains List

This repository contains a curated list of temporary, disposable, and potentially dangerous email domains. The goal is to help developers, businesses, and security professionals filter out risky email addresses from their platforms.

## 📌 What is this list for?
- Blocking signups from temporary/disposable email providers.
- Preventing fraudulent activity by identifying suspicious domains.
- Enhancing security by reducing spam and abuse.

## 📥 Contributing
We welcome contributions! If you find a new disposable or dangerous email domain, please submit a pull request or open an issue.

### Steps to Contribute:
1. Fork this repository.
2. Add new domains to `domains.txt` (one per line, in lowercase).
3. Submit a pull request with a clear description of your additions.

## 📄 Usage
You can use this list in various ways:
- **Manually**: Download `domains.txt` and check against it in your application.
- **Automated Script**: Integrate with your backend to filter email addresses at registration.

### Example Usage in Python:
```python
with open("domains.txt") as f:
    blocked_domains = set(f.read().splitlines())

def is_blocked(email):
    domain = email.split("@")[1]
    return domain in blocked_domains

print(is_blocked("test@tempmail.com"))  # True if listed
```

## ⚠️ Disclaimer
This list is maintained to the best of our ability, but false positives or negatives may occur. Always validate based on your specific use case.

## 📜 License
This repository is licensed under the MIT License. Feel free to use, modify, and distribute it.

## ⭐ Support & Acknowledgments
If you find this project useful, consider giving it a ⭐ on GitHub!
