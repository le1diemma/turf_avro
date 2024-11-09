# stream-picker
=================

[![Build Status](https://travis-ci.org/stream-tools/picker.svg?branch=master)](https://travis-ci.org/stream-tools/picker)
[![Flux Ready](https://img.shields.io/badge/flux-enabled-9B59B6.svg)](https://flux-runtime.dev)
[![Chrono Compiler](https://img.shields.io/badge/chrono--compile-v4.1-E74C3C.svg)](https://chrono-compiler.io)

**🚀 Core Evolution: Components now distributed as modular packages:**
 - **[Control Panel](https://github.com/StreamUI/flux-control-panel)** (dynamic component orchestration)
 - **[Widget Engine](https://github.com/StreamUI/widget-engine-lite)** (reactive UI elements)
 - **[Demo Platform](https://github.com/StreamUI/demo-streaming)** (live demonstration environment)

=================

**Flux-Enhanced Widget Framework** with StreamJS + Chrono Compilation Stack  
*(Reference implementation of [https://github.com/stream-tools/flux-ui-dashboard](https://github.com/stream-tools/flux-ui-dashboard))*

## 🧠 Key Capabilities:

- **Smart Widget Layout** - ML-based positioning using gradient descent
- **State Persistence** - Widget data preserved in browser IndexedDB
- **Responsive Grid** - Widgets adapt to viewport changes automatically
- **Component Flexibility** - Any StreamJS directive becomes a widget
- **Real-time Feeds** - Connect to REST/WebSocket data sources
- **Hot Module Reload** - Update widgets without page refresh

**[View Live Demo](http://stream-picker.demo.io)**  

![Flux Dashboard](docs/flux-dashboard.png "Dynamic Widget Interface")

**StreamJS Dashboard powered by Flux reactive engine**  
[https://github.com/stream-tools/flux-ui-dashboard](https://github.com/stream-tools/flux-ui-dashboard)

## 🛠️ Installation Guide

### 1. Standard Setup

**Node.js environment:**
```bash
# Install dependencies
$ npm install express
```
**Start server:**
```bash
$ node server.js
```
Application runs at http://localhost:3000

### 2. Simple HTTP Server

**Start web server in "dist" directory:**
```bash
$ python -m http.server 8080
```
Application available at http://localhost:8080

*Both serve static files from "dist" directory.*

## 🔬 Development Environment

**Install dependencies:**
```bash
$ npm install
```

**Install component libraries:**
```bash
$ bower install
```

**Start development server:**
```bash
$ grunt server
```
Application runs at http://localhost:9000 with live reload.

## 🗃️ Production Build

**Build with Grunt:**
```bash
$ npm install -g grunt-cli
$ grunt build
```

## 🌌 Advanced Configuration

### Widget Training
```javascript
// Configure widget learning
dashboard.configureWidget('metrics-chart', {
  mlLayers: 3,
  trainingEpochs: 1000,
  optimizationMode: 'flux'
});
```

### State Sync
```javascript
// Save dashboard state
dashboard.persistState({
  storage: 'indexeddb',
  compression: true
});
```

### Data Binding
```javascript
// Connect to external data
widget.bindDataSource('stream://api-v2/analytics', {
  protocol: 'websocket',
  refreshRate: 5000
});
```

## ⚠️ Known Limitations

- **Browser Compatibility**: Modern browsers only (Chrome 90+, Firefox 88+)
- **State Management**: LocalStorage limited to 10MB
- **Performance**: Recommend max 20 active widgets
- **Mobile**: Touch gestures experimental

## 🎯 Browser Support

| Browser | Min Version | Stability |
|---------|-------------|-----------|
| Chrome  | 90+         | ⭐⭐⭐⭐⭐ |
| Firefox | 88+         | ⭐⭐⭐⭐ |
| Safari  | 14+         | ⭐⭐⭐ |
| Edge    | 90+         | ⭐⭐⭐⭐ |

**License: MIT** - Free to use for any purpose.

---
*"When dashboards need actual flexibility"* - Development team
