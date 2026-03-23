<p align="center">
  <img src="https://raw.githubusercontent.com/ulogix-team/assets/main/dividers/divider-dark.svg" width="100%"/>
</p>

# 🔌 OPC — Comunicación OPC-UA

Configuración del servidor OPC-UA para interconexión entre PLC, SCADA y gemelo digital.

## Contenido esperado

- **configuracion/** — Archivos de configuración del servidor OPC (Ignition OPC-UA o KEPServer)
- **mapeo-tags/** — Tablas de mapeo entre direcciones PLC y tags OPC (`.csv`, `.xlsx`)

## Arquitectura de comunicación

```
Studio 5000 / Logix Emulate
        ↕  (OPC-UA)
Ignition SCADA  ←→  Power BI / Python
        ↕  (señales I/O)
NX Digital Factory / RobotStudio
```

## Responsable

Andrés M. Morales · [@mora200217](https://github.com/mora200217)  
Juan F. Triana · [@jutrianaa](https://github.com/jutrianaa)
