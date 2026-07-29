# 🛡️ Görev 05: Güncel AI & Siber Güvenlik Projelerinin İncelenmesi
**Proje Konusu:** NVIDIA Garak (Generative AI Red-teaming & Assessment Kit) ile Otonom Zafiyet Taraması  
**Kategori:** Siber Güvenlik / AI Security / DevSecOps  

![Security](https://img.shields.io/badge/Security-AI%20Red--Teaming-red?style=for-the-badge)
![DevSecOps](https://img.shields.io/badge/DevSecOps-Automated%20Scanning-blue?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.10%20%7C%203.11%20%7C%203.12-yellow?style=for-the-badge)

---

## 📌 Proje Hakkında
Bu depo, Büyük Dil Modellerinde (LLM) karşılaşılan **Prompt Injection, Veri Sızıntısı (Data Leakage), Halüsinasyon ve Jailbreak** gibi yeni nesil güvenlik tehditlerine karşı geliştirilen açık kaynaklı **NVIDIA Garak** aracının teknik incelemesini, kurulum adımlarını ve test raporlarını içermektedir.

Geleneksel SAST/DAST güvenlik araçlarının aksine Garak, yapay zekâ modelleri için bir **"Metasploit" veya "Nmap"** görevi görerek güvenlik testlerini (Red-Teaming) otomatikleştirir. CLI (Komut Satırı Arayüzü) üzerinden çalıştığı için CI/CD hatlarına entegre edilebilir bir DevSecOps çözümü sunar.

---

## 📂 Depo İçeriği
* `Garak_Teknik_Rapor.docx` — Detaylı teknik analiz, mimari inceleme ve haber metni.
* `Sunum.pptx` — Projenin amacını, mimarisini ve test süreçlerini özetleyen sunum dosyası.
* `runs/` — Garak taraması sonucunda oluşturulan örnek HTML ve JSONL zafiyet raporları.

---

## ⚡ Hızlı Başlangıç ve Çalıştırma Rehberi (Quickstart)

Projeyi kendi ortamınızda çalıştırmak için aşağıdaki adımları terminalinizde sırasıyla uygulayabilirsiniz.

### 1️⃣ Sanal Ortam Kurulumu ve Aktivasyonu (Environment Activation)
Dış ağları veya sistemleri riske atmamak ve bağımlılık çakışmalarını önlemek adına testler sanal Python ortamında (`venv`) çalıştırılmıştır:

```bash
# Proje dizinine girin
cd garak-llm-security-research

# Sanal Python ortamını oluşturun (Python 3.10 - 3.12 önerilir)
python3 -m venv garak_env

# Sanal ortamı AKTİF EDİN (macOS / Linux)
source garak_env/bin/activate
