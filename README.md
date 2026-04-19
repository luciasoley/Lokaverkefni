# Vatnafræðileg greining á Markarfljóti við Emstrur

Þetta repository inniheldur kóða fyrir greiningu á rennsli, árstíðabundnu flóðamynstri og flóðatíðnigreiningu fyrir Markarfljót (ID 66).

## Gögn
Verkefnið notar gögn úr **LamaH-Ice** gagnasafninu:
* `ID_66.csv`: Veðurgögn.
* `ID_66_q.csv`: Rennslisgögn.

## Uppbygging möppu
* **data/**: Inniheldur sótt gögn og útreiknaðar niðurstöður í .csv sniði.
* **figures/**: Myndrit sem sýna langæislínur, leitni (trend) og flóðatburði.
* **scripts/**: Jupyter Notebook (`greining.ipynb`) sem geymir allan kóðann.

## Hvernig keyra má kóðann
1. Gakktu úr skugga um að Python sé uppsett ásamt eftirfarandi söfnum: `pandas`, `numpy`, `matplotlib`, `scipy`.
2. Sæktu (clone) þetta repository.
3. Opnaðu `scripts/greining.ipynb` í Jupyter Notebook eða VS Code.
4. Keyrðu alla reiti (Run All). Kóðinn les gögnin úr `data/` möppunni og vistar nýjar myndir og töflur sjálfkrafa.

## Myndir í skýrslu
Allar myndir sem birtast í skýrslunni eru búnar til í `scripts/greining.ipynb` og vistaðar í möppuna `figures/`.

## Helstu niðurstöður
Kóðinn framkvæmir eftirfarandi greiningar:
* Útreikning á meðalhita, meðalúrkomu og meðalrennsli.
* Aðskilnað grunnvatnsrennslis (baseflow separation).
* Langæislínur með merkingu á Q5, Q50 og Q95.
* Leitnigreiningu (Theil-Sen slope) fyrir meðalrennsli hvers árstíðar.
* Nánari greiningu á stærstu árlegu flóðatoppunum (Time-to-peak, recession tími o.fl.).