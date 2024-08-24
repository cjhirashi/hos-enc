# SISTEMA DE CONTROL - HOSPITAL GENERAL REGIONAL 216 CAMA, ENSENADA, BAJA CALIFORNIA

Proyecto ejecutivo de sistema de control y automatización de aire acondicionado

## UBICACIÓN

Av. Reforma S/N, colonia Jardines de chapultepec, CP 22785, Ensenada, Baja California, México

## DIAGRAMAS

### IAC,AZ01 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, AZOTEA, SECCIÓN 02**

### IAC,DC01 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, DIAGRAMA DE CONECTIVIDAD**

Diagramas de control de Unidades Manejadoras de aire

#### UMA-P1 | VENT-VV, EF-AH, FT-UV/PF

- Lista de cliente

    > - Sensor de temperatura en ducto de inyección
    > - Sensor de presión diferencial en ducto de inyección
    > - Relevador para el encendido de luz ultravioleta
    > - Monitoreo de la velocidad del ventilador VFD
    > - Alarma del estado del ventilador VFD
    > - Control de la velocidad del ventilador VFD
    > - Actuador de válvula en las tuberías de agua helada

- Lista sugerida

    > - Temperatura de suministro | `AI` | **TEM-D**
    > - Temperatura de retorno | `AI` | **TEM-D**
    > - Temperatura de area | `AI` | **TEM-C**
    > - Presión de suministro de aire | `AI` | **DPT**
    > - Arranque de ventilador | `DO` | **RL** + **B_RL**
    > - Confirmación de ventilador | `DI` | **CS**
    > - Control de velocidad | `AO`
    > - Control de válvula AH | `AO`
    > - Estado de válvula de AH | `AI`
    > - Activación de FIltración UV | `DO` | **RL** + **B_RL**
    > - Estado de Prefiltros | `DI` | **DPS**

    ======================================================

    EQUIPO | TIPO | AREA
    -------|------|-----
    **UMA-02-01** | UNIZONA | GOBIERNO

#### UMA-P2 | VENT-VV, EF-AH, FT-UV/PF/M12

- Lista de cliente

    > - Sensor de temperatura en ducto de inyección
    > - Sensor de presión diferencial en ducto de inyección
    > - Relevador para el encendido de luz ultravioleta
    > - Interruptor de presión diferencial, estado de los filtros MERV 12
    > - Monitoreo de velocidad del ventilador VFD
    > - Alarma del estado del ventilador VFD
    > - Control de la velocidad del ventilador VFD
    > - Relevador para el arranque y paro del motor del ventilador
    > - Actuador de válvula en las tuberías de agua helada

- Lista sugerida

    > - Temperatura de suministro | `AI` | **TEM-D**
    > - Temperatura de retorno | `AI` | **TEM-D**
    > - Temperatura de area | `AI` | **TEM-C**
    > - Presión de suministro de aire | `AI` | **DPT**
    > - Arranque de ventilador | `DO` | **RL** + **B_RL**
    > - Confirmación de ventilador | `DI` | **CS**
    > - Control de velocidad | `AO`
    > - Control de válvula AH | `AO`
    > - Estado de válvula de AH | `AI`
    > - Activación de FIltración UV | `DO` | **RL** + **B_RL**
    > - Estado de Prefiltros | `DI` | **DPS**
    > - Estado de Filtros Merv 12 | `DI` | **DPS**
    
    ======================================================

    EQUIPO | TIPO | AREA
    -------|------|-----
    **UMA-00-03** | UNIZONA | CONSULTA EXTARNA 1
    **UMA-00-04** | UNIZONA | SALA DE ESPERA, CONSULTA EXTERNA
    **UMA-00-09** | UNIZONA | SALA DE ESPERA, LABORATORIO
    **UMA-01-01** | UNIZONA | SALA ESPERA/CONS. EXTERNA 1
    **UMA-01-02** | UNIZONA | SALA ESPERA/CONS. EXTERNA 2
    **UMA-01-07** | UNIZONA | SALA DE ESPERA, ENDOSCOPIA
    **UMA-01-09** | UNIZONA | SALA DE ESPERA/CONSULTA EXTERNA 3
    **UMA-01-10** | UNIZONA | SALA DE ESPERA/CONSULTA EXTERNA 4

#### UMA-P3 | VENT-VV, EF-AH, FT-UV/PF/M12 EX-VC

- Lista de cliente

    > - Sensor de temperatura en ducto de inyección
    > - Sensor de presión diferencial en ducto de inyección
    > - Relevador para el encendido de luz ultravioleta
    > - Interruptor presión diferencial, estado de los filtros MERV 12
    > - Monitoreo de la velocidad del ventilador VFD
    > - Alarma del estado del ventilador VFD
    > - Control de la velocidad del ventilador VFD
    > - Relevador para el arranque y paro del motor del ventilador
    > - Actuador de válvula en las tuberías de agua helada
    > - Relevador arranque y paro del ventilador de extracción
    > - Sensor de corriente estado del ventilador de extracción

- Lista sugerida

    > - Temperatura de suministro | `AI` | **TEM-D**
    > - Temperatura de retorno | `AI` | **TEM-D**
    > - Temperatura de area | `AI` | **TEM-C**
    > - Presión de suministro de aire | `AI` | **DPT**
    > - Arranque de ventilador | `DO` | **RL** + **B_RL**
    > - Confirmación de ventilador | `DI` | **CS**
    > - Control de velocidad | `AO`
    > - Control de válvula AH | `AO`
    > - Estado de válvula de AH | `AI`
    > - Activación de FIltración UV | `DO` | **RL** + **B_RL**
    > - Estado de Prefiltros | `DI` | **DPS**
    > - Estado de Filtros Merv 12 | `DI` | **DPS**
    > - Arranque de extractor | `DO` | **RL** + **B_RL**
    > - Confirmación de extracto | `DI` | **CS**
    
    ======================================================

    EQUIPO | TIPO | AREA
    -------|------|-----
    **UMA-00-08** | UNIZONA | LABORATORIO

#### UMA-P4 | VENT-VV, EF-AH/DX, FT-UV/PF/M12/M15

- Lista de cliente

    > - Sensor de temperatura en ducto de inyección
    > - Sensor de presión diferencial en ducto de inyección
    > - Relevador para el encendido de luz ultravioleta
    > - Interruptor presión diferencial, estado de los filtros MERV 12
    > - Interruptor presión diferencial, estado de los filtros MERV 15
    > - Monitoreo de la velocidad del ventilador VFD
    > - Alarma del estado del ventilador VFD
    > - Control de la velocidad del ventilador VFD
    > - Relevador para el arranque y paro del motor del ventilador
    > - Actuador de válvula en las tuberías de agua helada
    > - Arranque y paro de la unidad condensadora
    > - Estado de la unidad condensadora

- Lista sugerida

    > - Temperatura de suministro | `AI` | **TEM-D**
    > - Temperatura de retorno | `AI` | **TEM-D**
    > - Temperatura de area | `AI` | **TEM-C**
    > - Presión de suministro de aire | `AI` | **DPT**
    > - Arranque de ventilador | `DO` | **RL** + **B_RL**
    > - Confirmación de ventilador | `DI` | **CS**
    > - Control de velocidad | `AO`
    > - Control de válvula AH | `AO`
    > - Estado de válvula de AH | `AI`
    > - Activación de FIltración UV | `DO` | **RL** + **B_RL**
    > - Estado de Prefiltros | `DI` | **DPS**
    > - Estado de Filtros Merv 12 | `DI` | **DPS**
    > - Estado de Filtros Merv 15 | `DI` | **DPS**
    > - Arranque de condensadora | `DO` | **RL** + **B_RL**
    > - Confirmación de condensadora | `DI` | **CS**
    
    ======================================================

    EQUIPO | TIPO | AREA
    -------|------|-----
    **UMA-00-01DX** | UNIZONA | TOMOGRAFO

#### UMA-P5 | VENT-VV, EF-AH/AC/DX, FT-UV/PF/M12/M15

- Lista de cliente

    > - Sensor de temperatura en ducto de inyección
    > - Sensor de presión diferencial en ducto de inyección
    > - Relevador para el encendido de luz ultravioleta
    > - Interruptor presión diferencial, estado de los filtros MERV 12
    > - Interruptor presión diferencial, estado de los filtros MERV 15
    > - Monitoreo de la velocidad del ventilador VFD
    > - Alarma del estado del ventilador VFD
    > - Control de la velocidad del ventilador VFD
    > - Relevador para el arranque y paro del motor del ventilador
    > - Actuador de válvula en las tuberías de agua helada
    > - Actuador de válvula en las tuberías de agua condensada
    > - Arranque y paro de la unidad condensadora
    > - Estado de la unidad condensadora

- Lista sugerida

    > - Temperatura de suministro | `AI` | **TEM-D**
    > - Temperatura de retorno | `AI` | **TEM-D**
    > - Temperatura de area | `AI` | **TEM-C**
    > - Presión de suministro de aire | `AI` | **DPT**
    > - Arranque de ventilador | `DO` | **RL** + **B_RL**
    > - Confirmación de ventilador | `DI` | **CS**
    > - Control de velocidad | `AO`
    > - Control de válvula AH | `AO`
    > - Estado de válvula de AH | `AI`
    > - Control de válvula AC | `AO`
    > - Estado de válvula de AC | `AI`
    > - Activación de FIltración UV | `DO` | **RL** + **B_RL**
    > - Estado de Prefiltros | `DI` | **DPS**
    > - Estado de Filtros Merv 12 | `DI` | **DPS**
    > - Estado de Filtros Merv 15 | `DI` | **DPS**
    > - Arranque de condensadora | `DO` | **RL** + **B_RL**
    > - Confirmación de condensadora | `DI` | **CS**
    
    ======================================================

    EQUIPO | TIPO | AREA
    -------|------|-----
    **UMA-01-04DX** | UNIZONA | TOMOGRAFO

#### UMA-P6 | VENT-VV, EF-AH/AC/DX, FT-UV/PF/M12/M17 EX-VC

- Lista de cliente

    > - Sensor de temperatura en ducto de inyección
    > - Sensor de presión diferencial en ducto de inyección
    > - Relevador para el encendido de luz ultravioleta
    > - Interruptor presión diferencial, estado de los filtros MERV 12
    > - Interruptor presión diferencial, estado de los filtros MERV 17
    > - Monitoreo de la velocidad del ventilador VFD
    > - Alarma del estado del ventilador VFD
    > - Control de la velocidad del ventilador VFD
    > - Relevador para el arranque y paro del motor del ventilador
    > - Actuador de válvula en las tuberías de agua helada
    > - Actuador de válvula en las tuberías de agua condensada
    > - Relevador arranque y paro del ventilador de extracción
    > - Sensor de corriente estado del ventilador de extracción
    > - Arranque y paro de la unidad condensadora
    > - Estado de la unidad condensadora

- Lista sugerida

    > - Temperatura de suministro | `AI` | **TEM-D**
    > - Temperatura de retorno | `AI` | **TEM-D**
    > - Temperatura de area | `AI` | **TEM-C**
    > - Presión de suministro de aire | `AI` | **DPT**
    > - Arranque de ventilador | `DO` | **RL** + **B_RL**
    > - Confirmación de ventilador | `DI` | **CS**
    > - Control de velocidad | `AO`
    > - Control de válvula AH | `AO`
    > - Estado de válvula de AH | `AI`
    > - Control de válvula AC | `AO`
    > - Estado de válvula de AC | `AI`
    > - Activación de FIltración UV | `DO` | **RL** + **B_RL**
    > - Estado de Prefiltros | `DI` | **DPS**
    > - Estado de Filtros Merv 12 | `DI` | **DPS**
    > - Estado de Filtros Merv 17 | `DI` | **DPS**
    > - Arranque de condensadora | `DO` | **RL** + **B_RL**
    > - Confirmación de condensadora | `DI` | **CS**
    > - Arranque de extractor | `DO` | **RL** + **B_RL**
    > - Confirmación de extractor | `DI` | **CS**
    
    ======================================================

    EQUIPO | TIPO | AREA
    -------|------|-----
    **UMA-01-05DX** | UNIZONA | SALA DE PROCEDIMIENTOS
    **UMA-01-06DX** | UNIZONA | SALA DE CIRUGIA AMBULATORIA

### IAC,DC02 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, DIAGRAMA DE CONECTIVIDAD**

#### UMA-P7 | VENT-VV, EF-AH, FT-UV/PF/M12/M15

- Lista de cliente

    > - Sensor de temperatura en ducto de inyección
    > - Sensor de presión diferencial en ducto de inyección
    > - Relevador para el encendido de luz ultravioleta
    > - Interruptor presión diferencial, estado de los filtros MERV 12
    > - Interruptor presión diferencial, estado de los filtros MERV 15
    > - Monitoreo de la velocidad del ventilador VFD
    > - Alarma del estado del ventilador VFD
    > - Control de la velocidad del ventilador VFD
    > - Relevador para el arranque y paro del motor del ventilador
    > - Actuador de válvula en las tuberías de agua helada

- Lista sugerida

    > - Temperatura de suministro | `AI` | **TEM-D**
    > - Temperatura de retorno | `AI` | **TEM-D**
    > - Temperatura de area | `AI` | **TEM-C**
    > - Presión de suministro de aire | `AI` | **DPT**
    > - Arranque de ventilador | `DO` | **RL** + **B_RL**
    > - Confirmación de ventilador | `DI` | **CS**
    > - Control de velocidad | `AO`
    > - Control de válvula AH | `AO`
    > - Estado de válvula de AH | `AI`
    > - Activación de FIltración UV | `DO` | **RL** + **B_RL**
    > - Estado de Prefiltros | `DI` | **DPS**
    > - Estado de Filtros Merv 12 | `DI` | **DPS**
    > - Estado de Filtros Merv 15 | `DI` | **DPS**

    ======================================================

    EQUIPO | TIPO | AREA
    -------|------|-----
    **UMA-01-03** | UNIZONA | ENDOSCOPIAS

#### UMA-P8 | VENT-VV, EF-AH, FT-UV/PF/M12/M15 EX-VC

- Lista de cliente

    > - Sensor de temperatura en ducto de inyección
    > - Sensor de presión diferencial en ducto de inyección
    > - Relevador para el encendido de luz ultravioleta
    > - Interruptor presión diferencial, estado de los filtros MERV 12
    > - Interruptor presión diferencial, estado de los filtros MERV 15
    > - Monitoreo de la velocidad del ventilador VFD
    > - Alarma del estado del ventilador VFD
    > - Control de la velocidad del ventilador VFD
    > - Relevador para el arranque y paro del motor del ventilador
    > - Actuador de válvula en las tuberías de agua helada
    > - Relevador arranque y paro del ventilador de extracción
    > - Sensor de corriente estado del ventilador de extracción

- Lista sugerida

    > - Temperatura de suministro | `AI` | **TEM-D**
    > - Temperatura de retorno | `AI` | **TEM-D**
    > - Temperatura de area | `AI` | **TEM-C**
    > - Presión de suministro de aire | `AI` | **DPT**
    > - Arranque de ventilador | `DO` | **RL** + **B_RL**
    > - Confirmación de ventilador | `DI` | **CS**
    > - Control de velocidad | `AO`
    > - Control de válvula AH | `AO`
    > - Estado de válvula de AH | `AI`
    > - Activación de FIltración UV | `DO` | **RL** + **B_RL**
    > - Estado de Prefiltros | `DI` | **DPS**
    > - Estado de Filtros Merv 12 | `DI` | **DPS**
    > - Estado de Filtros Merv 15 | `DI` | **DPS**
    > - Arranque de extractor | `DO` | **RL** + **B_RL**
    > - Confirmación de extractor | `DI` | **CS**

    ======================================================

    EQUIPO | TIPO | AREA
    -------|------|-----
    **UMA-00-05** | UNIZONA | QUIMIOTERAPIA/DIALISIS
    **UMA-00-07** | UNIZONA | CLINICA DE HERIDAS

#### UMA-P8 | VENT-VV, EF-AH, FT-UV/PF/M12/M15 EX1-VC EX2-VC EX3-VC EX4-VC

- Lista de cliente

    > - Sensor de temperatura en ducto de inyección
    > - Sensor de presión diferencial en ducto de inyección
    > - Relevador para el encendido de luz ultravioleta
    > - Interruptor presión diferencial, estado de los filtros MERV 12
    > - Interruptor presión diferencial, estado de los filtros MERV 15
    > - Monitoreo de la velocidad del ventilador VFD
    > - Alarma del estado del ventilador VFD
    > - Control de la velocidad del ventilador VFD
    > - Relevador para el arranque y paro del motor del ventilador
    > - Actuador de válvula en las tuberías de agua helada
    > - Relevador arranque y paro del ventilador de extracción 1
    > - Sensor de corriente estado del ventilador de extracción 1
    > - Relevador arranque y paro del ventilador de extracción 2
    > - Sensor de corriente estado del ventilador de extracción 2
    > - Relevador arranque y paro del ventilador de extracción 3
    > - Sensor de corriente estado del ventilador de extracción 3
    > - Relevador arranque y paro del ventilador de extracción 4
    > - Sensor de corriente estado del ventilador de extracción 4

- Lista sugerida

    > - Temperatura de suministro | `AI` | **TEM-D**
    > - Temperatura de retorno | `AI` | **TEM-D**
    > - Temperatura de area | `AI` | **TEM-C**
    > - Presión de suministro de aire | `AI` | **DPT**
    > - Arranque de ventilador | `DO` | **RL** + **B_RL**
    > - Confirmación de ventilador | `DI` | **CS**
    > - Control de velocidad | `AO`
    > - Control de válvula AH | `AO`
    > - Estado de válvula de AH | `AI`
    > - Activación de FIltración UV | `DO` | **RL** + **B_RL**
    > - Estado de Prefiltros | `DI` | **DPS**
    > - Estado de Filtros Merv 12 | `DI` | **DPS**
    > - Estado de Filtros Merv 15 | `DI` | **DPS**
    > - Arranque de extractor 1 | `DO` | **RL** + **B_RL**
    > - Confirmación de extractor 1 | `DI` | **CS**
    > - Arranque de extractor 2 | `DO` | **RL** + **B_RL**
    > - Confirmación de extractor 2 | `DI` | **CS**
    > - Arranque de extractor 3 | `DO` | **RL** + **B_RL**
    > - Confirmación de extractor 3 | `DI` | **CS**
    > - Arranque de extractor 4 | `DO` | **RL** + **B_RL**
    > - Confirmación de extractor 4 | `DI` | **CS**

    ======================================================

    EQUIPO | TIPO | AREA
    -------|------|-----
    **UMA-00-06** | UNIZONA | HEMODIALISIS

#### PLANTA DE AGUA HELADA

- Lista de cliente

    > 3 CHILLERS
    >
    > 3 BOMBAS DE AGUA HELADA, CIRCUITO PRIMARIO (BOMBEO CONSTANTE)
    >
    > 3 BOMBAS DE AGUA HELADA, CIRCUITO SECUNDARIO (BOMBEO VARIABLE)

- Lista sugerida

    > - Temperatura de suministro de agua | `AI` | **TEM-D**
    > - Temperatura de retorno de agua | `AI` | **TEM-D**
    > - Presión diferencial en circuito de agua | `AI`| **DPT-A**
    > - Arranque de Chiller 1 | `DO` | **RL** + **B_RL**
    > - Estado de Chiller 1 | `DI` | **CS**
    > - Arranque de Chiller 2 | `DO` | **RL** + **B_RL**
    > - Estado de Chiller 2 | `DI` | **CS**
    > - Arranque de Chiller 3 | `DO` | **RL** + **B_RL**
    > - Estado de Chiller 3 | `DI` | **CS**
    > - Arranque de BP 1 | `DO` | **RL** + **B_RL**
    > - Estado de BP 1 | `DI` | **CS**
    > - Arranque de BP 2 | `DO` | **RL** + **B_RL**
    > - Estado de BP 2 | `DI` | **CS**
    > - Arranque de BP 3 | `DO` | **RL** + **B_RL**
    > - Estado de BP 3 | `DI` | **CS**
    > - Arranque de BS 1 | `DO` | **RL** + **B_RL**
    > - Estado de BS 1 | `DI` | **CS**
    > - Control de velocidad BS 1 | `AO`
    > - Arranque de BS 2 | `DO` | **RL** + **B_RL**
    > - Estado de BS 2 | `DI` | **CS**
    > - Control de velocidad BS 2 | `AO`
    > - Arranque de BS 3 | `DO` | **RL** + **B_RL**
    > - Estado de BS 3 | `DI` | **CS**
    > - Control de velocidad BS 3 | `AO`
    

#### PLANTA DE AGUA CONDENSADOS

    Este sistema lo marcan como Modbus, ¿Este lo dejamos como BACnet?

- Lista de cliente

    > 2 TORRES DE ENFRIAMIENTO
    >
    > 3 BOMBAS DE AGUA CONDENSADOS (BOMBEO CONSTANTE)

- Lista sugerida

    > - Temperatura de suministro de agua | `AI` | **TEM-D**
    > - Temperatura de retorno de agua | `AI` | **TEM-D**
    > - Presión diferencial en circuito de agua | `AI`| **DPT-A**
    > - Arranque de Torre 1 | `DO` | **RL** + **B_RL**
    > - Estado de Torre 1 | `DI` | **CS**
    > - Arranque de Torre 2 | `DO` | **RL** + **B_RL**
    > - Estado de Torre 2 | `DI` | **CS**
    > - Arranque de BP 1 | `DO` | **RL** + **B_RL**
    > - Estado de BP 1 | `DI` | **CS**
    > - Arranque de BP 2 | `DO` | **RL** + **B_RL**
    > - Estado de BP 2 | `DI` | **CS**
    > - Arranque de BP 3 | `DO` | **RL** + **B_RL**
    > - Estado de BP 3 | `DI` | **CS**

12. ***UNIDAD LIGERA DE PLAFON***

    ¿Este sistema se va a controlar?

13. ***UNIDADES FAN & COIL***

    ¿Este sistema se va a controlar?

14. ***UNIDAD PAQUETE***

    ¿Este sistema se va a controlar?

15. ***CONEXION SERPENTIN-CONDENSADOR MAYOR A 10 TONELADAS DE REFRIGERACION***

    ¿Este sistema se va a controlar?

16. ***CONEXION SERPENTIN-CONDENSADOR MENOR A 10 TONELADAS DE REFRIGERACION***

    ¿Este sistema se va a controlar?

### IAC001 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PLANTA BAJA, SECCIÓN 01**

### IAC002 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PLANTA BAJA, SECCIÓN 02**

### IAC005 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PLANTA BAJA, SECCIÓN 05**

### IAC006 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PLANTA BAJA, SECCIÓN 06**

### IAC007 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PLANTA BAJA, SECCIÓN 07**

### IAC008 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PLANTA BAJA, SECCIÓN 08**

### IAC009 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PLANTA BAJA, SECCIÓN 09**

### IAC010 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PLANTA BAJA, SECCIÓN 10**

### IAC011 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PLANTA BAJA, SECCIÓN 11**

### IAC102 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PRIMER NIVEL, SECCIÓN 02**

### IAC103 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PRIMER NIVEL, SECCIÓN 03**

### IAC104 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PRIMER NIVEL, SECCIÓN 04**

### IAC105 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PRIMER NIVEL, SECCIÓN 05**

### IAC106 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, PRIMER NIVEL, SECCIÓN 06**

### IAC201 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, SEGUNDO NIVEL, SECCIÓN 01**

### IAC202 

**SISTEMA DE CONTROL DE AIRE ACONDICIONADO, SEGUNDO NIVEL, SECCIÓN 02**