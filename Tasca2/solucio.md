# T02: Selecció d’un SAI per una empresa client

**Autor:** Pau Constanseu  
**Data:** 30/09/2025

---

## 1. Introducció

La protecció dels equips informàtics i la continuïtat del servei són essencials per a qualsevol empresa. TecnoGestió S.L., davant de talls de corrent habituals, ha decidit adquirir un SAI per garantir el correcte funcionament dels ordinadors i del router i permetre un apagament segur.

L’objectiu d’aquesta tasca és determinar els requisits del despatx, calcular la potència necessària i seleccionar el SAI més adequat segons autonomia, potència i cost.

---

## 2. Índex

1. Introducció  
2. Índex  
3. Inventari d’equips  
4. Càlcul de potència total amb 20% de marge  
5. Determinació de l’autonomia  
6. Recerca de models de SAI  
7. Informe tècnic

---

## 3. Inventari d’equips

| Dispositiu | Quantitat | Connexió al SAI? | Consum per unitat | Consum VA aproximat | Justificació |
|-------------|------------|------------------|-------------------|----------------------|---------------|
| PcCom Work Intel Core i5-12400 / 32GB / 1TB SSD + Windows 11 | 4 | Sí | 250 W | 278 VA | Evita la pèrdua de dades i permet l’apagament correcte. |
| Monitor Nilox NXM24FHD1 23.8" IPS FullHD | 4 | Si/No | 15 W | 16 VA | Poden suportar apagades; connectarem al SAI si hi ha prou potència. |
| HP Envy Impressora Multifunció 6530e | 1 | No | 4,25 W (Ready) | 5 VA | Consum baix, no essencial. |
| Router Xiaomi Mi Wifi 4C | 1 | Sí | 5 W | 6 VA | Garanteix connexió a internet durant apagades curtes. |
| Altres dispositius (carregadors, telèfons) | Variable | No | 10–20 W | 11–22 VA | No essencials, no es connectaran al SAI. |

**Enllaços de referència:**
- [PcCom Work i5-12400](https://www.pccomponentes.com/ordenador-sobremesa-pccom-work-intel-core-i5-12400-32gb-1tb-ssd)
- [Monitor Nilox NXM24FHD1](https://www.pccomponentes.com/monitor-nilox-nxm24fhd12-monitor-238-ips-fullhd)
- [HP Envy 6530e](https://www.hp.com/es-es/shop/product.aspx?id=714P1B&opt=629&sel=PRN)
- [Router Xiaomi Mi Wifi 4C](https://www.pccomponentes.com/xiaomi-mi-wifi-router-4c)

---

## 4. Càlcul de potència total amb 20% de marge

SAI connectarà:
- 4 ordinadors PcCom Work i5-12400  
- 1 router Xiaomi Mi Wifi 4C  
- Monitors opcionalment (exclosos per assegurar marge de potència)

| Dispositiu | Quantitat | Consum total (W) | Consum total (VA) |
|-------------|------------|------------------|-------------------|
| Ordinadors de sobretaula | 4 | 1000 W | 1112 VA |
| Router | 1 | 5 W | 6 VA |

Potència total sense marge: **1005 W / 1118 VA**  
Amb marge del **20%**:  
- **1206 W**  
- **1342 VA**

Per tant, el SAI hauria de ser aproximadament **1350 VA / 1200 W**.  
Si s’afegeixen monitors, uns **1470 VA / 1250 W**.

---

## 5. Determinació de l’autonomia

L’autonomia d’un SAI ha de permetre guardar treballs i apagar els equips amb seguretat (uns **10 minuts**).

Amb quatre ordinadors i un router connectats (~1200 W / 1350 VA), un SAI de **1350–1500 VA / 1200 W** ofereix l’autonomia necessària.

---

## 6. Recerca de models de SAI

| Model | Potència (VA/W) | Autonomia estimada | Preu aproximat |
|--------|------------------|--------------------|----------------|
| Riello UPS Vision VST 1500 | 1500 / 1200 | 10–12 min | 400,62 € |
| Salicru SPS 1500 Advance T | 1500 / 1350 | 10–12 min | 288,03 € |
| Eaton 5S 1500i | 1500 / 900 | 10–12 min | 437,62 € |

**Enllaços de referència:**
- [Riello UPS Vision VST 1500](https://www.tecnologiamodular.es/periferics/sais/sai-ups/sai-riello-vst-1500?utm_source=FEED_ID_20&utm_medium=marketplace)
- [Salicru SPS Advance T 1500](https://www.amazon.es/Salicru-Advance-Line-Interactive-senoidal-Torre/dp/B079G1LNHX)
- [Eaton 5S 1500i](https://www.pccomponentes.com/sai-eaton-5s-1500i-sai-1500va-900w)

---

## 7. Informe tècnic

TecnoGestió S.L. disposa de quatre ordinadors de sobretaula, monitors, una impressora multifunció i un router. Davant dels talls de corrent recurrents, es necessita un SAI que protegeixi els equips i permeti un apagament segur.

Els equips crítics que es connectaran al SAI són els quatre ordinadors **PcCom Work i5-12400** i el **router Xiaomi Mi Wifi 4C**.  
El consum total amb marge de seguretat del 20% és d’aproximadament **1200 W / 1350 VA**, suficient per dimensionar correctament el SAI.  
L’autonomia mínima necessària és de **10 minuts** per poder apagar els equips amb seguretat.

S’han analitzat diversos models: **Riello UPS Vision VST 1500**, **Eaton 5S 1500i** i **Salicru SPS Advance T 1500**.  
Tots compleixen amb els requisits mínims de potència i autonomia, però **el Riello destaca per la seva fiabilitat, servei tècnic i preu equilibrat**, oferint **10–12 minuts** d’autonomia, suficient per a un despatx petit com el de TecnoGestió S.L.

---

## Estructura del document

1. Introducció  
2. Índex  
3. Inventari d’equips  
4. Càlcul de potència total amb 20% de marge  
5. Determinació de l’autonomia  
6. Recerca de models de SAI  
7. Informe tècnic




[Tornar a la pàgina del projecte](../)

