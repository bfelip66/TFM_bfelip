# Treball final del màster de Data Science

---

## Descripció
El projecte que aquí és presenta com a treball final de màster (TFM) és un estudi sobre la possible relació causal entre el creixement de l'extrema dreta i la violència contra les dones a Espanya (2014-2023). La investigació utilitza evidència estadística i models de dades de panell (FE) per desmuntar narratives i analitzar punts d'inflexió institucionals.

El projecte s'ha desenvolupat íntegrament en Jupyter Notebook (Python) i inclou un **[informe analític visual](./Informe_analitic_visual_TFM_Bfelip.pdf)** dissenyat per recórrer l'estudi d'una manera seqüencial i entenedora. L'anàlisi combina el rigor dels models de recompte amb una narrativa visual accessible per a la transferència de resultats.

---

## Estructura del Git

Per facilitar la navegació pel repositori, el contingut s'organitza de la següent manera:

```text
.
├── Informe_analitic_visual_TFM_Bfelip.pdf             # Síntesi visual dels resultats i transferència.
├── requirements.txt                                   # Dependències de Python (pandas, statsmodels, etc.).
├── license                                            # Llicència d'ús del projecte.
├── LLEGEIX_ME.md                                      # Documentació de l'organització (aquest fitxer).
├── 📁 dades/
│   ├── 📁 originals/                                  # Fitxers de les fonts originals (INE, CGPJ, Ministeris).
│   └── 📁 processades/                                # Dataset unificat i depurat per a l'anàlisi.
└── 📁 notebooks/
    ├── 01_neteja_i_preparacio.ipynb                    # Execució de l'ETL i fusió de fonts.
    └── 02_analisi_exploratoria_i_descriptiva.ipynb     # Models FE, ITS i visualitzacions.

```
---

## Autoria
* Autora del TFM: Begoña Felip Bengochea
* Directora del TFM: Anna Muñoz Bollas
* Professora responsable de l'assignatura: Susana Acedo Nadal
