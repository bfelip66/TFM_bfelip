Documentació del repositori de dades i codi
Títol del TFM: Estudi sobre la relació entre el creixement de l'extrema dreta i la violència contra les dones.
Aquest directori conté tot el material computacional, les dades originals i els models estadístics utilitzats per a la investigació de la relació entre l’indicador del vot a l'extrema dreta i els indicadors de violència masclista.
1. Estructura de la carpeta
•
/data: conté els conjunts de dades en format CSV.
o
inicials/: registres bruts sense processar.
o
finals/: inclou el fitxer rates_all_metrics_by_province_year_unified_final.csv, que és el dataset unificat i net utilitzat en els models definitius.
•
/notebooks: fitxers Jupyter Notebook (.ipynb) organitzats per etapes:
o
01_neteja_i_preparacio.ipynb
o
02_analisi_exploratoria_i_descriptiva.ipynb
o
03_models_Poisson_i_NB.ipynb
•
requirements.txt: llistat detallat de llibreries de Python i les seves versions.
2. Requeriments tècnics
L'anàlisi s'ha desenvolupat sota l'entorn Python 3.8.8. Per garantir la reproductibilitat dels resultats, es recomana seguir aquests passos:
1.
Instal·lar la versió de Python 3.8.8.
2.
Instal·lar les dependències mitjançant el gestor de paquets pip: pip install -r requirements.txt
3. Notes sobre la metodologia i estadística
S'han aplicat mètodes específics per abordar la naturalesa complexa de les dades:
•
Ajust FDR (False Discovery Rate): S'ha utilitzat en les correlacions de Pearson per controlar la taxa de falsos descobriments en comparacions múltiples.
•
Imputació LOCF (Last Observation Carried Forward): Aplicada en les visualitzacions temporals per garantir la continuïtat de les sèries per província.
•
Models d'Efectes Fixos: Utilitzats per explotar la variació within (intra-provincial) i aïllar els efectes de variables temporals i territorials constants.
4. Autoria i Contacte
Autora: Begoña Felip Bengochea
Data: Desembre 2025
