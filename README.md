# project
Egy egyetemi projekthez készítettem ezeket a jupyter notebookokat. 
Adat:
- Vannak agygráfjaink, ezekben a csúcsok agyterületeknek felelnek meg, és két csúcs össze van kötve, ha a megfelelő agyterületek között található idegrost, amin az információ terjedhet. Az éleknek vannak attribútumai, amik személyenként eltérnek: fiber_length, number_of_fibers, FA. 
Ezeket csináltam:
- A gráfokból készítettem 101 gráfot úgy, hogy minden 0<=i<=100 számra az i. gráfban azok az élek szerepljenek, amelyek az összes alany legalább i%-ánál jelen vannak. Ezt a frequency_graphs jupyter notebookban leírt módon csináltam meg, a gráfokat graphml formátumban mentettem el, ezek megtalálhatóak a frequency_graphs mappában.
- Minden 0<=i<=100 számra készítettem egy táblázatot, ami azokat az éleket tartalmazza, amelyek az alanyok legalább i%-ában jelen vannak. Ezek a táblázatok tartalmazzák a következőket:
  -  az egyes élek végpontjainak indexei
  -  a végpontoknak megfelelő agyi területek elnevezései
  -  az adott él hány személynél fordul elő 
  -  az élek attribútumainak átlagát és mediánját (csak azokat a személyeket nézzük, akiknél megtalálható az adott él).
Az ehhez tartozó kód az edge_tables notebookban, a létrehozott táblázatok a tables mappában találhatóak meg.
- Végül a diagram notebookban néhány ábra szerepel, ami azt mutatja, hogy különböző felbontásoknál (egyre több és több részre osztjuk az agyat), hogyan változik a közös élek száma.
