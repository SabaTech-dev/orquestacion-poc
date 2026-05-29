# ⚡ Orquestación Multi-Agente POC — SabaTech

> Demo visual de arquitectura de orquestación multi-agente con 6 agentes especializados trabajando 24/7.

## 🎯 Qué es esto

POC (Proof of Concept) que demuestra el sistema de orquestación multi-agente de SabaTech:

- **6 agentes especializados** coordinados por Alfred (orquestador)
- **Pipeline automático**: Coder → Security → QA-Tester → Done
- **Kanban Board** en tiempo real con tracking de tareas
- **Heartbeat system** para monitoreo continuo 24/7
- **Hindsight Memory** para memoria persistente

## 🚀 Quick Start

### Opción 1: Docker (recomendado)

```bash
docker build -t orquestacion-poc .
docker run -p 8080:80 orquestacion-poc
# Abrir http://localhost:8080
```

### Opción 2: Servidor local

```bash
# Con Python
python3 -m http.server 8080

# Con Node.js
npx serve .

# Con PHP
php -S localhost:8080
```

Abrir `http://localhost:8080` en el navegador.

## 🤖 Arquitectura de Agentes

| Agente | Rol | Color |
|--------|-----|-------|
| 🎩 Alfred | Orchestrator / CEO | Púrpura |
| 💻 Coder | Implementation | Azul |
| 🛡️ Security | Audit & Review | Rojo |
| 🔧 DevOps | Infrastructure | Naranja |
| 🔬 Research | Analysis | Verde |
| ✅ QA-Tester | Quality | Amarillo |

## 🔄 Pipeline Automático

```
Backlog → Coder → Security → QA-Tester → Done
```

1. Las tareas entran al **Backlog**
2. **Coder** las implementa y mueve a review
3. **Security** audita y aprueba/rechaza
4. **QA-Tester** valida calidad
5. Tarea marcada como **Done** ✅

## 📋 Kanban Board

4 columnas con drag & drop conceptual:

- **Backlog** — Tareas pendientes
- **In Progress** — En desarrollo
- **Review** — En revisión (security/qa)
- **Done** — Completadas

## 💓 Heartbeat System

Cada agente reporta estado periódicamente:

| Campo | Value |
|-------|-------|
| Cycle | 24/7 continuo |
| Response Time | <2min |
| LLM Models | 12 fallbacks |
| Memory | Hindsight (persistent) |

## 📁 Estructura del Proyecto

```
orquestacion-poc/
├── index.html      # Landing page principal (self-contained)
├── Dockerfile      # Configuración Docker (nginx:alpine)
└── README.md       # Este archivo
```

## 🛠️ Stack Tecnológico

- **Frontend**: HTML5 + CSS3 (dark mode, responsive, animaciones)
- **Servidor**: nginx:alpine (Docker)
- **Datos**: Estáticos/demo (sin backend)

## ⚠️ Nota Importante

**Todos los datos mostrados son simulados/demo.**

Este POC es una demostración visual estática. En producción, los datos vendrían de:
- API de Kanban (Mission Control)
- WebSocket para heartbeat en tiempo real
- Base de datos con estado de agentes

## 📈 Próximos Pasos (Roadmap)

- [ ] Integrar API real de Kanban
- [ ] WebSocket para heartbeat en tiempo real
- [ ] Backend con Express/Fastify
- [ ] Integración con OpenClaw
- [ ] Dashboard interactivo con React/Vue

## 📄 Licencia

© 2026 SabaTech — Demo POC

## 🔗 Enlaces

- [SabaTech](https://sabatech.dev)
- [Contacto](https://sabatech.dev/contact)
