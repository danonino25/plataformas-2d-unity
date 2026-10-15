# 🎮 Juego de Plataformas 2D en Unity

![Unity Version](https://img.shields.io/badge/Unity-6000.6.0f1-blue.svg)
![Render Pipeline](https://img.shields.io/badge/Render%20Pipeline-URP%202D-green.svg)
![Status](https://img.shields.io/badge/Estado-En%20Desarrollo-yellow.svg)

## 📌 Descripción del Proyecto
Este proyecto es un videojuego de plataformas en 2D desarrollado como parte de la asignatura de **Creación de Videojuegos**
El objetivo es construir un prototipo jugable aplicando conceptos fundamentales de física 2D, detección de suelo, manejo de spritesheets y controladores en C#.

---

## 🚀 Mecánicas e Implementaciones Técnicas

- **Controlador del Jugador (`JugadorController.cs`):** 
  - Movimiento horizontal responsivo mediante entradas del teclado.
  - Inversión automática del gráfico (*Flip X*) mediante modificación de la escala local en el eje X.
  - Mecánica de salto utilizando impulsos de física sobre el componente `Rigidbody2D`.
- **Sistema de Físicas y Colisiones:**
  - Configuración de `Rigidbody2D` con restricción de rotación en el eje Z (*Freeze Rotation Z*) para evitar caídas de costado.
  - Uso de `BoxCollider2D` en el jugador y en los bloques del escenario.
  - Detección dinámica de colisiones con el suelo mediante `OnCollisionEnter2D`.
- **Gestión de Assets:**
  - Importación y segmentación de *Spritesheets* de escenario y personajes utilizando el *Sprite Editor* de Unity.
  - Ajuste de filtros de textura (*Point / No Filter*) para renderizado nítido de gráficos.

---

## 🛠️ Tecnologías Utilizadas

- **Motor de Juego:** Unity Engine 6 (versión 6000.6.0f1 - 2D URP).
- **Lenguaje de Programación:** C# (.NET Core).
- **Editor de Código:** Visual Studio Code.
- **Control de Versiones:** Git & GitHub.
- **Assets Gráficos:** Kenney 2D Platformer Assets.

---

## 📂 Estructura del Repositorio

```text
JuegoPlataformas2D/
├── Assets/
│   ├── Scenes/          # Escenas del nivel (SampleScene)
│   ├── Scripts/         # Scripts en C# (JugadorController.cs)
│   ├── Settings/        # Configuraciones del Render Pipeline e Input System
│   └── Sprites/         # Spritesheets recortados de personajes y terreno
├── .gitignore           # Exclusión de archivos temporales de Unity
└── README.md            # Documentación del proyecto

## 🕹️ Controles del Juego

| Acción | Controles |
| :--- | :--- |
| **Mover a la Izquierda** | Flecha Izquierda / Tecla `A` |
| **Mover a la Derecha** | Flecha Derecha / Tecla `D` |
| **Saltar** | Barra Espaciadora (`Space`) |

---

## 👤 Autor

Desarrollado por **Ana María Barrientos Guerrero**
como evidencia de aprendizaje y proyecto de portafolio para la materia de **Creación de Videojuegos**
en la **Universidad Tecnológica del Norte de Guanajuato (UTNG)**.
