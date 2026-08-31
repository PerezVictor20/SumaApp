# ➕ SumaApp

**SumaApp** es una aplicación nativa de Android desarrollada en **Kotlin** diseñada para realizar operaciones aritméticas sencillas (sumas) con una interfaz limpia, ágil y moderna.

---

## 🚀 Características

- 📱 **Interfaz Intuitiva:** Entrada rápida de datos y visualización clara de resultados.
- ⚡ **Compilación Moderna:** Utiliza **Gradle 8.13** y **Kotlin DSL (`build.gradle.kts`)**.
- 🛠️ **Preparada para Debug:** Generación directa de APKs ejecutables (`app-debug.apk`).

---

## 📁 Estructura del Proyecto

```text
SumaApp/
├── app/                      # Módulo principal de la aplicación
│   ├── build.gradle.kts      # Configuración de dependencias y entorno Android
│   └── build/outputs/apk/    # Binarios generados (app-debug.apk)
├── .gradle/                  # Caché y archivos de trabajo de Gradle (v8.13)
└── .gitignore                # Reglas de exclusión para Git
