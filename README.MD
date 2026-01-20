# Aether 2.0

Интерактивная 3D визуализация частиц с поддержкой отслеживания рук и жестов.

![Aether 2.0](https://img.shields.io/badge/version-2.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## 🌟 Особенности

- **5 режимов визуализации**: Сфера, ДНК-спираль, Кольцо Сатурна, Тессеракт, Варп-туннель
- **Отслеживание рук**: Интеграция с MediaPipe Hands для управления жестами
- **Интерактивность**: Реакция на движение мыши и жесты рук
- **Настраиваемые параметры**: 
  - Плотность частиц (5k - 50k)
  - Фактор хаоса (0 - 1)
- **Современный UI**: Glassmorphism дизайн с эффектом размытия
- **Post-processing**: Bloom эффект для свечения частиц
- **Адаптивный дизайн**: Поддержка мобильных устройств

## 🚀 Быстрый старт

1. Клонируйте репозиторий:
```bash
git clone https://github.com/patricweb/AETHER.git
cd AETHER
```

2. Откройте `index.html` в современном браузере:
   - Chrome/Edge (рекомендуется)
   - Firefox
   - Safari

3. Нажмите кнопку **"Initialize Vision"** для активации камеры и отслеживания рук

## 📖 Использование

### Управление

- **Мышь**: Движение мыши влияет на вращение сцены и отталкивает частицы
- **Жесты рук**: 
  - Сжатый кулак - частицы сжимаются и становятся более плотными
  - Открытая ладонь - частицы расслабляются и плавно движутся
- **Кнопки форм**: Переключение между режимами визуализации
- **Слайдеры**: Настройка плотности частиц и фактора хаоса

### Режимы визуализации

1. **Sphere** (Сфера) - Классическая сферическая форма
2. **Helix** (ДНК) - Двойная спираль с вращением
3. **Saturn** (Кольцо) - Планета с кольцами
4. **Tesseract** (Куб) - Кубовая структура
5. **Warp Drive** (Туннель) - Анимированный туннель

## 🛠 Технологии

- **Three.js** (v0.160.0) - 3D графика и рендеринг
- **MediaPipe Hands** - Распознавание и отслеживание рук
- **WebGL Shaders** - Кастомные шейдеры для визуальных эффектов
- **ES Modules** - Современный JavaScript

## 📁 Структура проекта

```
AETHER/
├── index.html          # Основной файл приложения
├── README.MD          # Документация
└── LICENSE            # MIT License
```

## 🎨 Настройка

Вы можете изменить параметры в объекте `CONFIG`:

```javascript
const CONFIG = {
    count: 20000,                    // Количество частиц по умолчанию
    baseColor: new THREE.Color(0x00f2ff),    // Основной цвет (голубой)
    secondaryColor: new THREE.Color(0xbd00ff), // Вторичный цвет (фиолетовый)
    bloomParams: { 
        threshold: 0, 
        strength: 1.5, 
        radius: 0.5 
    }
};
```

## 🔧 Требования

- Современный браузер с поддержкой WebGL 2.0
- Камера (опционально, для отслеживания рук)
- Разрешение на использование камеры в браузере

## 📝 Лицензия

Этот проект распространяется под лицензией MIT. См. файл [LICENSE](LICENSE) для подробностей.

## 👤 Автор

**patricweb**

## 🙏 Благодарности

- [Three.js](https://threejs.org/) - Потрясающая библиотека для 3D графики
- [MediaPipe](https://mediapipe.dev/) - Решение для машинного обучения от Google

---

## English Version

# Aether 2.0

Interactive 3D particle visualization with hand tracking and gesture support.

## ✨ Features

- **5 Visualization Modes**: Sphere, DNA Helix, Saturn Ring, Tesseract, Warp Tunnel
- **Hand Tracking**: MediaPipe Hands integration for gesture control
- **Interactivity**: Responds to mouse movement and hand gestures
- **Customizable Parameters**:
  - Particle Density (5k - 50k)
  - Chaos Factor (0 - 1)
- **Modern UI**: Glassmorphism design with blur effects
- **Post-processing**: Bloom effect for particle glow
- **Responsive Design**: Mobile device support

## 🚀 Quick Start

1. Clone the repository:
```bash
git clone https://github.com/patricweb/AETHER.git
cd AETHER
```

2. Open `index.html` in a modern browser:
   - Chrome/Edge (recommended)
   - Firefox
   - Safari

3. Click the **"Initialize Vision"** button to activate camera and hand tracking

## 📖 Usage

### Controls

- **Mouse**: Mouse movement affects scene rotation and repels particles
- **Hand Gestures**:
  - Clenched fist - particles compress and become denser
  - Open palm - particles relax and move smoothly
- **Shape Buttons**: Switch between visualization modes
- **Sliders**: Adjust particle density and chaos factor

### Visualization Modes

1. **Sphere** - Classic spherical form
2. **Helix** - Double helix with rotation
3. **Saturn** - Planet with rings
4. **Tesseract** - Cubic structure
5. **Warp Drive** - Animated tunnel

## 🛠 Technologies

- **Three.js** (v0.160.0) - 3D graphics and rendering
- **MediaPipe Hands** - Hand recognition and tracking
- **WebGL Shaders** - Custom shaders for visual effects
- **ES Modules** - Modern JavaScript

## 📁 Project Structure

```
AETHER/
├── index.html          # Main application file
├── README.MD          # Documentation
└── LICENSE            # MIT License
```

## 🎨 Customization

You can modify parameters in the `CONFIG` object:

```javascript
const CONFIG = {
    count: 20000,                    // Default particle count
    baseColor: new THREE.Color(0x00f2ff),    // Primary color (cyan)
    secondaryColor: new THREE.Color(0xbd00ff), // Secondary color (purple)
    bloomParams: { 
        threshold: 0, 
        strength: 1.5, 
        radius: 0.5 
    }
};
```

## 🔧 Requirements

- Modern browser with WebGL 2.0 support
- Camera (optional, for hand tracking)
- Browser camera permission

## 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 👤 Author

**patricweb**

## 🙏 Acknowledgments

- [Three.js](https://threejs.org/) - Amazing 3D graphics library
- [MediaPipe](https://mediapipe.dev/) - Machine learning solution by Google

