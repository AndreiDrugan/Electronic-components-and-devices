# Local Python Assistant & Electronic Components Classifier

Un asistent local inteligent bazat pe Python care combină recunoașterea vizuală a componentelor electronice (prin rețele convoluționale avansate) cu o componentă de automatizare prin comenzi vocale (Whisper și procesare de intentii).

## Caracteristici principale

- **Clasificare Vizuală (Computer Vision):** Model bazat pe **EfficientNet-B2** fine-tunat pentru recunoașterea a **36 de clase** de componente electronice.
- **Pipeline de Date Robust:**
  - Încărcare automată din structura de directoare pe clase.
  - Împărțire stratificată în seturi de `Train`, `Validation` și `Test`.
  - Transformări avansate de **Data Augmentation** (rotații, flip-uri, ajustări de culoare, crop-uri aleatoare) pentru combaterea overfitting-ului.

## Tehnologii utilizate

- **Python 3.10+**
- **PyTorch & Torchvision** (Deep Learning & CNNs)
- **Scikit-learn** (Label encoding, metrici, split-uri și NLP pentru comenzi)
- **Pandas & NumPy** (Manipularea datelor tabulare)
- **Pillow (PIL)** (Procesare imagini)

Instalează dependențele:

pip install torch torchvision torchaudio scikit-learn pandas numpy pillow

Rulează antrenarea:
Deschide main.ipynb în Jupyter Notebook sau VS Code și rulează celulele secvențial pentru a pregăti dataset-ul, a configura transformările și a rula bucla de antrenare cu ReduceLROnPlateau.
