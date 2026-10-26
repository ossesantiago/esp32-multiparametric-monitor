# ESP32 Multiparametric Monitor

Monitor multiparamétrico portátil basado en **ESP32** para el registro y supervisión en tiempo real de variables fisiológicas (ECG, SpO2, presión arterial), con transmisión inalámbrica a una aplicación móvil.

> Trabajo Práctico Final de **Instrumentación Biomédica** – Ingeniería Biomédica, Universidad Nacional de Córdoba (UNC).

*English summary: portable multiparameter patient monitor built around an ESP32 that acquires ECG, SpO2 and blood pressure signals and streams them wirelessly to a mobile app for live visualization.*

---

## Descripción

El sistema utiliza un microcontrolador ESP32 como unidad central de procesamiento e interfaz entre los sensores biomédicos y una aplicación móvil. El ESP32 adquiere y acondiciona las señales, las procesa y las transmite de forma inalámbrica para su visualización en vivo.

## Variables medidas

| Variable | Sensor / módulo | Estado |
|----------|-----------------|--------|
| ECG | _[completar]_ | 🔲 Pendiente |
| SpO2 | _[completar]_ | 🔲 Pendiente |
| Presión arterial | _[completar]_ | 🔲 Pendiente |
| Otras | _[completar]_ | 🔲 Pendiente |

## Arquitectura general

```
 Sensores biomédicos ──► Acondicionamiento ──► ESP32 ──► BLE / Wi-Fi ──► App móvil
 (ECG, SpO2, PA)         de señal              (ADC,     (telemetría)    (visualización
                                               procesado)                 en vivo)
```

## Características

- Adquisición de ECG, SpO2 y presión arterial
- Acondicionamiento de señal analógica
- Procesamiento embebido en ESP32
- Transmisión inalámbrica de datos telemétricos
- Visualización en tiempo real en aplicación móvil
- Diseño portátil

## Hardware

- ESP32 _[modelo / placa de desarrollo]_
- Sensor de ECG _[completar]_
- Sensor de SpO2 _[completar]_
- Módulo de presión arterial _[completar]_
- Alimentación: _[batería / carga]_

## Estructura del repositorio

```
esp32-multiparametric-monitor/
├── firmware/      # Código del ESP32
├── hardware/      # Esquemáticos, PCB, lista de materiales (BOM)
├── app/           # Aplicación móvil
├── docs/          # Informe, diagramas, hojas de datos
├── images/        # Capturas y fotos del prototipo
└── README.md
```

## Puesta en marcha

### Requisitos

- [Arduino IDE](https://www.arduino.cc/en/software) o [PlatformIO](https://platformio.org/)
- Soporte de placas ESP32 instalado
- _[Librerías utilizadas]_

### Firmware

```bash
git clone https://github.com/<tu-usuario>/esp32-multiparametric-monitor.git
cd esp32-multiparametric-monitor/firmware
```

1. Abrir el proyecto en el IDE.
2. Seleccionar la placa ESP32 y el puerto correspondiente.
3. Compilar y cargar.

### Aplicación móvil

_[Instrucciones de instalación / uso de la app]_

## Resultados

_[Capturas de la app, señales adquiridas, fotos del prototipo]_

## Hoja de ruta

- [ ] Adquisición de ECG
- [ ] Adquisición de SpO2
- [ ] Medición de presión arterial
- [ ] Comunicación inalámbrica ESP32 ↔ app
- [ ] Visualización en vivo
- [ ] Pruebas y validación
- [ ] Informe final

## Aviso

Proyecto con fines **académicos y educativos**. No es un dispositivo médico certificado y no debe utilizarse para diagnóstico ni toma de decisiones clínicas.

## Autor

**Santiago** – Estudiante de Ingeniería Biomédica, UNC.
**Enzo** – Estudiante de Ingeniería Biomédica, UNC.
**Nahuel** – Estudiante de Ingeniería Biomédica, UNC.
