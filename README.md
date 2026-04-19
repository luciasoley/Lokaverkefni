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

## Helstu niðurstöður
Kóðinn framkvæmir eftirfarandi greiningar:
* Útreikning á meðalhita, meðalúrkomu og meðalrennsli.
* Aðskilnað grunnvatnsrennslis (baseflow separation).
* Langæislínur með merkingu á Q5, Q50 og Q95.
* Leitnigreiningu (Theil-Sen slope) fyrir meðalrennsli hvers árstíðar.
* Nánari greiningu á stærstu árlegu flóðatoppunum (Time-to-peak, recession tími o.fl.).