# 🎮 Face Detection Game - OpenCV

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![C++](https://img.shields.io/badge/C++-17-blue.svg)](https://isocpp.org/)
[![OpenCV](https://img.shields.io/badge/OpenCV-4.x-red.svg)](https://opencv.org/)

Um jogo "catch the falling items" desenvolvido em **C++ com OpenCV** onde você coleta itens usando apenas os movimentos do seu **rosto**! Os itens caem do topo e você deve se mover para pegá-los. Cada item capturado vale pontos; os que caem no chão reduzem sua vida.

---

## 🎮 Mecânica do Jogo

| Elemento | Descrição |
|----------|-----------|
| 🧑 **Controle** | Mova o rosto para ESQUERDA ou DIREITA para mover o personagem |
| 📦 **Itens** | Caem do topo da tela em velocidades variadas |
| ✅ **Pegar item** | Personagem coleta o item → ganha **pontos** |
| ❌ **Deixar cair** | Item atinge o chão → perde **1 vida** |
| ❤️ **Vidas** | Começa com **3 vidas**. Quando chegar a 0 → **GAME OVER** |
| 🏆 **Pontuação** | Cada item capturado vale uma quantidade de pontos |

---

## ✨ Funcionalidades

- 🎯 **Controle facial em tempo real** - Mova o rosto para esquerda/direita para posicionar o personagem
- 📦 **Sistema de itens** - Itens caem com diferentes velocidades e valores de pontuação
- ❤️ **Sistema de vidas** - 3 vidas, perde uma a cada item que cai no chão
- 🏆 **Placar dinâmico** - Pontuação atualizada em tempo real na tela
- 📹 **Captura por webcam** - Processamento contínuo com OpenCV
- 🎮 **Interface gráfica simples** - Exibe personagem, itens, pontuação e vidas
- ⚡ **Baixa latência** - Otimizado para resposta rápida aos movimentos faciais

---

## 🛠️ Tecnologias Utilizadas

- **C++ 17** - Linguagem principal
- **OpenCV 4.x** - Detecção facial e captura de vídeo
- **SFML / SDL2** - Renderização do jogo e eventos

---

## 📂 Estrutura do Projeto
FaceDetectionGame-OpenCV/
│
├── src/
│   ├── main.cpp                 # Loop principal do jogo
│   ├── game.cpp                 # Lógica do jogo (itens, colisões, vidas)
│   ├── player.cpp               # Classe do personagem
│   └── item.cpp                 # Classe dos itens que caem
│
├── include/
│   ├── game.hpp
│   ├── player.hpp
│   ├── item.hpp
│   ├── face_detector.hpp        # Detecção facial com OpenCV
│   └── collision.hpp            # Detecção de colisão
│
├── assets/
│   ├── images/                  # Sprites e gráficos
│   ├── sounds/                  # Efeitos sonoros
│   └── fonts/                   # Fontes para texto
│
├── models/
│   └── haarcascade_frontalface_default.xml
│
├── CMakeLists.txt
├── Makefile
├── README.md
└── LICENSE
---

## ⚙️ Pré-requisitos

Antes de compilar o projeto, você precisa ter:

- **Compilador C++17** (g++ 7+ / clang 10+ / MSVC 2019+)
- **CMake 3.10+** ou **Make**
- **OpenCV 4.x** instalado
- **SFML** ou **SDL2** (para renderização do jogo)
- **Webcam** funcional
