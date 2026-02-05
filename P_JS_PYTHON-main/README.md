# Curso Ingeniería de Software - JavaScript

Despliegue de JupyterLite con kernel JavaScript para enseñanza de fundamentos de software.

## 🚀 Uso

1. **Fork**: Haz fork de este repositorio
2. **GitHub Pages**: Ve a Settings > Pages > Source: GitHub Actions
3. **Espera**: El primer deploy toma ~2 minutos
4. **Accede**: `https://TU_USUARIO.github.io/nombre-repo/lab/index.html`

## 📚 Contenido

- **01_testing_tdd.ipynb**: Framework de testing propio, TDD básico
- **02_modulos_solid.ipynb**: Encapsulamiento, SRP, Strategy Pattern
- **03_patrones_eventos.ipynb**: Observer, EventEmitter, Async/Await
- **04_complejidad.ipynb**: Big O, Benchmarking, SVG visualización

## ⚠️ Limitaciones del Kernel JS

- No hay acceso a `window`, `document`, `alert()`
- Usar `return {...}` o `({"mime/type": ...})` para output visual
- `console.log()` va a la consola del navegador (F12), no a la celda
- Todo corre en Web Worker (aislado)

## 🛠 Desarrollo local

```bash
pip install jupyterlite-core jupyterlite-javascript-kernel
jupyter lite build --contents content
jupyter lite serve
