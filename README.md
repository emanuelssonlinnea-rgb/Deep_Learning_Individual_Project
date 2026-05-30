# Utforskning och fördjupning i neurala nätverk

## Introduktion

Projektet går ut på att använda neurala nätverk för att bygga en modell som kan klassificera ansiktsuttryck från bilder.

Det innebär att modellen ska:
- lära sig från bilddata
- skilja mellan olika ansiktsuttryck
- göra prediktioner på nya bilder
  
Målet är inte bara att få hög accuracy, utan att förstå hur olika val i modellen påverkar resultatet.

## Dataset

- Datasetet innehåller 35,887 gråskaliga bilder där varje bild representeras i 48 x 48 pixels var.
- Datasetet är redan indelat i train-set: 28,709 bilder, och test-set: 7,178.
- Det finns 7 klasskategorier (labels). Varje label representerar vilken sorts ansiktsuttryck bilderna hamnar inom.
- Klass kategorierna är: angry, disgust, fear, happy, neutral, sad, surprise.

## Modeller som byggts

- Baseline CNN: ~39% validation accuracy
- Improved CNN: ~38% validation accuracy  
- Transfer Learning (MobileNetV2): ~44% test accuracy

## Setup

pip install tensorflow keras numpy pandas matplotlib scikit-learn

## Projekt Struktur

├── notebooks/
│   └── facial_expression_recognition.ipynb
├── models/          # sparade modeller (not tracked by git)
├── data/            # dataset (not tracked by git)
└── README.md

## Hur man kör projektet

### 1. Klona repositoryt

```bash
git clone https://github.com/emanuelssonlinnea-rgb/Deep_Learning_Individual_Project.git

cd Deep_Learning_Individual_Project

python -m venv .venv
.venv\Scripts\activate

pip install -r requirements.txt

```

### Öppna filen
report.ipynb

Miljö: Python 3.13.7 "# Deep_Learning_Individual_Project"
