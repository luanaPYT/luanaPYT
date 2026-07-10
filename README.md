<div align="center">

<h1>
  ✨ Fantasy Portal ✨
</h1>

<p>
  <b>Погружение в мир фэнтези — иммерсивный веб-портал, API и дизайн-канвас в одном монорепозитории.</b>
</p>

<p>
  <img src="https://img.shields.io/badge/pnpm-workspace-8B5CF6?style=for-the-badge&logo=pnpm&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-5.9-7C3AED?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-24-9333EA?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/React-Vite-A855F7?style=for-the-badge&logo=react&logoColor=white" />
  <img src="https://img.shields.io/badge/Express-5-6D28D9?style=for-the-badge&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-Drizzle-8B5CF6?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/License-MIT-C084FC?style=for-the-badge" />
</p>

</div>

<div align="center">

![purple divider](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=6&section=header)

</div>

## 💜 О проекте

**Fantasy Portal** — монорепозиторий на pnpm workspaces, объединяющий фронтенд-портал в фэнтезийной стилистике, backend API и песочницу для дизайна. Проект построен на строгой типизации, кодогенерации API из OpenAPI-спецификации и современном стеке.

<div align="center">

`⟡ ─────────────────────────────  ⟡  ───────────────────────────── ⟡`

</div>

## 🔮 Возможности

- 🎨 **Иммерсивный лендинг** — single-page портал на React + Vite с анимациями (Framer Motion) и компонентами Radix UI.
- ⚡ **Типобезопасный API** — Express 5 с валидацией через Zod и кодогенерацией клиента (Orval).
- 🗄️ **Надёжное хранение** — PostgreSQL + Drizzle ORM.
- 🧩 **Монорепо-архитектура** — общие библиотеки и строгие TypeScript project references.
- 🖌️ **Дизайн-канвас** — отдельная песочница для макетов и прототипов.

## 🛠️ Стек технологий

| Слой         | Технологии                                              |
| ------------ | ------------------------------------------------------- |
| **Фронтенд** | React, Vite, Tailwind CSS, Radix UI, Framer Motion      |
| **Бэкенд**   | Express 5, Pino, Zod (`zod/v4`)                         |
| **База данных** | PostgreSQL, Drizzle ORM                             |
| **Кодоген**  | Orval (из OpenAPI-спеки)                                |
| **Тулинг**   | pnpm workspaces, TypeScript 5.9, esbuild, Prettier      |

## 📂 Структура проекта

```text
.
├── artifacts/
│   ├── fantasy-portal/   💜 Веб-портал (React + Vite)
│   ├── api-server/       ⚡ API-сервер (Express 5)
│   └── mockup-sandbox/   🎨 Дизайн-канвас
├── lib/                  🧩 Общие библиотеки
├── scripts/              🛠️ Служебные скрипты
└── pnpm-workspace.yaml
```

## 🚀 Быстрый старт

```bash
# Установка зависимостей (только pnpm!)
pnpm install

# Запуск API-сервера (порт 5000)
pnpm --filter @workspace/api-server run dev

# Запуск фэнтези-портала
pnpm --filter @workspace/fantasy-portal run dev
```

### Полезные команды

```bash
pnpm run typecheck    # Проверка типов по всем пакетам
pnpm run build        # Typecheck + сборка всех пакетов
pnpm --filter @workspace/api-spec run codegen   # Кодоген хуков и Zod-схем
pnpm --filter @workspace/db run push            # Пуш схемы БД (только dev)
```

> **Требуется env:** `DATABASE_URL` — строка подключения к Postgres.

<div align="center">

`⟡ ─────────────────────────────  ⟡  ───────────────────────────── ⟡`

</div>

## 📜 Лицензия

Распространяется под лицензией **MIT**.

<div align="center">

<sub>Создано с 💜 в фэнтезийной стилистике</sub>

![purple footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=6&section=footer)

</div>
