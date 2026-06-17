# OpenSpec Sandbox — Ejercicio Spec-Driven Development

## ✅ Evidencias

- **Node.js v20.19.0 o superior** (requisito de OpenSpec)

Verifica tu versión antes de empezar:

```bash
node --version
```

## ![alt text](image.png)

### 1. Instala la CLI de OpenSpec

```bash
npm install -g @fission-ai/openspec@latest
openspec --version   # debe responder con un número de versión
```

![alt text](image-1.png)

### 2. Inicializa OpenSpec en el sandbox

```bash
openspec init
```

En el asistente: selecciona tu copiloto (Claude Code, Cursor, Copilot…) y **acepta los defaults** del resto de prompts.

### 3. Verifica la estructura

```bash
ls -la
ls -R openspec/
```

![alt text](image-2.png)
![alt text](image-3.png)

Deberías ver el directorio `openspec/`, la carpeta de skills de tu copiloto (`.claude/skills/` o equivalente) y posiblemente `openspec/project.md`.

### 4. Explora (no escribas specs todavía)

- Lee `openspec/project.md` — la "constitución" del proyecto.
- Recorre el árbol de `openspec/`: ¿dónde van las propuestas? ¿los specs? ¿lo archivado?
- Date una vuelta por el workflow **propose → apply → archive** (OPSX) en la doc oficial. Solo familiarízate con el vocabulario.

---

## 📦 Observaciones

1. Revisando de alto nivel puedo ver que los archivos generados parece que revisan el estado actual del proyecto.
2. Nos ayudan con proponer un cambio antes de modificar el proyecto, lo cual es bueno para no generar regresiones.
3. Tenemos procesos para aplicar las propuestas o incluso omitir cuando ya fue completado o cerrado.

## 🗂️ Estructura esperada al terminar

```
.
├── openspec/              # generado por openspec init (evidencia)
├── .claude/skills/        # o el equivalente de tu copiloto
├── ENTREGA.md             # tu entregable
└── README.md
```

---

## 📚 Recursos

- **Doc oficial:** https://openspec.pro
- **Repo:** `fission-ai/openspec` en GitHub
- **Guía en español:** _Spec Driven Development con OpenSpec_ en webreactiva.com
- **Vídeo (opcional):** "Getting Started with OpenSpec | Spec Driven Development | Setup Tutorial" en YouTube
