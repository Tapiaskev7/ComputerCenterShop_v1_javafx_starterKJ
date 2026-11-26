# ComputerCenterShop — pràctica integradora RA2

> **Plantilla de l'equip.** Copieu aquest fitxer al vostre repositori de treball i completeu-lo a mesura que avanceu. No inclou solucions de codi: les decisions, proves i explicacions han de ser vostres.

## Fitxa de l'equip

- Integrants: **[Kevin Tapias]** i **[Jordan Hidalgo]**
- Repositori compartit: **[https://github.com/Tapiaskev7/ComputerCenterShop_v1_javafx_starterKJ.git]**
- Branca de treball habitual: **[main]**
- Data d'inici: **[2026-11-17]**
- Última actualització: **[2026/11/24]**

## Propòsit del projecte

En aquesta pràctica desenvolupem una aplicació Java que accedeix a una base de dades relacional amb JDBC. Treballem sobre el projecte *starter* indicat pel professorat i fem servir el backlog RA2 per organitzar les tasques, els commits, les proves i les decisions tècniques.

El repositori ha de mostrar el procés de treball real de l'equip. No es tracta només d'arribar a una aplicació que s'executi: també cal poder explicar què s'ha canviat, com s'ha comprovat i per què la decisió correspon a cada *issue*.

## Punt de partida

- Repositori *starter* utilitzat: **[https://github.com/Bemen3-LLHB/ComputerCenterShop_v1_javafx_starter]**
- Gestor de base de dades relacional utilitzat: **[H2]**
- Connector utilitzat: **[ JDBC H2]**
- Entorn de desenvolupament: **[Eclipse IDE amb Maven]**
- Comandament o acció que fem servir per comprovar l'execució: **[Executem amb Run As -> Maven build utilitzant clean javafx:run]**

> No incorporeu ORM, Hibernate, ObjectDB, MongoDB, serveis externs ni persistència principal en fitxers. Aquests elements no formen part de RA2.

## Com treballem cada *issue*

1. Llegim l'objectiu i els criteris d'acceptació de l'*issue*.
2. Acordem què ha de canviar i qui inicia la feina.
3. Fem canvis petits i comprensibles, amb *commits* que expliquin la decisió.
4. Provem el comportament esperat i en guardem una evidència.
5. Actualitzem aquest README amb el resultat, la prova i l'enllaç al *commit* o a la *pull request*.
6. Tanquem l'*issue* només quan l'equip pot explicar individualment la solució aplicada.

## Progrés del backlog

Marqueu una tasca quan la prova i el rastre al repositori estiguin recollits. Els enllaços apunten a l'enunciat, no a una solució.

### M1 · Base JDBC operativa

- [X] [RA2-ISSUE-01 · Preparar el projecte JDBC](issues/RA2-ISSUE-01-preparar-projecte-jdbc.md)
- [X] [RA2-ISSUE-02 · Connector, URL i connexió](issues/RA2-ISSUE-02-revisar-connector-url-connexio.md)
- [X] [RA2-ISSUE-03 · Estructura relacional](issues/RA2-ISSUE-03-crear-estructura-relacional.md)

### M2 · Operacions relacionals principals

- [X] [RA2-ISSUE-04 · Inserció de dades](issues/RA2-ISSUE-04-inserir-producte-preparedstatement.md)
- [X] [RA2-ISSUE-05 · Actualització d'estoc](issues/RA2-ISSUE-05-actualitzar-estoc.md)
- [X] [RA2-ISSUE-06 · Eliminació controlada](issues/RA2-ISSUE-06-eliminar-producte-controlat.md)
- [ ] [RA2-ISSUE-07 · Consultes i resultats](issues/RA2-ISSUE-07-consultar-inventari-resultset.md)

### M3 · Robustesa JDBC

- [ ] [RA2-ISSUE-08 · Tancament de recursos](issues/RA2-ISSUE-08-tancar-recursos.md)
- [ ] [RA2-ISSUE-09 · Transaccions](issues/RA2-ISSUE-09-transaccio-commit-rollback.md)
- [ ] [RA2-ISSUE-10 · Procediment amb paràmetres](issues/RA2-ISSUE-10-procediment-parametres.md)
- [ ] [RA2-ISSUE-11 · Errors de connexió i operacions](issues/RA2-ISSUE-11-errors-connexio-recursos.md)

### M4 · Documentació i tancament

- [ ] [RA2-ISSUE-12 · Documentar l'execució i la configuració](issues/RA2-ISSUE-12-documentar-execucio-configuracio.md)
- [ ] [RA2-ISSUE-13 · Preparar el lliurament de la pràctica](issues/RA2-ISSUE-13-lliurament-practica-integradora.md)

## Registre de treball

Dupliqueu aquest bloc per a cada *issue* que completeu. Escriviu amb les vostres paraules i enllaceu només proves i *commits* del vostre repositori.

### RA2-ISSUE-XX · [títol de l'*issue*]

- Estat: **pendent | en curs | comprovat**
- Persona que l'ha iniciat: **[nom]**
- Problema inicial: **[què no funcionava o què faltava]**
- Decisió aplicada: **[què heu decidit fer i per què]**
- Canvis fets: **[fitxers o parts del projecte modificades]**
- Prova realitzada: **[cas que heu provat i resultat observat]**
- Evidència: **[enllaç a captura, registre, vídeo breu o apartat del repositori]**
- *Commit* o *pull request*: **[enllaç o identificador]**
- Explicació individual: **[què pot explicar cada integrant sobre aquesta tasca]**
- Ús d'IA, si n'hi ha hagut: **[consulta feta, ajuda rebuda i comprovació pròpia]**

### RA2-ISSUE-01 · [Preparar projecte JDBC local*]

- Estat: **comprovat**
- Persona que l'ha iniciat: **[Kevin]**
- Problema inicial: **[Havíem de preparar i revisar el projecte inicial abans de començar a treballar amb JDBC.]**
- Decisió aplicada: **[Revisar el pom.xml per identificar el gestor de base de dades, el connector JDBC i la classe principal de JavaFX.]**
- Canvis fets: **[No ha sigut necessari modificar el codi. Hem revisat la configuració del projecte i els TODO del fitxer ProductDaoImplJDBC.java per identificar les tasques pendents.]**
- Prova realitzada: **[Hem executat el projecte amb Maven Build (javafx:run) per comprovar quina issue pendent apareixia primer.]**
- Evidència: **[Captures adjuntades al git de la issue 1]**
- *Commit* o *pull request*: **[commit]**
- Explicació individual: **[Hem identificat que el gestor de base de dades és H2 i que utilitzem el connector JDBC per comunicar Java amb la base de dades. També hem comprovat com executar el projecte amb JavaFX.]**
- Ús d'IA, si n'hi ha hagut: **[consulta feta, ajuda rebuda i comprovació pròpia]**
## Proves que hem de poder repetir

### RA2-ISSUE-02 · [títol de l'*issue*]

- Estat: **Comprovat**
- Persona que l'ha iniciat: **[Jordan]**
- Problema inicial: **[ Faltava implementar la connexió entre l'aplicació Java i la base de dades H2.]**
- Decisió aplicada: **[Hem decidit utilitzar DriverManager amb les dades de connexió definides al projecte. També hem revisat que la dependència H2 estigui al pom.xml.]**
- Canvis fets: **[ Hem completat el mètode connect() del fitxer ProductDaoImplJDBC.java.]**
- Prova realitzada: **[Hem executat l'aplicació i hem comprovat que es connecta correctament a la base de dades.]**
- Evidència: **[https://github.com/Tapiaskev7/ComputerCenterShop_v1_javafx_starterKJ/issues/2#issuecomment-7017511416]**
- *Commit* o *pull request*: **[https://github.com/Tapiaskev7/ComputerCenterShop_v1_javafx_starterKJ/issues/3#issuecomment-7140957984]**
- Explicació individual: **[Aquesta tasca no m'ha semblat gaire complicada. He après com es connecta una aplicació Java amb una base de dades H2 i la importància de tenir ben configurada la dependència al pom.xml.]**
- Ús d'IA, si n'hi ha hagut: **[consulta feta, ajuda rebuda i comprovació pròpia]**

### RA2-ISSUE-03 · [Implementar estructura relacional*]

- Estat: **comprovat**
- Persona que l'ha iniciat: **[Kevin]**
- Problema inicial: **[ Faltava crear l'estructura de la base de dades per guardar els productes i els moviments de l'inventari.]**
- Decisió aplicada: **[Hem decidit crear les taules products i inventory_history si no existeixen, relacionar-les mitjançant una clau forana i afegir productes inicials si l'inventari està buit.]**
- Canvis fets: **[Hem completat el mètode initSchema() del fitxer ProductDaoImplJDBC.java, incloent-hi la creació de les taules, l'àlies d'alerta d'estoc i les dades inicials.]**
- Prova realitzada: **[ Hem inicialitzat l'esquema i hem comprovat des del CMD que les taules existeixen i que es poden consultar els productes i l'historial.]**
- Evidència: **[https://github.com/Tapiaskev7/ComputerCenterShop_v1_javafx_starterKJ/issues/3#issuecomment-7140957984]**
- *Commit* o *pull request*: **[enllaç o identificador]**
- Explicació individual: **[Aquesta tasca m'ha semblat una mica més complicada perquè calia entendre com es relacionaven les dues taules. He après com es crea l'estructura de la base de dades i per què s'utilitzen les claus foranes.]**
- Ús d'IA, si n'hi ha hagut: **[consulta feta, ajuda rebuda i comprovació pròpia]**

### RA2-ISSUE-04 · [Implementar insercio amb PreparedStatement*]

- Estat: **comprovat**
- Persona que l'ha iniciat: **[Jordan]**
- Problema inicial: **[ Faltava implementar el mètode insertProduct() per guardar nous productes a la base de dades.]**
- Decisió aplicada: **[Hem decidit utilitzar PreparedStatement per inserir el nom, el preu, la disponibilitat i l'estoc del producte mitjançant paràmetres.]**
- Canvis fets: **[Hem completat el mètode insertProduct() del fitxer ProductDaoImplJDBC.java.]**
- Prova realitzada: **[Hem afegit el producte Impressora HP des de JavaFX i l'aplicació ha mostrat un missatge confirmant la inserció. Posteriorment, hem comprovat els productes guardats mitjançant una consulta SQL.]**
- Evidència: **[https://github.com/Tapiaskev7/ComputerCenterShop_v1_javafx_starterKJ/issues/4#issuecomment-7197198858]**
- *Commit* o *pull request*: **[enllaç o identificador]**
- Explicació individual: **[Al principi m'ha costat una mica entendre com funcionava PreparedStatement i com s'assignaven els paràmetres. Després de fer les proves, he entès com es guarda un producte a la base de dades.]**
- Ús d'IA, si n'hi ha hagut: **[consulta feta, ajuda rebuda i comprovació pròpia]**

### RA2-ISSUE-05 · [títol de l'*issue*]

- Estat: **comprovat**
- Persona que l'ha iniciat: **[Kevin]**
- Problema inicial: **[ Faltava implementar el mètode updateStock() per modificar l'estoc i la disponibilitat dels productes.]**
- Decisió aplicada: **[Hem decidit utilitzar PreparedStatement per actualitzar l'estoc del producte pel seu nom. Si l'estoc és superior a zero, el producte està disponible. Si és zero, deixa d'estar disponible.]**
- Canvis fets: **[Hem completat el mètode updateStock() del fitxer ProductDaoImplJDBC.java.]**
- Prova realitzada: **[ Hem preparat una prova per modificar l'estoc d'un producte i comprovar que la disponibilitat canvia quan l'estoc arriba a zero. Falta confirmar els resultats amb les consultes corresponents.]**
- Evidència: **[https://github.com/Tapiaskev7/ComputerCenterShop_v1_javafx_starterKJ/issues/5#issuecomment-7198543232]**
- *Commit* o *pull request*: **[enllaç o identificador]**
- Explicació individual: **[Aquesta tasca m'ha semblat més fàcil perquè ja havia treballat amb PreparedStatement a la tasca anterior. He entès com modificar l'estoc d'un producte i controlar la seva disponibilitat segons les unitats que té.]**
- Ús d'IA, si n'hi ha hagut: **[consulta feta, ajuda rebuda i comprovació pròpia]**


### RA2-ISSUE-06 · [Implementar eliminacio controlada*]

- Estat: **comprovat**
- Persona que l'ha iniciat: **[Jordan]**
- Problema inicial: **[Faltava implementar el mètode deleteProduct() per poder eliminar productes de la base de dades.]**
- Decisió aplicada: **[Hem decidit utilitzar PreparedStatement per eliminar el producte pel seu nom i un try-catch per controlar l'error si té historial associat.]**
- Canvis fets: **[Hem modificat el mètode deleteProduct() del fitxer ProductDaoImplJDBC.java.]**
- Prova realitzada: **[ Hem eliminat el producte Raton correctament. També hem afegit un registre de prova a l'historial de Teclado i hem intentat eliminar-lo, però l'aplicació ens ha mostrat un missatge d'error. Finalment, hem comprovat els resultats amb consultes SQL des del CMD.]**
- Evidència: **[https://github.com/Tapiaskev7/ComputerCenterShop_v1_javafx_starterKJ/issues/6#issuecomment-7199698911]**
- *Commit* o *pull request*: **[enllaç o identificador]**
- Explicació individual: **[Aquesta tasca m'ha semblat una mica més complicada per la gestió de l'error quan un producte té historial associat. També he après a connectar-me a H2 des del CMD i comprovar directament si un producte s'ha eliminat o no.]**
- Ús d'IA, si n'hi ha hagut: **[consulta feta, ajuda rebuda i comprovació pròpia]**


| Cas que comprovem | Dades o condicions inicials | Resultat observat | Evidència |
| --- | --- | --- | --- |
| Arrencada del projecte | **[completeu]** | **[completeu]** | **[enllaç]** |
| Operació de modificació | **[completeu]** | **[completeu]** | **[enllaç]** |
| Consulta de dades | **[completeu]** | **[completeu]** | **[enllaç]** |
| Cas d'error controlat | **[completeu]** | **[completeu]** | **[enllaç]** |
| Operació agrupada o transacció | **[completeu]** | **[completeu]** | **[enllaç]** |

## Decisions i dubtes de l'equip

| Data | *Issue* | Decisió o dubte | Com s'ha resolt | Referència |
| --- | --- | --- | --- | --- |
| **[AAAA-MM-DD]** | **[RA2-ISSUE-XX]** | **[completeu]** | **[completeu]** | **[enllaç]** |

## Ús responsable d'IA

El nivell previst és **IA-1**: podeu usar eines d'IA com a suport per entendre conceptes, formular hipòtesis o revisar una explicació. No substitueixen les proves del projecte ni l'explicació individual.

Si n'heu fet ús, anoteu a l'*issue* corresponent què heu preguntat, què heu contrastat amb el projecte i quina decisió final heu pres. No enganxeu una resposta d'IA com si fos una prova de funcionament.

## Abans de donar la pràctica per preparada

- [ ] Els *issues* P0 tenen un resultat comprovat o una incidència explicada.
- [ ] El repositori conté *commits* que permeten seguir el treball de l'equip.
- [ ] Les proves de funcionament tenen evidències enllaçades.
- [ ] Les decisions sobre connector, consultes, recursos, transaccions i procediments estan explicades amb paraules pròpies.
- [ ] Tots dos integrants poden defensar individualment les decisions tècniques del repositori.
- [ ] El README no inclou solucions copiades ni contingut fora de l'abast de RA2.

---

*Aquesta plantilla és un suport per documentar el treball. El que acredita el procés és el repositori de l'equip, amb els seus canvis, proves, decisions i explicacions.*
