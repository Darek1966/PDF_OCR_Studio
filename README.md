# 📄 PDF OCR Studio

## ℹ️ Opis projektu

**PDF OCR Studio** to aplikacja webowa zbudowana w technologii **Streamlit**, służąca do konwersji plików PDF do przeszukiwalnego tekstu z wykorzystaniem technologii OCR (Tesseract). Oferuje tłumaczenie z języka angielskiego na polski, podgląd miniatur stron, wybór zakresu stron, eksport do formatów **TXT, DOCX, PDF**, wyświetlanie metadanych dokumentu oraz prowadzenie historii konwersji. Projekt utrzymuje spójny i nowoczesny **ciemny motyw** z brandingiem *netdark_1966*.

---

## ✨ Funkcje

- 📥 **Wgrywanie PDF** i podgląd miniaturek stron
- 🔍 **OCR (Optical Character Recognition)** z wielojęzycznym wsparciem
- 🌐 **Tłumaczenie EN → PL** (deep_translator / Google Translate API)
- 🈶 **Auto-wykrywanie języka** w dokumencie
- 📋 **Wyświetlanie metadanych PDF** (tytuł, autor, data utworzenia, itp.)
- 💾 **Eksport wyników** do TXT, DOCX i PDF
- 🗂 **Historia konwersji** z możliwością czyszczenia
- 🎨 **Ciemny motyw** i nowoczesny interfejs użytkownika

## 🔧 Instalacja

### Wymagania wstępne

1. Python 3.8 lub nowszy
2. Tesseract OCR zainstalowany w systemie

### Instalacja Tesseract OCR

#### Windows

```bash
winget install -e --id UB-Mannheim.TesseractOCR
```

lub pobierz z [oficjalnej strony](https://github.com/UB-Mannheim/tesseract/wiki)

#### Linux (Ubuntu/Debian)

```bash
sudo apt-get update
sudo apt-get install tesseract-ocr
sudo apt-get install tesseract-ocr-pol tesseract-ocr-eng
```

### Instalacja aplikacji

1. Sklonuj repozytorium:

```bash
git clone https://github.com/Darek1966/PDF_OCR_Studio.git
cd PDF_OCR_Studio
```

2. Zainstaluj wymagane biblioteki:

```bash
pip install -r requirements.txt
```

3. Uruchom aplikację:

```bash
streamlit run app.py
```

## 📋 Użycie

1. Wgraj plik PDF za pomocą przycisku w lewym panelu
2. Zaznacz strony do przetworzenia
3. Wybierz opcje OCR i tłumaczenia
4. Kliknij "🚀 Uruchom OCR" i poczekaj na zakończenie procesu
5. Pobierz wyniki w wybranym formacie (TXT, DOCX, PDF)
6. Przeglądaj metadane dokumentu w panelu bocznym

## 🧰 Technologie

* **Python** - język programowania
* **Streamlit** - framework do tworzenia aplikacji webowych
* **PyMuPDF (fitz)** - biblioteka do obsługi plików PDF
* **Tesseract OCR** - silnik OCR do rozpoznawania tekstu
* **pytesseract** - wrapper Pythona dla Tesseract
* **deep_translator** - biblioteka do tłumaczenia tekstu
* **langdetect** - biblioteka do wykrywania języka
* **python-docx** - tworzenie dokumentów DOCX
* **reportlab** - generowanie plików PDF
* **PIL/Pillow** - przetwarzanie obrazów

## 📁 Struktura projektu

```
PDF_OCR_Studio/
├── app.py
├── requirements.txt
├── .streamlit/
│   └── config.toml
├── assets/
│   ├── icon.png
│   └── logo.png
├── history/
│   └── conversions.json   # tworzony automatycznie
├── output/                # tworzony automatycznie
└── README.md
```

## 🤝 Współpraca

Jeśli chcesz przyczynić się do rozwoju projektu:

1. Utwórz fork repozytorium
2. Stwórz nową gałąź dla swojej funkcji (`git checkout -b feature/amazing-feature`)
3. Zatwierdź zmiany (`git commit -m 'Dodano nową funkcję'`)
4. Wypchnij do gałęzi (`git push origin feature/amazing-feature`)
5. Otwórz Pull Request

## 📜 Licencja

Ten projekt jest udostępniany na licencji MIT. Szczegółowe informacje znajdują się w pliku LICENSE.

## 📞 Kontakt

[![Email](https://img.shields.io/badge/Email-Napisz%20do%20mnie-blue?style=for-the-badge&logo=gmail&logoColor=white)](mailto:netdark_1966@op.pl)

[![GitHub](https://img.shields.io/badge/GitHub-Darek1966-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Darek1966)

---
