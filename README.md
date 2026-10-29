# Prostorová analýza uliční sítě: Staré Město (Praha) pomocí OSMnx

Tento repozitář obsahuje semestrální projekt zaměřený na představení a praktickou demonstraci Python knihovny **OSMnx** pro modelování a analýzu prostorových sítí.

## Obsah projektu
- **Knihovna:** OSMnx (verze 2.x)
- **Zájmové území:** Staré Město, Praha
- **Hlavní soubor:** [`osmnx_stare_mesto.ipynb`](./osmnx_stare_mesto.ipynb) *(případně upravte název podle vašeho souboru)*

## Co projekt demonstruje
1. **Topologie a stahování dat:** Automatizované stažení pěší sítě z OpenStreetMap přes Overpass API a zjednodušení křižovatek.
2. **Převod datových struktur:** Transformace síťového multigrafu (`MultiDiGraph`) na GeoDataFrames (uzly a hrany) pro GeoPandas.
3. **Síťová analýza (Routing):** Nalezení nejkratší pěší trasy mezi Staroměstským náměstím a Karlovým mostem pomocí Dijkstrova algoritmu.
4. **Body zájmu (POIs):** Extrakce a vizualizace historických památek a kaváren na uliční síti.
5. **Diskuse limitů:** Zhodnocení závislosti na veřejných Overpass serverech (HTTP 502 chyby) a statické povahy modelu.

## Jak projekt spustit lokálně
Pro replikaci prostředí doporučujeme použít Conda / Mamba:

```bash
# Vytvoření a aktivace prostředí
conda create -n osmnx_project -c conda-forge osmnx jupyterlab matplotlib
conda activate osmnx_project

# Spuštění prostředí
jupyter lab
```
