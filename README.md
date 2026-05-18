# 🐾 Pets Media

**Pets Media** es una red social estilo Instagram diseñada exclusivamente para mascotas y sus dueños. Comparte fotos de tu peludo favorito, dale likes a las publicaciones de otros, y descubre las mascotas más populares en el ranking.

---

## Funcionalidades

- **Feed** — Explora las fotos más recientes de mascotas de toda la comunidad.
- **Crear post** — Sube una foto de tu mascota con un caption desde tu dispositivo.
- **Top Mascotas** — Ranking de las publicaciones con más likes en formato grilla.
- **Likes** — Reacciona a las publicaciones que más te gusten.

## Tecnologías

| Capa | Tecnología |
|------|-----------|
| Frontend | Next.js 16 (App Router) + TypeScript |
| Estilos | Tailwind CSS |
| Backend | Supabase (PostgreSQL + Storage) |
| Deploy | Vercel |

## Estructura de la app

```
app/
├── page.tsx          # Feed principal
├── post/page.tsx     # Crear publicación
├── rank/page.tsx     # Ranking de mascotas
└── utils/
    ├── client.ts     # Cliente de Supabase
    └── time.ts       # Utilidad de fechas relativas
```

## Variables de entorno

Crea un archivo `.env` en la raíz con:

```env
NEXT_PUBLIC_SUPABASE_URL=tu_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=tu_anon_key
```

## Comenzar

```bash
npm install
npm run dev
```

Abre [http://localhost:3000](http://localhost:3000) en tu navegador.

## Recursos

- [Documentación de Next.js](https://nextjs.org/docs)
- [Documentación de Supabase](https://supabase.com/docs)
- [Curso de Supabase — Platzi](https://platzi.com)
