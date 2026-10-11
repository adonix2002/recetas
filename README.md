# Mi Libro de Recetas V6 — Vercel + Supabase

Esta versión añade cuentas de usuario y base de datos online.

1. Crea un proyecto Supabase.
2. En Supabase > SQL Editor ejecuta `supabase/schema.sql`.
3. Sube este proyecto a GitHub.
4. En Vercel importa el repositorio.
5. Añade `NEXT_PUBLIC_SUPABASE_URL` y `NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY`.
6. Deploy.

Supabase Auth gestiona las cuentas y PostgreSQL guarda el índice y las recetas. Las políticas RLS hacen que cada usuario solo pueda acceder a sus propios registros.

La importación usa una función serverless de Vercel y prioriza Schema.org Recipe/JSON-LD.

Aún falta conectar almacenamiento de archivos para copiar físicamente las imágenes y añadir el generador PDF A4; las recetas pueden guardar de momento la URL de su imagen.
