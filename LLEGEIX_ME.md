# Documentació del repositori de dades i codi

**Títol del TFM:** *Estudi sobre la relació entre el creixement de l'extrema dreta i la violència contra les dones*

Aquest repositori conté el material computacional, les dades originals i els models estadístics utilitzats per investigar la relació entre l’indicador de vot a l'extrema dreta i diversos indicadors de violència masclista.

## 1. Estructura del repositori

- `data/` — conjunts de dades en format CSV.
  - `inicials/` — registres bruts sense processar.
  - `finals/` — dades processades i preparades per a l’anàlisi.
    - `rates_all_metrics_by_province_year_unified_final.csv` — dataset unificat i net utilitzat en els models definitius.

- `notebooks/` — Jupyter Notebooks (`.ipynb`) organitzats per etapes:
  - `01_neteja_i_preparacio.ipynb`
  - `02_analisi_exploratoria_i_descriptiva.ipynb`
  - `03_models_Poisson_i_NB.ipynb`

- `requirements.txt` — llistat de llibreries de Python i versions.

## 2. Requeriments tècnics

L’anàlisi s’ha desenvolupat en un entorn **Python 3.8.8**. Per garantir la reproductibilitat dels resultats:

1. Instal·la **Python 3.8.8**.
2. Instal·la les dependències amb `pip`:

```bash
pip install -r requirements.txt
````

> [!NOTE]
> Si treballes amb entorns virtuals (recomanat), crea i activa l’entorn abans d’instal·lar les dependències.

---

## 3. Notes sobre metodologia i estadística

S’han aplicat mètodes específics per abordar la naturalesa de les dades i la robustesa dels resultats:

* **Ajust FDR (False Discovery Rate):** utilitzat en les correlacions de Pearson per controlar la taxa de falsos descobriments en comparacions múltiples.
* **Imputació LOCF (Last Observation Carried Forward):** aplicada en visualitzacions temporals per garantir la continuïtat de les sèries per província.
* **Models d’efectes fixos:** utilitzats per explotar la variació *within* (intra-provincial) i aïllar l’efecte de factors constants en el temps o territorials.

---

## 4. Autoria i contacte

* **Autora:** Begoña Felip Bengochea (bfelip@uoc.edu)
* **Data:** Desembre 2025
