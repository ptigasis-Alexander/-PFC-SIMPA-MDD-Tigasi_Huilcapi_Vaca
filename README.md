# PFC-SIMPA-MDD-

Exposición y demostración práctica del ciclo completo de **Model-Driven Development (MDD)** aplicado al subsistema de **Monitoreo Fitosanitario y Gestión de Labores Agrícolas** del **SIMPA (Sistema Inteligente de Mantenimiento de Palma Africana)**, desarrollado para la asignatura **Ingeniería de Requisitos** de la **Universidad Técnica Estatal de Quevedo (UTEQ)**, período académico **2026–2027 PPA**.

---

# Integrantes del equipo

| Integrante | Fase liderada |
|------------|---------------|
| Tigasi Sampedro Paul Alexander | Marco teórico, redacción en LaTeX, README y referencias |
| Huilcapi [Leon Denisses Fabiola  | Configuración del generador, generación de código y Roundtrip Engineering |
| Vaca Romero David Octavio| Modelado UML, trazabilidad y verificación del modelo |

---

# Descripción del proyecto

El **SIMPA** es un sistema orientado a la gestión integral de plantaciones de palma africana. Entre sus principales funcionalidades se encuentran:

- Gestión de plantaciones.
- Gestión de lotes.
- Administración de trabajadores.
- Gestión de labores agrícolas.
- Monitoreo fitosanitario.
- Detección de plagas mediante Inteligencia Artificial.
- Generación de alertas.
- Recomendaciones de tratamiento.
- Predicción de cosechas.
- Generación de reportes.

En este proyecto se modela específicamente el subsistema de **Monitoreo Fitosanitario y Gestión de Labores Agrícolas**, compuesto por **11 clases de dominio**, utilizando la metodología **Model-Driven Development (MDD)**.

---

# Herramientas utilizadas

- Enterprise Architect 17.1.1716
- C# 12
- .NET 8
- Visual Studio 2026
- LaTeX

---

# Requisitos previos

Antes de ejecutar el proyecto se requiere disponer de:

- Enterprise Architect 17.1 con licencia académica.
- .NET SDK 8.0 o superior.
- Visual Studio 2022 o Visual Studio Code con C# Dev Kit.
- Windows 11 (Sistema operativo utilizado durante las pruebas).

---

# Estructura del proyecto

```text
PFC-SIMPA-MDD-LaGeneracionIA
│
├── modelo/
│   └── SIMPA_MDD.qea
│
├── generado/
│   └── Modelos/
│
├── docs/
│   ├── informe.tex
│   └── informe.pdf
│
├── evidencias/
│   └── video-demo.mp4
│
└── README.md
```

---

# Instrucciones de ejecución

## 1. Clonar el repositorio

```bash
git clone https://github.com/[usuario]/PFC-SIMPA-MDD-LaGeneracionIA.git
cd PFC-SIMPA-MDD
```

---

## 2. Abrir el modelo UML

Abrir el archivo:

```text
modelo/SIMPA_MDD.qea
```

mediante **Enterprise Architect**.

El paquete de trabajo corresponde a:

```text
Monitoreo Fitosanitario
```

---

## 3. Generar el código fuente

1. Seleccionar el paquete de clases.
2. Ir al menú:

```text
Generate
    └── Generate Code
```

3. Seleccionar el lenguaje **C#**.

El código generado se almacenará en:

```text
generado/Modelos/
```

---

## 4. Compilar el proyecto

Ubicarse dentro del proyecto generado.

```bash
cd generado
dotnet build
```

---

## 5. Ejecutar el proyecto

```bash
dotnet run
```

Si existen pruebas automatizadas:

```bash
dotnet test
```

---

# Demostración de Roundtrip Engineering

Para comprobar el funcionamiento del proceso de ingeniería inversa y sincronización:

1. Abrir la clase **Incidencia** en Enterprise Architect.
2. Agregar el atributo:

```text
coordenadasGPS : string
```

3. Regenerar el código.

4. Verificar que el archivo:

```text
generado/Modelos/Incidencia.cs
```

contiene la propiedad:

```csharp
public string CoordenadasGPS { get; set; }
```

---

# Compilación del informe LaTeX

Ubicarse en la carpeta:

```bash
cd docs
```

Compilar el documento:

```bash
pdflatex informe.tex
pdflatex informe.tex
```

Se recomienda utilizar **TeX Live** con el paquete:

```text
texlive-lang-spanish
```

El resultado será:

```text
docs/informe.pdf
```

---

# Video demostrativo

El video de respaldo se encuentra en:

```text
evidencias/video-demo.mp4
```

o mediante el enlace correspondiente (si aplica).

---

# Tecnologías utilizadas

- Enterprise Architect
- C#
- .NET 8
- GitHub
- LaTeX

---

# Resultados obtenidos

- Modelado del subsistema mediante UML.
- Generación automática de código C#.
- Demostración del proceso Model-Driven Development.
- Sincronización del modelo mediante Roundtrip Engineering.
- Elaboración del informe técnico en LaTeX.

---

# Distribución del trabajo

La distribución de responsabilidades individuales puede consultarse en:

- **Sección 11** del documento `docs/informe.pdf`
- Historial de commits del repositorio (**Insights → Contributors**)

---

