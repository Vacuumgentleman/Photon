## Photon Fusion 2 – Tutorial Project

  Photon Fusion 2 Tutorial Project es una implementación limpia y organizada del
  tutorial oficial de Fusion 2 para Unity. Incluye movimiento sincronizado,
  disparos, manejo del NetworkRunner y modos Host/Client. Ideal como base para
  proyectos multijugador más avanzados.

---

## Overview

  Este proyecto reproduce de forma estructurada el tutorial oficial de Photon
  Fusion 2, permitiendo entender cómo funciona la sincronización de jugadores,
  inputs, objetos instanciados en red y la gestión del NetworkRunner.  
  Incluye código modular, comentado y fácil de extender.

---

## Gameplay

- Movimiento del jugador sincronizado por ticks.
- Instanciación y disparo de proyectiles sincronizados.
- Rotación y acciones enviadas mediante PollInput.
- Comportamiento idéntico entre Host y Client.
- Escena cargada automáticamente mediante el Runner.
- Ejecución estable y óptima para pruebas multijugador.

---

## Multiplayer (Fusion 2 – Player Host)

- Iniciar como **Host** o unirse como **Client**.
- Sincronización completa de:
  - posición  
  - rotación  
  - inputs  
  - disparos  
  - spawn de objetos  
- Modo Shared disponible para pruebas locales.
- Arquitectura compatible con extensiones multijugador (lobby, matchmaking, equipos, etc.).

---

## Project Structure

folders:
  - Scripts
  - Scripts/Network
  - Scripts/Gameplay
  - Scripts/Input
  - Prefabs
  - Scenes
  - Fusion_Settings

principles:
  - Código limpio en C# siguiendo buenas prácticas.
  - Modularidad y separación de responsabilidades.
  - Sin `Debug.Log` innecesarios.
  - Prefabs registrados con NetworkObject.
  - Uso correcto de NetworkProjectConfig.

---

## Visual Style

- Elementos simples y funcionales para pruebas de red.
- UI mínima para Host / Client.
- Modelos básicos optimizados para sincronización.
- Diseño centrado en claridad del flujo multijugador.

---

## Controls

- **Move:** WASD  
- **Rotate / Aim:** Mouse  
- **Shoot:** Click izquierdo  
- **Start as Host:** Botón en UI  
- **Start as Client:** Botón en UI  

---

## How to Run


  - Abrir la escena principal del tutorial.
  - Configurar tu AppID en Photon Fusion (PhotonAppSettings).
  - Ejecutar el proyecto desde Unity.
  - Seleccionar "Host" para crear sesión.
  - Abrir otra instancia del juego y presionar "Client".
  - Probar movimiento y disparos sincronizados.

---

## Requirements

- Unity 2022.3 LTS o superior.
- Photon Fusion 2.x.
- AppID configurado desde el Photon Dashboard.
- .NET Framework 4.x.
- Conexión a internet para usar Photon Cloud.

---


