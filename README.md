# Proxy Tester

A simple Python project for testing whether proxies are working or not. This tool checks proxy connectivity by sending a request through each proxy and showing whether the proxy is valid, failed, or timed out.

---

## 🚀 Features

* Test multiple proxies from a file
* Check whether each proxy is working
* Show success or failure status
* Display response status code
* Handle timeout and connection errors
* Easy to customize for HTTP and HTTPS proxies

---

## 🛠️ Tech Stack

* Python
* Requests library

---

## 📁 Project Structure

```bash
proxy-tester/
│
├── rotating_proxies.py
├── proxies.txt
├── final_proxies.txt
└── README.md
```

---

## 📦 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/proxy-tester.git
cd proxy-tester
```

Create a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 📄 proxies.txt Format

Add proxies inside `proxies.txt`, one proxy per line:

```text
http://proxy_ip:port
https://proxy_ip:port
http://username:password@proxy_ip:port
```

Example:

```text
http://123.45.67.89:8080
http://98.76.54.32:3128
https://45.67.89.10:3128
```

---

## ▶️ Usage

Run the script:

```bash
python main.py
```

The program will read proxies from `proxies.txt` and test each proxy.

---

## 🧠 How It Works

1. The program loads proxies from `proxies.txt`.
2. It sends a test request through each proxy.
3. If the request succeeds, the proxy is marked as working.
4. If the request fails or times out, the proxy is marked as failed.
5. Results are printed in the terminal.

---

## 🧪 Example Output

```text
Testing proxy: http://123.45.67.89:8080
✅ Working | Status Code: 200

Testing proxy: http://98.76.54.32:3128
❌ Failed | Connection timeout
```

---

## 📌 Requirements

Create a `requirements.txt` file:

```text
requests
```

Install it:

```bash
pip install -r requirements.txt
```

---

## ⚠️ Important Notes

* This project is only for checking proxy availability.
* Do not use proxies for spam, abuse, or illegal activity.
* Free proxies may be slow, unstable, or unsafe.
* Always use proxies responsibly and follow website terms of service.

---

## 🔮 Future Improvements

* Save working proxies to a separate file
* Add proxy speed testing
* Add country/IP information
* Add async proxy testing
* Add support for SOCKS proxies
* Export results to CSV

---

## 👨‍💻 Author

**Anuj Paroha**

GitHub: [77anuj77](https://github.com/77anuj77)

---

## ⭐ Support

If this project helped you, consider giving it a star.
