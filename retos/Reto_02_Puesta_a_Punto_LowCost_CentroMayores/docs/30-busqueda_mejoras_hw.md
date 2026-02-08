# 30 — Búsqueda y selección de mejoras de **hardware**

> **Objetivo:** Encontrar las **mejoras mínimas** que conviertan cada PC en **usable** para el centro de mayores, **respetando** S0/S1/S2.

## 1) Piezas candidatas (con enlaces y capturas)

Busca en **tiendas online españolas** (PcComponentes, Amazon ES, Coolmod, Wallapop/segunda mano con precaución) y documenta **al menos 2 opciones por categoría** (cuando aplique):

- **Almacenamiento:** SSD 2.5" (120–240 GB) o adaptadores 2.5"→3.5".
- **Memoria RAM:** módulos compatibles (capacidad y MHz soportados por tu placa).
- **Mantenimiento:** pasta térmica económica, filtros de polvo, tornillería o caddy(**adaptador/bandeja (caddy) para montar una unidad de almacenamiento** en un hueco del PC).
- **Otros (si procede):** adaptador Wi-Fi USB de bajo coste, altavoz barato si no hay sonido, etc.

**Tabla por categoría (ejemplo SSD):**

| Categoria | Marca/Modelo | Capacidad | Precio (€) | Tienda | URL | Captura |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| SSD | Kingston A400 | 120 GB | 16.99 (07/02/2026) | Amazon ES | https://www.amazon.es/Kingston-A400-SSD-Disco-Sólido/dp/B01N6JQS8C | ![SSD](../assets/img/30-hw/SSD01.jpg "SSD") |
| SSD | TeamGroup CX2 | 256 GB | 17.99 (07/02/2026) | Amazon ES | https://www.amazon.es/TEAMGROUP-CX2-256GB-Internal-Solid/dp/B08CKFDPJ3 | ![SSD](../assets/img/30-hw/SSD02.jpg "SSD") |
| RAM | DDR2 PC2-6400 | 2 GB | 6.81 (07/02/2026) | eBay | https://www.ebay.es/itm/183656018363 | ![RAM](../assets/img/30-hw/RAM01.png "RAM") |
| RAM | DDR2 800MHz | 2 GB | 6.00 (07/02/2026) | Wallapop | https://es.wallapop.com/item/2x-kingston-ddr2-2gb-800mhz-ram-1224981514 | ![RAM](../assets/img/30-hw/RAM02.png "RAM") |
| Mantenimiento | Arctic MX-4 | 4 g | 7.19 (07/02/2026) | Amazon ES | https://www.amazon.es/Arctic-MX-4-Pasta-térmica-disipadores/dp/B07L9BDY3T | ![PASTA](../assets/img/30-hw/PASTA.jpg "PASTA") |

> Guarda capturas en `../assets/img/30-hw/` con **URL completa** visible y **fecha/hora**.

## 2) Compatibilidad técnica (justifica con datos)

**_Compatibilidad de los componentes:_**
**Memoria RAM:**
Mi placa base (modelo HP 437793-001 con chipset Q35 Express) admite hasta 8 GB de RAM DDR2. Aunque los módulos actuales funcionan a 667 MHz, la placa soporta hasta 800 MHz, por lo que las piezas nuevas son totalmente compatibles. Además, al tener 4 ranuras y estar usando solo dos, tengo espacio físico de sobra para pinchar el módulo extra de 2 GB.

**Disco SSD:**
El equipo dispone de puertos SATA estándar, que es lo que necesito. El SSD que he elegido es SATA 3, y aunque la versión de los puertos de mi placa sea anterior, la tecnología es retrocompatible. Vamos, que funcionará perfectamente y se notará mucho la aceleración del sistema respecto al disco mecánico.

**Otros componentes:**
Al ser un chasis formato SFF (pequeño), instalaré el SSD de 2,5" en el hueco del disco antiguo usando un adaptador caddy para que quede bien sujeto y no baile. Por último, la pasta térmica seleccionada es apta para el socket LGA775 de mi procesador Intel Core 2 Duo E6750, lo cual es básico para mantener buenas temperaturas y evitar sobrecalentamientos.

> Incluye captura de **fuente oficial** (manual/hoja técnica de la placa o del fabricante de la pieza) donde se vea el dato clave (ej.: “hasta 8 GB DDR2-1600”).
> https://h10032.www1.hp.com/ctg/Manual/c01202501.pdf
![SSD](../assets/img/30-hw/Manual.PNG "SSD")


## 3) Mini‑estimación de impacto (sentido común + referencias)
**De HDD a SSD:**
Este es sin duda el cambio que más se va a notar. Al quitar el viejo disco mecánico Seagate y poner el SSD Kingston, los tiempos de carga desaparecen. El sistema arranca rápido y los programas se abren al instante; esto es vital para que una persona mayor no se líe ni se frustre esperando a que el ordenador reaccione.

**De 1 GB a 3 GB de RAM:**
Ahora mismo con 1 GB el equipo se ahoga. Al añadir el módulo de 2 GB (para tener 3 GB en total), el ordenador podrá gestionar la multitarea real, como tener una videollamada y el navegador abiertos a la vez. Con esto evitamos que el sistema se quede "congelado" tirando de disco duro porque le falta memoria.

**Pasta térmica y limpieza:**
Aplicar la pasta MX-4 en el procesador y limpiar el polvo es básico para la salud del PC. Al mejorar la transferencia de calor, el ventilador no necesita girar tan rápido para enfriar el Core 2 Duo. El resultado es un equipo que no se calienta y, sobre todo, que hace mucho menos ruido ambiente.

> **No** se piden benchmarks. Usa criterio y referencias de fuentes fiables.

## 4) Escenario elegido y desglose de gasto (S0/S1/S2)

**Escenario S2:** Porque, con un presupuesto de 30 euros, puedo abarcar directamente los tres puntos críticos del equipo: el almacenamiento, la RAM y la temperatura.

| Escenario | Pieza | Precio (€) | Unidades | Subtotal (€) | Nota |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **S2** | SSD Kingston 120 GB | 16.99 | 1 | 16.99 | Nuevo en Amazon |
| **S2** | RAM 2 GB DDR2 | 5 | 1 | 5 | Segunda mano Wallapop |
| **S2** | Pasta térmica Arctic | 5.60 | 1 | 5.60 | Bote para varios usos |
| | **Total HW** | | | **27.59** | |

El gasto total de **27,59 euros** entra perfectamente dentro del límite de los 30 euros marcados para el escenario S2.
Luego traslada el **Total HW** a `75-plan_presupuesto_hw_y_roi.md` para calcular costes y ROI.
