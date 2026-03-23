<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/banners/header-dark.svg" width="100%"/>

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-dark.svg" width="100%"/>

# opc — Comunicación OPC-UA

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-section-dark.svg" width="100%"/>

Configuración del servidor OPC-UA para la interconexión entre PLC, SCADA y gemelo digital.

## Contenido esperado

- `configuracion/` — Archivos de configuración del servidor OPC
- `mapeo-tags/` — Tablas de mapeo entre direcciones PLC y tags OPC

## Arquitectura

```
Studio 5000 / Logix Emulate
      ↕  OPC-UA
Ignition SCADA  ←→  Power BI / Python
      ↕  Señales I/O
NX Digital Factory / RobotStudio
```

## Responsables

Andrés Mauricio Morales Martínez · [@mora200217](https://github.com/mora200217)  
Juan Felipe Triana Aguilera · [@jutrianaa](https://github.com/jutrianaa)

<img src="https://raw.githubusercontent.com/ulogix-team/assets/main/banners/footer-dark.svg" width="100%"/>
