<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/banners/header-dark.svg" width="100%"/>

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-dark.svg" width="100%"/>

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

Repositorio de supervisión, control e interfaz hombre-máquina. Incluye el diseño de pantallas HMI bajo estándar ISA-101, implementación SCADA con Ignition, programación Ladder en Studio 5000 / Logix Emulate e integración OPC-UA con el gemelo digital.

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

## Estructura

```
ulogix-scada-control/
├── scada/       Ignition: proyectos, pantallas, alarmas
├── hmi/         Diseño HMI ISA-101, símbolos P&ID
├── plc-ladder/  Rutinas Ladder Studio 5000, base de tags
├── ignition/    Scripts Python Ignition, reportes
└── opc/         Configuración OPC-UA, mapeo de tags
```

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
