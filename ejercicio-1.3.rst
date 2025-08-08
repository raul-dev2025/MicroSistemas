Ejercicio 1.3: Comparativa de Buses de Expansión: PCIe vs USB vs SATA
------------------------------------------------------------------------

Tecnologías Analizadas:
- PCI Express (PCIe) 3.0, 4.0 y 5.0.
- USB 2.0, 3.2 Gen 1/Gen 2 y 4.0.
- SATA 3.0.

Tabla Comparativa
-----------------

+------------+----------------+---------------------+-----------------+------------------------+--------------------
| Tecnología |     Versión    | Ancho de Banda Máx. |   Topología     |   Velocidad Transfer.  |             Usos Tí
+============+================+=====================+=================+========================+====================
|    PCIe    |       3.0      |   985 MB/s/carril   | Punto a punto   |          8 GT/s        |     GPUs, NVMe, tar
+------------+----------------+---------------------+-----------------+------------------------+--------------------
|            |       4.0      |   1.97 GB/s/carril  | Punto a punto   |         16 GT/s        |     GPUs modernas, 
+------------+----------------+---------------------+-----------------+------------------------+--------------------
|            |       5.0      |   3.94 GB/s/carril  | Punto a punto   |         32 GT/s        | GPUs gama alta, SSD
+------------+----------------+---------------------+-----------------+------------------------+--------------------
|    USB     |       2.0      |   60 MB/s           |   Compartido    |        480 Mbps        |        Periféricos 
+------------+----------------+---------------------+-----------------+------------------------+--------------------
|            |    3.2 Gen 1   |   625 MB/s          |   Compartido    |          5 Gbps        |          Discos ext
+------------+----------------+---------------------+-----------------+------------------------+--------------------
|            |    3.2 Gen 2   |   1.25 GB/s         |    Dedicado     |         10 Gbps        |            SSDs ext
+------------+----------------+---------------------+-----------------+------------------------+--------------------
|            |    4.0         |   5 GB/s            | Punto a punto   |         40 Gbps        |      Monitores 8K, 
+------------+----------------+---------------------+-----------------+------------------------+--------------------
|   SATA     |    3.0         |   600 MB/s          | Punto a punto   |          6 Gbps        |         HDDs, SSDs 
+------------+----------------+---------------------+-----------------+------------------------+--------------------

Claves Técnicas
--------------

PCI Express
~~~~~~~~~~
- Escalabilidad: Rendimiento multiplicado por carriles (x1, x4, x8, x16).
- Latencia ultra-baja para componentes críticos.
- Evolución: Cada versión duplica el ancho de banda.

USB
~~~
- Retrocompatibilidad entre versiones.
- USB4 unifica protocolos Thunderbolt.
- Alimentación eléctrica integrada (hasta 240W en USB PD 3.1).

SATA
~~~~
- Protocolo optimizado para almacenamiento.
- Sustituido progresivamente por NVMe en SSDs.
- Sigue siendo estándar en HDDs mecánicos.

Recomendaciones de Uso
----------------------

1. Máximo rendimiento (GPU/SSD).
   - PCIe 5.0 x16 (63 GB/s teóricos).
   
2. Almacenamiento externo.
   - USB4 para NVMe externo.
   - USB 3.2 Gen 2 para SSDs SATA.

3. Equilibrio costo-rendimiento.
   - PCIe 4.0 para la mayoría de usuarios.
   - SATA 3.0 para HDDs y SSDs secundarios.
.
Notas Adicionales
----------------
- GT/s = GigaTransfers por segundo (no equivalente directo a GB/s).
- Los anchos de banda reales son ~20% menores por overhead de protocolo.
- Thunderbolt 3/4 comparte connector USB-C pero usa protocolo PCIe.

-----