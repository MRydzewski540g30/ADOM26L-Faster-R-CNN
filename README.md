# Detekcja obiektów - Faster R-CNN (2015)
**Przedmiot:** Analiza Danych Obrazowych i Multimedialnych (ADOM 26L)

## Zespół
* **Theory Lead:** Piotr Markiewicz
* **Implementation Lead:** Mateusz Rydzewski
* **Experiments Lead:** Adam Mantiuk
* **Presentation/demo Lead:** Jakub Kołyska

## Opis repozytorium
Repozytorium zawiera zrefaktoryzowaną implementację modelu Faster R-CNN opartą na oficjalnym tutorialu PyTorch (Torchvision). Kod został przygotowany w sposób umożliwiający łatwe modyfikowanie hiperparametrów (m.in. progu IoU / NMS oraz rozmiarów kotwic) na potrzeby testów i ewaluacji.

## Instrukcja uruchomienia (Setup)

1. **Sklonuj repozytorium:**
   ```bash
   git clone [link_do_repo]
   ```

2. **Utwórz i aktywuj środowisko wirtualne:**
   
   **Windows:**
   ```powershell
   python -m venv venv 
   .\venv\Scripts\activate
   ```
   
   **Linux/MacOs:**
   ```bash
   python3 -m venv venv 
   source venv/bin/activate
   ```

3. **Zainstaluj wymagane biblioteki:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Uruchomienie modelu:**
   * Otwórz notatnik demonstracyjny/treningowy.
   * Zbiór danych (PennFudanPed) oraz skrypty pomocnicze pobiorą się automatycznie przy pierwszym uruchomieniu odpowiednich komórek.
   * **Dla Adama (Eksperymenty):** Parametry do testów (np. `box_nms_thresh`) zostały wyciągnięte do osobnych zmiennych na początku sekcji inicjalizującej model. Wystarczy zmienić wartość i kliknąć "Run All".