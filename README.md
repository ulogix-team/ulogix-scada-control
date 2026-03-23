<p align="center">
  <img src="https://raw.githubusercontent.com/ulogix-team/assets/main/banners/header-dark.svg" width="100%"/>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-dark.svg" width="100%"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Ignition-SCADA-7C3AED?style=flat-square"/>
  &nbsp;
  <img src="https://img.shields.io/badge/OPC--UA-Comunicación-a855f7?style=flat-square"/>
  &nbsp;
  <img src="https://img.shields.io/badge/ISA--101-HMI%20Design-7C3AED?style=flat-square"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Ladder-Studio%205000-0e0525?style=flat-square"/>
</p>

# ulogix-scada-control · SCADA, HMI y Control PLC

Repositorio de supervisión, control e interfaz hombre-máquina. Incluye el diseño de pantallas HMI bajo estándares ISA-101, la implementación SCADA con Ignition, la programación Ladder en Studio 5000 / Logix Emulate y la integración OPC para comunicación con el gemelo digital.

<p align="center">
  <img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-dark.svg" width="100%"/>
</p>

## 📁 Estructura del Repositorio

```
ulogix-scada-control/
│
├── scada/                      # Sistema SCADA (Ignition)
│   ├── proyectos/              # Archivos de proyecto Ignition (.gwbk)
│   ├── pantallas/              # Diseño de vistas y navegación
│   ├── alarmas/                # Configuración de alarmas y eventos
│   └── README.md
│
├── hmi/                        # Interfaz Hombre-Máquina
│   ├── diseno/                 # Mockups y estándares ISA-101
│   ├── simbolos/               # Biblioteca de símbolos P&ID
│   └── README.md
│
├── plc-ladder/                 # Programación PLC Ladder
│   ├── programas/              # Rutinas Ladder en Studio 5000
│   ├── tags/                   # Base de tags del PLC
│   └── README.md
│
├── ignition/                   # Configuración específica Ignition
│   ├── scripts/                # Scripts Python Ignition
│   ├── reportes/               # Módulo de reportes
│   └── README.md
│
└── opc/                        # Comunicación OPC-UA
    ├── configuracion/          # Configuración del servidor OPC
    ├── mapeo-tags/             # Mapeo de tags OPC ↔ PLC
    └── README.md
```

<p align="center">
  <img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-dark.svg" width="100%"/>
</p>

## 🖥️ Arquitectura de Control

```
Nivel 4 (ERP/MES)
     │ Power BI / Python Analytics
     │
Nivel 3 (SCADA)
     │ Ignition (Inductive Automation)
     │ OPC-UA Server
     │
Nivel 2 (Control)
     │ Studio 5000 / Logix Emulate
     │ Grafcet → Ladder
     │
Nivel 1 (Campo)
     │ Sensores / Actuadores virtuales
     │ NX Digital Factory / RobotStudio
```

<p align="center">
  <img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-dark.svg" width="100%"/>
</p>

## 🔧 Estándares Aplicados

| Estándar | Aplicación |
|---|---|
| **ISA-95** | Arquitectura de automatización por niveles |
| **ISA-101** | Diseño de pantallas HMI |
| **IEC 61131-3** | Lenguaje Ladder y Grafcet (SFC) |
| **OPC-UA** | Comunicación entre PLC ↔ SCADA ↔ Gemelo Digital |

<p align="center">
  <img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-dark.svg" width="100%"/>
</p>

## 👥 Responsables

| Módulo | Responsable | GitHub |
|---|---|---|
| SCADA / HMI / MES | Juan F. Triana | [@jutrianaa](https://github.com/jutrianaa) |
| PLC / Ladder / Grafcet | Juan J. Díaz | [@Judiazgu](https://github.com/Judiazgu) |
| Arquitectura de Red / OPC | Andrés M. Morales | [@mora200217](https://github.com/mora200217) |

**Supervisores académicos:** Carlos J. Cortés · Luis M. Méndez · Víctor H. Grisales · Ricardo Ramírez · Ubaldo García · Eduardo Barrera

<p align="center">
  <img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-dark.svg" width="100%"/>
</p>

## 🔗 Repositorios Relacionados

- [ulogix-manufacturing](https://github.com/ulogix-team/ulogix-manufacturing) — Gemelo digital, PLC físico
- [ulogix-data-finance](https://github.com/ulogix-team/ulogix-data-finance) — OEE, Power BI
- [ulogix-team.github.io](https://ulogix-team.github.io) — Sitio web del proyecto

<p align="center">
  <img src="https://raw.githubusercontent.com/ulogix-team/assets/main/banners/footer-dark.svg" width="100%"/>
</p>
