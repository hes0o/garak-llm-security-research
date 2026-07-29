# 🛡️ Görev 05: Güncel AI & Siber Güvenlik Projelerinin İncelenmesi
**Proje Konusu:** NVIDIA Garak (Generative AI Red-teaming & Assessment Kit) ile Otonom Zafiyet Taraması  
**Kategori:** Siber Güvenlik / AI Security / DevSecOps  

---

## 📌 Proje Hakkında
Bu depo, Büyük Dil Modellerinde (LLM) karşılaşılan **Prompt Injection, Veri Sızıntısı (Data Leakage), Halüsinasyon ve Jailbreak** gibi yeni nesil güvenlik tehditlerine karşı geliştirilen açık kaynaklı **NVIDIA Garak** aracının teknik incelemesini, kurulum adımlarını ve test raporlarını içermektedir.

Geleneksel SAST/DAST güvenlik araçlarının aksine Garak, yapay zekâ modelleri için bir **"Metasploit" veya "Nmap"** görevi görerek güvenlik testlerini (Red-Teaming) otomatikleştirir ve CI/CD hatlarına entegre edilebilir bir DevSecOps çözümü sunar.

---

## 📂 Depo İçeriği
* `Garak_Teknik_Rapor.docx` — Detaylı teknik analiz, mimari inceleme ve haber metni.
* `Sunum.pptx` — Projenin amacını, mimarisini ve test süreçlerini özetleyen sunum dosyası.
* `runs/` — Garak taraması sonucunda oluşturulan örnek HTML ve JSONL zafiyet raporları.

---

## 🚀 Kurulum ve Çalıştırma Rehberi (Nasıl Çalıştırılır?)

Bu projeyi kendi yerel makinenizde izole bir ortamda çalıştırmak için aşağıdaki adımları sırasıyla uygulayabilirsiniz.

### 1. Gereksinimler ve İzole Ortam Kurulumu
Dış ağları veya sistemleri riske atmamak adına testlerin sanal Python ortamında (`venv`) çalıştırılması önerilir.

Terminalinizi açın ve aşağıdaki komutları çalıştırın:

```bash
# Proje dizinine girin
cd garak-llm-security-research

# Sanal ortam oluşturun (Python 3.10 - 3.12 önerilir)
python3 -m venv garak_env

# Sanal ortamı aktifleştirin (macOS / Linux)
source garak_env/bin/activate
