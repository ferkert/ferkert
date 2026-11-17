<img src="assets/banner.svg" width="100%" alt="ferkert, full-stack developer and apprentice trainer at Navigate AG, Karlsruhe">

Full-stack developer and apprentice trainer at [Navigate AG](https://navigate.de) in Karlsruhe.
I started out as an apprentice myself, have worked as a developer ever since and hold the German trainer certification (AEVO).

I build Symfony and Laravel applications, CMS-driven portals and progressive web apps, with Svelte and Vue on the front and REST APIs, data imports, charts and document pipelines behind them.
More and more of that work involves LLMs: retrieval-augmented chat on PostgreSQL and guardrails that keep the model on topic.
I also own the parts nobody sees: CI pipelines, static analysis, deployments and documentation.

### About me, as a `composer.json`

```json
{
    "name": "ferkert/ferkert",
    "description": "Full-stack developer and apprentice trainer from Karlsruhe",
    "type": "human",
    "require": {
        "php": "^7.0 || ^8.0",
        "symfony/framework-bundle": "^3.4 || ^4.4 || ^7.4 || ^8.1",
        "laravel/framework": "^10.0",
        "doctrine/orm": "^2.0 || ^3.0",
        "contao/core-bundle": "^4.13 || ^5.0"
    },
    "require-dev": {
        "phpstan/phpstan": "^2.0",
        "larastan/larastan": "^2.9",
        "rector/rector": "^2.0",
        "phpunit/phpunit": "^10.5"
    },
    "suggest": {
        "dependencytrack/dependency-track": "Knowing what is inside the software I ship",
        "mintplex-labs/anything-llm": "Self-hosted LLM experiments"
    },
    "config": {
        "editor": ["phpstorm", "vscode"],
        "shell": "fish",
        "pair-programmer": "claude-code"
    },
    "extra": {
        "career": ["apprentice", "developer", "apprentice trainer"],
        "certification": "AEVO"
    }
}
```

### What I work on

- **Symfony applications** from Symfony 3.4 on PHP 7.0 up to Symfony 8.1 on PHP 8.5, with Doctrine, Messenger, Security, Forms and Twig
- **Laravel applications** on Laravel 10 with Sanctum, queued jobs, notifications, Fractal transformers and a Vue 3 frontend built with Vite
- **AI features**: a RAG chatbot in plain PHP that chunks PDFs, stores 1024-dimensional embeddings in PostgreSQL with pgvector and an HNSW index, answers through an OpenAI-compatible model API and runs an LLM guard on both the question and the reply; plus self-hosted LLM experiments with AnythingLLM
- **CMS-driven portals** on Contao 5.7, TYPO3, WordPress and Weblication: Contao sites assembled from dozens of in-house bundles served from a private Composer repository, with versioned REST and JSON APIs, RSS feeds, AMP pages, sitemaps and a connector that plugs Laravel into Weblication
- **Svelte frontends**: Svelte 5 and TypeScript components inside Contao, built with Webpack Encore, for product configurators, calculators and form fields with input masking; a shared Svelte component library covered by Playwright component tests
- **Vue apps and PWAs**: an installable event app with Vue 3, TypeScript, Pinia, Vue Router and Tailwind CSS, with service worker, map and distance view, fed by a Symfony 7.4 JSON API with automatic cache invalidation; a search portal frontend with Vue 3, Vuex, autocomplete against an OpenAPI-described search API, D3.js knowledge maps and a Vite multi-page build with Handlebars partials
- **Market data and charts**: intraday, end-of-day and historical data pulled from external APIs, streamed over WebSockets with Node.js and turned into time-series charts
- **Data from many sources**: MariaDB, MySQL, PostgreSQL and SQL Server, sometimes all in one application
- **Document generation**: PDFs, spreadsheets and office files built with XSLT, mPDF, PhpSpreadsheet and LibreOffice
- **Quality gates in CI**: PHPStan, Larastan, Rector, PHP-CS-Fixer, PHP_CodeSniffer, PHPMD, PHPUnit, ESLint, Stylelint, Prettier, vue-tsc and security audits on every merge request
- **Shipping and docs**: GitLab CI, GitHub Actions, Docker, DDEV and Ansible; documentation as code with AsciiDoc, PlantUML and Doxygen

### Toolbox

<table>
  <tr>
    <td>backend</td>
    <td>
      <a href="https://www.php.net/"><img src="https://img.shields.io/badge/PHP-121a28?style=flat-square&logo=php&logoColor=f2b53a" alt="PHP"></a>
      <a href="https://symfony.com/"><img src="https://img.shields.io/badge/Symfony-121a28?style=flat-square&logo=symfony&logoColor=f2b53a" alt="Symfony"></a>
      <a href="https://laravel.com/"><img src="https://img.shields.io/badge/Laravel-121a28?style=flat-square&logo=laravel&logoColor=f2b53a" alt="Laravel"></a>
      <a href="https://www.doctrine-project.org/"><img src="https://img.shields.io/badge/Doctrine-121a28?style=flat-square&logo=doctrine&logoColor=f2b53a" alt="Doctrine"></a>
      <a href="https://twig.symfony.com/"><img src="https://img.shields.io/badge/Twig-121a28?style=flat-square" alt="Twig"></a>
      <a href="https://getcomposer.org/"><img src="https://img.shields.io/badge/Composer-121a28?style=flat-square&logo=composer&logoColor=f2b53a" alt="Composer"></a>
      <a href="https://www.w3.org/TR/xslt-30/"><img src="https://img.shields.io/badge/XSLT-121a28?style=flat-square&logo=xml&logoColor=f2b53a" alt="XSLT"></a>
      <a href="https://nodejs.org/"><img src="https://img.shields.io/badge/Node.js-121a28?style=flat-square&logo=nodedotjs&logoColor=f2b53a" alt="Node.js"></a>
      <a href="https://www.openapis.org/"><img src="https://img.shields.io/badge/OpenAPI-121a28?style=flat-square&logo=openapiinitiative&logoColor=f2b53a" alt="OpenAPI"></a>
    </td>
  </tr>
  <tr>
    <td>ai</td>
    <td>
      <a href="https://arxiv.org/abs/2005.11401"><img src="https://img.shields.io/badge/RAG-121a28?style=flat-square" alt="RAG"></a>
      <a href="https://github.com/pgvector/pgvector"><img src="https://img.shields.io/badge/pgvector-121a28?style=flat-square&logo=postgresql&logoColor=f2b53a" alt="pgvector"></a>
      <a href="https://cloud.ionos.com/managed/ai-model-hub"><img src="https://img.shields.io/badge/IONOS_AI_Model_Hub-121a28?style=flat-square&logo=ionos&logoColor=f2b53a" alt="IONOS AI Model Hub"></a>
      <a href="https://anythingllm.com/"><img src="https://img.shields.io/badge/AnythingLLM-121a28?style=flat-square" alt="AnythingLLM"></a>
    </td>
  </tr>
  <tr>
    <td>cms</td>
    <td>
      <a href="https://contao.org/"><img src="https://img.shields.io/badge/Contao-121a28?style=flat-square&logo=contao&logoColor=f2b53a" alt="Contao"></a>
      <a href="https://typo3.org/"><img src="https://img.shields.io/badge/TYPO3-121a28?style=flat-square&logo=typo3&logoColor=f2b53a" alt="TYPO3"></a>
      <a href="https://wordpress.org/"><img src="https://img.shields.io/badge/WordPress-121a28?style=flat-square&logo=wordpress&logoColor=f2b53a" alt="WordPress"></a>
      <a href="https://www.weblication.de/"><img src="https://img.shields.io/badge/Weblication-121a28?style=flat-square" alt="Weblication"></a>
    </td>
  </tr>
  <tr>
    <td>frontend</td>
    <td>
      <a href="https://svelte.dev/"><img src="https://img.shields.io/badge/Svelte-121a28?style=flat-square&logo=svelte&logoColor=f2b53a" alt="Svelte"></a>
      <a href="https://www.typescriptlang.org/"><img src="https://img.shields.io/badge/TypeScript-121a28?style=flat-square&logo=typescript&logoColor=f2b53a" alt="TypeScript"></a>
      <a href="https://ecma-international.org/publications-and-standards/standards/ecma-262/"><img src="https://img.shields.io/badge/JavaScript-121a28?style=flat-square&logo=javascript&logoColor=f2b53a" alt="JavaScript"></a>
      <a href="https://vuejs.org/"><img src="https://img.shields.io/badge/Vue.js-121a28?style=flat-square&logo=vuedotjs&logoColor=f2b53a" alt="Vue.js"></a>
      <a href="https://pinia.vuejs.org/"><img src="https://img.shields.io/badge/Pinia-121a28?style=flat-square&logo=pinia&logoColor=f2b53a" alt="Pinia"></a>
      <a href="https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps"><img src="https://img.shields.io/badge/PWA-121a28?style=flat-square&logo=pwa&logoColor=f2b53a" alt="PWA"></a>
      <a href="https://d3js.org/"><img src="https://img.shields.io/badge/D3.js-121a28?style=flat-square&logo=d3&logoColor=f2b53a" alt="D3.js"></a>
      <a href="https://tailwindcss.com/"><img src="https://img.shields.io/badge/Tailwind_CSS-121a28?style=flat-square&logo=tailwindcss&logoColor=f2b53a" alt="Tailwind CSS"></a>
      <a href="https://vite.dev/"><img src="https://img.shields.io/badge/Vite-121a28?style=flat-square&logo=vite&logoColor=f2b53a" alt="Vite"></a>
      <a href="https://getbootstrap.com/"><img src="https://img.shields.io/badge/Bootstrap-121a28?style=flat-square&logo=bootstrap&logoColor=f2b53a" alt="Bootstrap"></a>
      <a href="https://sass-lang.com/"><img src="https://img.shields.io/badge/Sass-121a28?style=flat-square&logo=sass&logoColor=f2b53a" alt="Sass"></a>
      <a href="https://symfony.com/doc/current/frontend/encore/index.html"><img src="https://img.shields.io/badge/Webpack_Encore-121a28?style=flat-square&logo=webpack&logoColor=f2b53a" alt="Webpack Encore"></a>
      <a href="https://jquery.com/"><img src="https://img.shields.io/badge/jQuery-121a28?style=flat-square&logo=jquery&logoColor=f2b53a" alt="jQuery"></a>
    </td>
  </tr>
  <tr>
    <td>data</td>
    <td>
      <a href="https://mariadb.org/"><img src="https://img.shields.io/badge/MariaDB-121a28?style=flat-square&logo=mariadb&logoColor=f2b53a" alt="MariaDB"></a>
      <a href="https://www.mysql.com/"><img src="https://img.shields.io/badge/MySQL-121a28?style=flat-square&logo=mysql&logoColor=f2b53a" alt="MySQL"></a>
      <a href="https://www.postgresql.org/"><img src="https://img.shields.io/badge/PostgreSQL-121a28?style=flat-square&logo=postgresql&logoColor=f2b53a" alt="PostgreSQL"></a>
      <a href="https://www.microsoft.com/sql-server"><img src="https://img.shields.io/badge/SQL_Server-121a28?style=flat-square" alt="SQL Server"></a>
    </td>
  </tr>
  <tr>
    <td>quality</td>
    <td>
      <a href="https://phpstan.org/"><img src="https://img.shields.io/badge/PHPStan-121a28?style=flat-square" alt="PHPStan"></a>
      <a href="https://github.com/larastan/larastan"><img src="https://img.shields.io/badge/Larastan-121a28?style=flat-square" alt="Larastan"></a>
      <a href="https://getrector.com/"><img src="https://img.shields.io/badge/Rector-121a28?style=flat-square" alt="Rector"></a>
      <a href="https://phpunit.de/"><img src="https://img.shields.io/badge/PHPUnit-121a28?style=flat-square" alt="PHPUnit"></a>
      <a href="https://playwright.dev/"><img src="https://img.shields.io/badge/Playwright-121a28?style=flat-square" alt="Playwright"></a>
      <a href="https://eslint.org/"><img src="https://img.shields.io/badge/ESLint-121a28?style=flat-square&logo=eslint&logoColor=f2b53a" alt="ESLint"></a>
      <a href="https://prettier.io/"><img src="https://img.shields.io/badge/Prettier-121a28?style=flat-square&logo=prettier&logoColor=f2b53a" alt="Prettier"></a>
      <a href="https://cs.symfony.com/"><img src="https://img.shields.io/badge/PHP--CS--Fixer-121a28?style=flat-square" alt="PHP-CS-Fixer"></a>
      <a href="https://stylelint.io/"><img src="https://img.shields.io/badge/Stylelint-121a28?style=flat-square" alt="Stylelint"></a>
    </td>
  </tr>
  <tr>
    <td>ops</td>
    <td>
      <a href="https://docs.gitlab.com/ci/"><img src="https://img.shields.io/badge/GitLab_CI-121a28?style=flat-square&logo=gitlab&logoColor=f2b53a" alt="GitLab CI"></a>
      <a href="https://github.com/features/actions"><img src="https://img.shields.io/badge/GitHub_Actions-121a28?style=flat-square&logo=githubactions&logoColor=f2b53a" alt="GitHub Actions"></a>
      <a href="https://www.docker.com/"><img src="https://img.shields.io/badge/Docker-121a28?style=flat-square&logo=docker&logoColor=f2b53a" alt="Docker"></a>
      <a href="https://ddev.com/"><img src="https://img.shields.io/badge/DDEV-121a28?style=flat-square" alt="DDEV"></a>
      <a href="https://docs.ansible.com/"><img src="https://img.shields.io/badge/Ansible-121a28?style=flat-square&logo=ansible&logoColor=f2b53a" alt="Ansible"></a>
      <a href="https://www.kernel.org/"><img src="https://img.shields.io/badge/Linux-121a28?style=flat-square&logo=linux&logoColor=f2b53a" alt="Linux"></a>
    </td>
  </tr>
  <tr>
    <td>docs</td>
    <td>
      <a href="https://asciidoc.org/"><img src="https://img.shields.io/badge/AsciiDoc-121a28?style=flat-square&logo=asciidoctor&logoColor=f2b53a" alt="AsciiDoc"></a>
      <a href="https://plantuml.com/"><img src="https://img.shields.io/badge/PlantUML-121a28?style=flat-square" alt="PlantUML"></a>
      <a href="https://www.doxygen.nl/"><img src="https://img.shields.io/badge/Doxygen-121a28?style=flat-square" alt="Doxygen"></a>
    </td>
  </tr>
  <tr>
    <td>daily</td>
    <td>
      <a href="https://www.jetbrains.com/phpstorm/"><img src="https://img.shields.io/badge/PhpStorm-121a28?style=flat-square&logo=phpstorm&logoColor=f2b53a" alt="PhpStorm"></a>
      <a href="https://code.visualstudio.com/"><img src="https://img.shields.io/badge/VS_Code-121a28?style=flat-square" alt="VS Code"></a>
      <a href="https://claude.com/product/claude-code"><img src="https://img.shields.io/badge/Claude_Code-121a28?style=flat-square&logo=claude&logoColor=f2b53a" alt="Claude Code"></a>
      <a href="https://fishshell.com/"><img src="https://img.shields.io/badge/fish-121a28?style=flat-square&logo=fishshell&logoColor=f2b53a" alt="fish shell"></a>
      <a href="https://git-scm.com/"><img src="https://img.shields.io/badge/Git-121a28?style=flat-square&logo=git&logoColor=f2b53a" alt="Git"></a>
    </td>
  </tr>
</table>
