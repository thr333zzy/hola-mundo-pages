# Hola mundo en GitHub Pages

Página estática que se publica sola en [GitHub Pages](https://pages.github.com/) cada vez que hay un push a `main`.

Sitio: https://thr333zzy.github.io/hola-mundo-pages/

## Cómo se despliega

1. Este repositorio guarda `index.html`.
2. El workflow `.github/workflows/deploy.yml` corre en cada push a `main`.
3. GitHub Actions empaqueta los archivos y los publica en GitHub Pages.
4. La página queda servida en la URL de arriba. El primer despliegue puede tardar un minuto.

No hace falta un servidor propio ni un token externo. El permiso lo da el `GITHUB_TOKEN` del workflow (`pages: write` e `id-token: write`).

## Cómo cambiar la página

Edita `index.html`, haz commit y súbelo a `main`:

```powershell
git add index.html
git commit -m "Actualizar la pagina"
git push
```

GitHub Actions vuelve a publicar el sitio con ese cambio.
