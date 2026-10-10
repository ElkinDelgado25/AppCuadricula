# App Cuadrícula (Courses App)

Práctica Experimental de Aprendizaje (PEA) para la asignatura **Aplicaciones Móviles Nativas** de la **Universidad Laica Eloy Alfaro de Manabí (ULEAM)**.

Basado en el Codelab oficial de Google: **[Android Basics with Compose - Practice: Build a grid](https://developer.android.com/codelabs/basic-android-kotlin-compose-practice-grid)**.

---

## 📱 Descripción del Proyecto

La aplicación **Courses** muestra una cuadrícula dinámica con desplazamiento que lista diversas áreas temáticas o cursos disponibles. La interfaz está construida completamente con **Jetpack Compose** y **Material 3**.

### 🎯 Objetivos y conceptos practicados
- **Cuadrículas optimizadas con Compose:** Uso del componente `LazyVerticalGrid` configurado con dos columnas fijas (`GridCells.Fixed(2)`).
- **Diseño de componentes modulares:** Creación de composables reutilizables como `TopicCard` para modelar cada tarjeta temática y `TopicGrid` para orquestar la lista.
- **Modelado de datos en Kotlin:** Definición de la clase inmutable `Topic` utilizando anotaciones de recursos (`@StringRes`, `@DrawableRes`).
- **Separación de responsabilidades:** Implementación de un objeto `DataSource` para desacoplar el origen de datos de la interfaz de usuario.
- **Manejo de recursos:** Integración de imágenes bitmap, iconos vectoriales XML (`ic_grain.xml`), recursos de texto en `strings.xml` y dimensiones unificadas en `dimens.xml`.

---

## 🛠️ Tecnologías y Requisitos

- **Lenguaje:** Kotlin
- **Toolkit UI:** Jetpack Compose (Material Design 3)
- **Minimum SDK:** API 24 (Android 7.0) / Target SDK: API 35
- **Gradle:** Kotlin DSL (`build.gradle.kts`)

---

## 📂 Estructura del Código

```text
app/src/main/
├── java/com/example/appcuadriculaamn/
│   ├── data/
│   │   └── DataSource.kt         # Catálogo de temas y cursos disponibles
│   ├── model/
│   │   └── Topic.kt              # Data class para representar cada ítem
│   ├── ui/theme/                 # Configuración de tema Material 3
│   └── MainActivity.kt           # Implementación de TopicCard, TopicGrid y Previews
└── res/
    ├── drawable/                 # Imágenes de los temas e icono decorativo
    ├── values/
    │   ├── dimens.xml            # Espaciados estándar (8dp, 16dp)
    │   └── strings.xml           # Cadenas de texto internacionalizadas
```

---

## 🚀 Repositorio

- **GitHub:** [https://github.com/ElkinDelgado25/AppCuadricula](https://github.com/ElkinDelgado25/AppCuadricula)