# Moises Giraldo · Ciberseguridad defensiva e Ingeniería de Software

Sitio personal para presentar mi formación en ciberseguridad defensiva, el interés en agentes de IA para apoyar el análisis de alertas y registros, proyectos de ingeniería de software y canales de contacto.

## Funcionalidades

- Inicio con enfoque en análisis defensivo proactivo, límites del servicio y formación en curso.
- Sobre mí con ruta de aprendizaje en ciberseguridad, ingeniería de software y sistemas; paneles desplegables y navegación por teclado.
- Galería de diez proyectos de software y fichas individuales con repositorios y demos cuando están configuradas. Incluye un caso de estudio educativo de ciberseguridad defensiva con su análisis y evidencias.
- Proceso propuesto para acordar alcance autorizado, revisar alertas y registros, priorizar hallazgos y comunicar observaciones.
- Contacto con validación del formulario y preparación de un borrador mediante `mailto:`. El envío se realiza desde el cliente de correo del visitante; no hay backend.
- Diseño adaptable, menú móvil y enlace para saltar al contenido.

Las portadas son ilustraciones representativas; no son capturas de las aplicaciones.

El portafolio distingue la formación en curso de la experiencia demostrable. La exploración de agentes de IA para flujos defensivos está en etapa de estudio y las recomendaciones requieren revisión humana.

## Tecnologías y requisitos

HTML, CSS y JavaScript sin framework, paquetes de producción ni compilación. Google Fonts es un recurso externo; hay fuentes alternativas locales.

Para desarrollo se necesita un navegador y Node.js para el servidor local y las comprobaciones de sintaxis. También puede usarse un servidor HTTP como Live Server. No se necesitan credenciales ni variables de entorno.

## Ejecutar

```sh
git clone https://github.com/ellmoi/portafolio-ciberseguridad-MoisesGiraldo.git
cd portafolio-ciberseguridad-MoisesGiraldo
node scripts/serve.cjs
```

Abrir <http://127.0.0.1:8080>. Detener con `Ctrl+C`. Usar HTTP: las fichas de proyecto cargan `proyectos.html` mediante `fetch` y no funcionan correctamente abriendo archivos con `file://`.

## Estructura

```text
*.html                 Páginas públicas
css/                   Estilos compartidos y por página
js/                    Navegación, áreas técnicas, proyectos y contacto
assets/                Imágenes del sitio y recursos visuales conservados
docs/                  Material de referencia
docs/ciberseguridad/   Casos de estudio defensivos organizados por módulo
docs/design/           Procedencia y prompts de las ilustraciones
scripts/serve.cjs      Servidor local sin dependencias
.github/               Validación y plantilla de Pull Request
```

`proyectos.html` es la fuente de datos de las fichas: los atributos `data-project`, `data-project-page` y `data-project-repository` definen sus enlaces. `tecnologias.html` conserva una redirección a Proyectos por compatibilidad.

El caso de estudio del Módulo 02 aparece en `proyectos.html`; sus entregables viven en `docs/ciberseguridad/modulo-02/`. El material de origen se trata como escenario académico: las afirmaciones no se presentan como hechos confirmados sin fuentes verificables.

## Verificación

No hay suite de pruebas, linter de terceros ni build. Comprobar la sintaxis con `node --check` para cada archivo de `js/` y `scripts/`, y ejecutar `git diff --check`.

Antes de integrar, revisar mediante HTTP las páginas modificadas en escritorio y móvil, los enlaces locales, las fichas de proyectos, el menú, las pestañas técnicas y la preparación del borrador de correo. GitHub Actions comprueba sintaxis y espacios en los cambios; no sustituye la revisión del navegador.

## Flujo de trabajo

`main` representa la versión estable. Crear ramas breves por tarea (`feature/`, `fix/`, `refactor/`, `docs/`, `test/`, `chore/`), verificar, realizar commits, publicar y abrir un Pull Request. Integrar únicamente con las verificaciones correctas. No se utiliza `develop`.

Los commits nuevos siguen Conventional Commits con descripción en español, por ejemplo `fix: corregir navegación móvil`. Las reglas de trabajo están en [AGENTS.md](AGENTS.md). El historial anterior se conserva.

## Publicación y estado

Sitio publicado: [Abrir el portafolio de Moises Giraldo](https://ellmoi.github.io/portafolio-ciberseguridad-MoisesGiraldo/).

El portafolio es estático y no requiere compilación de producción. GitHub Pages publica la versión configurada en el repositorio; la actualización puede tardar unos minutos tras cada despliegue. Los enlaces a demos dependen de proyectos externos; Superdeportivos BGA continúa identificado como demo en revisión.

## Contacto

[GitHub](https://github.com/ellmoi) · [LinkedIn](https://www.linkedin.com/in/moises-giraldo-7874b9283) · [Correo](mailto:moises10giraldo@gmail.com)
