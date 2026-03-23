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
  <img src="https://img.shields.io/badge/Ladder-Studio_5000-000000?style=flat-square"/>
</p>

# ulogix-scada-control

Repositorio de supervisión, control e interfaz hombre-máquina. Diseño HMI bajo estándar ISA-101, implementación SCADA con Ignition, programación Ladder en Studio 5000 / Logix Emulate e integración OPC-UA con el gemelo digital.

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

## Módulos

<table>
<tr>
  <td align="center"><img src="https://raw.githubusercontent.com/ulogix-team/assets/main/icons/node-tech.svg" width="50"/></td>
  <td><strong>scada/</strong> — Ignition: proyectos (.gwbk), pantallas HMI, alarmas y eventos</td>
</tr>
<tr>
  <td align="center"><img src="https://raw.githubusercontent.com/ulogix-team/assets/main/icons/node-tech.svg" width="50"/></td>
  <td><strong>hmi/</strong> — Diseño bajo ISA-101: jerarquía de pantallas, símbolos P&ID</td>
</tr>
<tr>
  <td align="center"><img src="https://raw.githubusercontent.com/ulogix-team/assets/main/icons/node-tech.svg" width="50"/></td>
  <td><strong>plc-ladder/</strong> — Rutinas Ladder (.L5X), base de tags del controlador</td>
</tr>
<tr>
  <td align="center"><img src="https://raw.githubusercontent.com/ulogix-team/assets/main/icons/node-tech.svg" width="50"/></td>
  <td><strong>ignition/</strong> — Scripts Python Ignition, reportes programados</td>
</tr>
<tr>
  <td align="center"><img src="https://raw.githubusercontent.com/ulogix-team/assets/main/icons/node-tech.svg" width="50"/></td>
  <td><strong>opc/</strong> — Configuración OPC-UA, mapeo de tags PLC ↔ SCADA</td>
</tr>
</table>

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

## Arquitectura de Comunicación

```
Nivel 4  Power BI / Python Analytics
           │ OPC-UA / REST
Nivel 3  Ignition SCADA
           │ OPC-UA
Nivel 2  Studio 5000 / Logix Emulate
           │ Señales I/O virtuales
Nivel 1  NX Digital Factory / RobotStudio
```

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

## Estándares Aplicados

| Estándar | Aplicación |
|---|---|
| **ISA-95** | Arquitectura de automatización por niveles |
| **ISA-101** | Diseño de pantallas HMI |
| **IEC 61131-3** | Lenguajes Ladder y Grafcet (SFC) |
| **OPC-UA** | Comunicación PLC ↔ SCADA ↔ Gemelo Digital |

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

## Responsables

| Módulo | Responsable | GitHub |
|---|---|:---:|
| SCADA / HMI / MES | Juan Felipe Triana Aguilera | [@jutrianaa](https://github.com/jutrianaa) |
| PLC / Ladder / Grafcet | Juan José Díaz Guerrero | [@Judiazgu](https://github.com/Judiazgu) |
| Arquitectura de Red / OPC | Andrés Mauricio Morales Martínez | [@mora200217](https://github.com/mora200217) |

**Supervisores:** Carlos J. Cortés · Luis M. Méndez · Víctor H. Grisales · Ricardo Ramírez · Ubaldo García · Eduardo Barrera

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

## Flujo de Trabajo

```
main ──────────────────► producción estable
  └── develop ─────────► integración y desarrollo
```

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/banners/footer-dark.svg" width="100%"/>
