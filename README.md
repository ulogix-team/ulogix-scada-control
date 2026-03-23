<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/banners/header-dark.svg" width="100%"/>

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-dark.svg" width="100%"/>

<p align="center">
  <img src="https://raw.githubusercontent.com/ulogix-team/assets/main/logos/ulogix-icon-transparent-dark.svg" height="55"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Ignition-SCADA-000000?style=flat-square"/>
  &nbsp;
  <img src="https://img.shields.io/badge/OPC--UA-Comunicación-000000?style=flat-square"/>
  &nbsp;
  <img src="https://img.shields.io/badge/ISA--101-HMI_Design-000000?style=flat-square"/>
  &nbsp;
  <img src="https://img.shields.io/badge/MQTT-IoT_Cloud-000000?style=flat-square"/>
</p>

# ulogix-scada-control

Repositorio de supervisión, control e interfaz hombre-máquina. Diseño HMI ISA-101, SCADA Ignition, Ladder en Studio 5000, OPC-UA y MQTT para IoT/Cloud.

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

## Estructura

```
ulogix-scada-control/
├── scada/       Ignition: proyectos (.gwbk), pantallas, alarmas
├── hmi/         Diseño ISA-101: jerarquía de pantallas, símbolos P&ID
├── plc-ladder/  Rutinas Ladder (.L5X), base de tags
├── ignition/    Scripts Python Ignition, reportes programados
└── opc/         Configuración OPC-UA, mapeo de tags PLC ↔ SCADA
```

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

## Tareas por Módulo

<table>
<tr>
  <td align="center"><img src="https://raw.githubusercontent.com/ulogix-team/assets/main/icons/node-tech.svg" width="50"/></td>
  <td>
    <strong>plc-ladder/</strong> — Módulo 6 — Controladores Industriales<br/>
    • Implementación Ladder en Logix Emulate (Apr 22)<br/>
    • Validación funcional PLC – Gemelo Digital (Apr 29)
  </td>
</tr>
<tr>
  <td align="center"><img src="https://raw.githubusercontent.com/ulogix-team/assets/main/icons/node-tech.svg" width="50"/></td>
  <td>
    <strong>hmi/ + scada/ + opc/ + ignition/</strong> — Módulo 7 — SCADA<br/>
    • Diseño de interfaz HMI bajo estándar ISA-101 (Apr 29)<br/>
    • Configuración comunicación OPC entre PLC y SCADA (May 6)<br/>
    • Implementación del SCADA en Ignition (May 7)<br/>
    • Comunicación MQTT para IoT/Cloud (May 7)
  </td>
</tr>
</table>

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

## Arquitectura de Comunicación

```
Nivel 4  Power BI / Python Analytics  ←── May 9
           │ OPC-UA / REST / MQTT
Nivel 3  Ignition SCADA               ←── May 7
           │ OPC-UA
Nivel 2  Studio 5000 / Logix Emulate  ←── Apr 22
           │ Señales I/O virtuales
Nivel 1  NX Digital Factory           ←── Apr 18
```

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

## Estándares Aplicados

| Estándar | Aplicación |
|---|---|
| **ISA-95** | Arquitectura de automatización por niveles |
| **ISA-101** | Diseño de pantallas HMI (Apr 29) |
| **IEC 61131-3** | Lenguajes Ladder y Grafcet (Apr 22) |
| **OPC-UA** | Comunicación PLC ↔ SCADA ↔ Gemelo Digital (May 6) |
| **MQTT** | Comunicación IoT/Cloud (May 7) |

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

## Responsables

| Módulo | Responsable | GitHub |
|---|---|:---:|
| SCADA / HMI / MQTT / MES | Juan Felipe Triana Aguilera | [@jutrianaa](https://github.com/jutrianaa) |
| PLC / Ladder / Grafcet | Juan José Díaz Guerrero | [@Judiazgu](https://github.com/Judiazgu) |
| Arquitectura / OPC-UA / Red | Andrés Mauricio Morales Martínez | [@mora200217](https://github.com/mora200217) |

**Supervisores:** Carlos J. Cortés · Luis M. Méndez · Víctor H. Grisales · Ricardo Ramírez · Ubaldo García · Eduardo Barrera

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

## Flujo de Trabajo

```
main ──────────────────► producción estable
  └── develop ─────────► integración y desarrollo
```

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/banners/footer-dark.svg" width="100%"/>
