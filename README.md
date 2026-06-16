# Forge Studio — ProjectTracker

An enterprise-style, single-file project workspace that takes a project from idea to
production — and an **Excalidraw-style infinite canvas** for designing the architecture.

Everything lives in one standalone `index.html`. No build step, no backend.

> **Open it:** double-click `index.html`, or visit the GitHub Pages site once enabled
> (Settings → Pages → deploy from `main`). Needs internet for the rough.js + fonts CDNs.

## What's inside

A single workspace that walks a project through its whole lifecycle:

| Section | What it does |
| --- | --- |
| **Goal** | The north-star statement, with full revision history. |
| **Build** | A 7-stage lifecycle (Plan → Design → Develop → Test → Deploy → Monitor → Scale & Secure), each stage offering curated tool choices with "best for" guidance. |
| **Stack** | Every chosen tool assembled into one integrated picture. |
| **Environments & preview** | Dev / Preview / Production with a live mock preview and one-click "deploy". |
| **Architecture** | A full hand-drawn infinite canvas — see below. |
| **Decisions** | Every tool choice logged with a *why*. |
| **Docs** | Living plan, milestones, and a discussion log. |
| **Versions** | An automatic checkpoint on every meaningful change. |
| **Overview** | The whole project on one printable page, including the architecture diagram. |

## The Architecture canvas (Excalidraw-style)

- **Tools:** select, hand/pan, rectangle, diamond, ellipse, arrow, line, freehand draw,
  text, eraser — with single-key shortcuts (`V H R D O A L P T E`).
- **Infinite canvas:** scroll to pan, ⌘/Ctrl-scroll or pinch to zoom, Space-drag to pan,
  plus zoom controls and **Fit to view**.
- **Hand-drawn rendering** via [rough.js](https://roughjs.com), set in the Kalam font.
- **Style panel:** stroke & background colour, fill style (hachure / cross-hatch / solid),
  stroke width, sloppiness, font size, opacity, and arrange (front / back / duplicate / delete).
- **Selection:** click, shift-multi-select, marquee, 8 resize handles, move, alt-drag to
  duplicate, arrow-key nudge.
- **Smart arrows** that bind to shapes — connect two boxes and the arrow follows when you move them.
- **Editing:** double-click to add a note or label any shape.
- **Undo/redo, copy/paste, right-click context menu.**
- **Component palette:** one-click stencils for User, Client, CDN, Load Balancer, API Gateway,
  Service, Worker, Database, Cache, Queue, Storage, Auth, and more.

The diagram saves into the project and renders as a fitted SVG on the **Overview** page.

## Tech

Plain HTML/CSS/JavaScript in one file. Only two external dependencies, both via CDN:
[rough.js](https://roughjs.com) for the hand-drawn rendering and Google Fonts (Geist + Kalam).
Dark and light themes included.
