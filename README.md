euniprincez-digital-2026/
├── .gitignore
├── README.md
├── main.py
├── style.css
├── database/
│   └── triggers.sql
└── docs/
    ├── infraestructura_red.md
    └── numerologia_seguridad.md

# Euniprincez Digital 2026 — Valentín² (Esencia Potenciada)

## 👤 Autor e Identidad
* **Titular:** Juan Valentín García Espinoza
* **Concepto:** Valentín² (Esencia Potenciada)
* **Licencia:** © Todos los derechos reservados

---

## 📌 Descripción del Proyecto
Este repositorio centraliza el ecosistema tecnológico unificado de **Euniprincez Digital**, fusionando una arquitectura de red profesional segmentada (Capa Física y Lógica) con sistemas distribuidos automatizados en Python y capas avanzadas de seguridad transaccional en bases de datos relacionales.

---

## 🛠️ Arquitectura e Infraestructura de Red

El núcleo operativo se despliega sobre una topología de red con aislamiento lógico gestionada a través de Firewalls y Switches Administrables:

* **VLAN 10 (Administración):** Segmento `192.168.10.0/24` para la gestión de infraestructura crítica (Switches, Routers, APs).
* **VLAN 20 (Corporativa):** Segmento `192.168.20.0/24` donde residen los servidores de aplicaciones y bases de datos.
* **VLAN 30 (Videovigilancia):** Segmento `192.168.30.0/24` aislado exclusivamente para tráfico NVR y cámaras IP.
* **VLAN 40 (Visitas):** Segmento `192.168.40.0/24` con políticas estrictas de firewall que impiden el salto lateral (*Inter-VLAN routing*) hacia zonas seguras.

---

## 🔒 Capa de Seguridad SQL y Lógica Aplicada

Las transacciones de datos se encuentran blindadas mediante reglas restrictivas a nivel de motor de base de datos para prevenir inyecciones y errores lógicos:

1.  **Validación de Token Activo:** Implementación del trigger `TRG_Auditoria_Seguridad_Euniprincez` que restringe el acceso si el token criptográfico no cumple estrictamente con una longitud de **64 caracteres hexadecimales**.
2.  **Control Aritmético Bancario:** Auditoría automatizada que ejecuta un `ROLLBACK TRANSACTION` instantáneo si se detectan balances negativos acompañados por multiplicadores positivos.
3.  **Identidad Numerológica Integrada:** Algoritmos de validación basados en raíces digitales pitagóricas para consistencia del sistema:
    * *Identidad Personal:* 44
    * *Identidad Social:* 76
    * *Armonía / Misión:* 3

---

## 🚀 Despliegue Rápido (Módulo Python)

El script principal está diseñado para interactuar de forma segura dentro del perímetro de la **VLAN 20**.

### Requisitos Previos
```bash
