<p align="center">
  <img src="https://img.icons8.com/external-tal-revivo-regular-tal-revivo/96/external-readme-is-a-easy-to-build-a-developer-hub-that-adapts-to-the-user-logo-regular-tal-revivo.png" width="100" />
</p>
<p align="center">
    <h1 align="center">TCPCHAT</h1>

<p align="center">
	<img src="https://img.shields.io/github/license/FlewToL/tcpchat?style=flat&color=0080ff" alt="license">
	<img src="https://img.shields.io/github/last-commit/FlewToL/tcpchat?style=flat&logo=git&logoColor=white&color=0080ff" alt="last-commit">
	<img src="https://img.shields.io/github/languages/top/FlewToL/tcpchat?style=flat&color=0080ff" alt="repo-top-language">
	<img src="https://img.shields.io/github/languages/count/FlewToL/tcpchat?style=flat&color=0080ff" alt="repo-language-count">
<p>
<p align="center">
		<em>Developed with the software and tools below.</em>
</p>
<p align="center">
	<img src="https://img.shields.io/badge/GNU%20Bash-4EAA25.svg?style=flat&logo=GNU-Bash&logoColor=white" alt="GNU%20Bash">
	<img src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?style=flat&logo=JavaScript&logoColor=black" alt="JavaScript">
	<img src="https://img.shields.io/badge/YAML-CB171E.svg?style=flat&logo=YAML&logoColor=white" alt="YAML">
	<img src="https://img.shields.io/badge/PowerShell-5391FE.svg?style=flat&logo=PowerShell&logoColor=white" alt="PowerShell">
	<img src="https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white" alt="Python">
	<img src="https://img.shields.io/badge/TypeScript-3178C6.svg?style=flat&logo=TypeScript&logoColor=white" alt="TypeScript">
	<img src="https://img.shields.io/badge/Docker-2496ED.svg?style=flat&logo=Docker&logoColor=white" alt="Docker">
	<img src="https://img.shields.io/badge/JSON-000000.svg?style=flat&logo=JSON&logoColor=white" alt="JSON">
</p>
<hr>

##  Оглавление

> - [ Overview](#-overview)
> - [ Features](#-features)
> - [ Repository Structure](#-repository-structure)
> - [ Modules](#-modules)
> - [ Getting Started](#-getting-started)
>   - [ Installation](#-installation)
>   - [ Running tcpchat](#-running-tcpchat)
>   - [ Tests](#-tests)
> - [ Project Roadmap](#-project-roadmap)
> - [ Contributing](#-contributing)
> - [ License](#-license)
> - [ Acknowledgments](#-acknowledgments)

---

##  Введение

Современный рынок разработки программного обеспечения требует от разработчиков не только глубоких знаний в своей области, но и способности ориентироваться в смежных технологических направлениях. Данная курсовая работа посвящена разработке TCP чат-сервера и клиента, а также веб-приложения для российского рынка на платформе AstraLinux. Актуальность данной темы обусловлена растущей потребностью в безопасных и надежных коммуникационных системах, особенно в условиях использования отечественных операционных систем.

Целью данной работы является разработка программного продукта, включающего TCP чат-сервер и клиент, а также веб-приложение, которое будет функционировать на AstraLinux. Для достижения поставленной цели необходимо решить следующие задачи:
1.	Провести анализ предметной области.
2.	Проанализировать аналоги разрабатываемого решения.
3.	Описать требования к разрабатываемому решению.
4.	Выбрать инструменты и/или средства для реализации проекта.
5.	Разработать проект решения.
6.	Разработать программный продукт.
7.	Составить отчет по работе.
8.	Представить отчет к защите и ответить на вопросы по проекту

Объектом данного исследования является процесс создания коммуникационной системы, включающей серверную и клиентскую части, а также веб-интерфейс для управления и мониторинга.

Предметом исследования в данной работе является разработка TCP чат-сервера и клиента, а также веб-приложения для российского рынка на платформе AstraLinux.

В качестве основных методов исследования применены анализ, синтез, сравнение и моделирование. Практическая реализация поставленной задачи соответствует основным подходам к разработке программного обеспечения.

Информационной базой исследования являются открытые источники, в том числе доступные в сети Интернет, а также материалы курса «Создание программного обеспечения», доступные через систему дистанционного обучения РТУ МИРЭА.

В данном отчете будет представлен процесс разработки программного продукта, в том числе теоретический обзор области и системы, технологическое проектирование и описание системы. а также непосредственно результаты разработки.


---

##  Структура

```sh
└── tcpchat/
    ├── CHANGELOG.md
    ├── Dockerfile
    ├── LICENSE
    ├── README.md
    ├── codeql-analytics.txt
    ├── commitlintrc.json
    ├── data
    │   └── README
    ├── deployment.yml
    ├── docker-compose.yml
    ├── docs
    │   ├── css
    │   │   └── index.css
    │   ├── index.html
    │   └── js
    │       └── index.js
    ├── docs-markdown
    │   ├── CODE_STYLING_GUIDES.md
    │   ├── dealings
    │   │   ├── README
    │   │   └── conventions
    │   │       ├── MANAGING.txt
    │   │       └── SEMVER.md
    │   └── github
    │       ├── COMMIT_CONVENTION.md
    │       └── ISSUES
    │           ├── ISSUE_POLICY.md
    │           └── ISSUE_TRIAGE.md
    ├── environment.ts
    ├── esbuild.config.mjs
    ├── gh.cli.sh
    ├── jsconfig.json
    ├── scripts
    │   ├── README
    │   ├── js
    │   │   ├── analytics-workflow.ts
    │   │   ├── check-patch-diff.ts
    │   │   ├── create-api-json.js
    │   │   ├── generate-version-json.js
    │   │   ├── gn-asar-hash.js
    │   │   ├── gn-asar.js
    │   │   ├── gn-check.js
    │   │   ├── labels-api.js
    │   │   └── labels-import.js
    │   ├── lint.js
    │   ├── patcher.js
    │   ├── python
    │   │   ├── clonesource.py
    │   │   ├── git-export-patches.py
    │   │   ├── git-import-patches.py
    │   │   ├── lib
    │   │   │   ├── git.py
    │   │   │   └── patches.py
    │   │   ├── pack.py
    │   │   ├── run-clang-format.py
    │   │   ├── run-clang-tidy.py
    │   │   └── run-gn-format.py
    │   ├── shell
    │   │   ├── publish-npm.ps1
    │   │   ├── publish-npm.sh
    │   │   ├── publish-nuget.ps1
    │   │   └── publish-nuget.sh
    │   └── spec-runner.js
    ├── source
    │   ├── config
    │   │   ├── __init__.py
    │   │   ├── __pycache__
    │   │   │   ├── __init__.cpython-312.pyc
    │   │   │   └── config_reader.cpython-312.pyc
    │   │   └── config_reader.py
    │   ├── main.py
    │   └── src
    │       ├── api
    │       │   ├── __init__.py
    │       │   ├── __pycache__
    │       │   │   ├── __init__.cpython-312.pyc
    │       │   │   └── server.cpython-312.pyc
    │       │   ├── auth
    │       │   │   ├── __init__.py
    │       │   │   ├── auth.py
    │       │   │   ├── manager.py
    │       │   │   └── schemas.py
    │       │   ├── endpoints
    │       │   │   ├── __init__.py
    │       │   │   ├── __pycache__
    │       │   │   ├── main.py
    │       │   │   ├── messages.py
    │       │   │   ├── register.py
    │       │   │   └── users.py
    │       │   ├── fau.py
    │       │   └── server.py
    │       ├── database
    │       │   ├── __init__.py
    │       │   ├── __pycache__
    │       │   │   ├── __init__.cpython-312.pyc
    │       │   │   ├── connection.cpython-312.pyc
    │       │   │   └── models.cpython-312.pyc
    │       │   ├── connection.py
    │       │   ├── models.py
    │       │   └── queries
    │       │       ├── __init__.py
    │       │       ├── messages.py
    │       │       └── users.py
    │       ├── frontend
    │       │   ├── App.css
    │       │   ├── App.js
    │       │   ├── App.test.js
    │       │   ├── Chat.css
    │       │   ├── Chat.js
    │       │   ├── Login.css
    │       │   ├── Login.js
    │       │   ├── Registration copy.js
    │       │   ├── Registration.css
    │       │   ├── Registration.js
    │       │   ├── index.css
    │       │   ├── index.js
    │       │   ├── reportWebVitals.js
    │       │   └── setupTests.js
    │       └── tcp
    │           ├── __init__.py
    │           ├── __pycache__
    │           │   ├── __init__.cpython-312.pyc
    │           │   └── server.cpython-312.pyc
    │           ├── client.py
    │           └── server.py
    ├── tsconfig.json
    ├── tsconfig.script.json
    ├── tsconfig.spec.json
    ├── tsconfig.tsbuildinfo
    └── typings
        └── environment.d.ts
```

---

##  Модули

<details closed><summary>.</summary>

| File                                                                                        | Summary                                          |
| ---                                                                                         | ---                                              |
| [jsconfig.json](https://github.com/FlewToL/tcpchat/blob/master/jsconfig.json)               | HTTP error 401 for prompt `jsconfig.json`        |
| [docker-compose.yml](https://github.com/FlewToL/tcpchat/blob/master/docker-compose.yml)     | HTTP error 401 for prompt `docker-compose.yml`   |
| [esbuild.config.mjs](https://github.com/FlewToL/tcpchat/blob/master/esbuild.config.mjs)     | HTTP error 401 for prompt `esbuild.config.mjs`   |
| [environment.ts](https://github.com/FlewToL/tcpchat/blob/master/environment.ts)             | HTTP error 401 for prompt `environment.ts`       |
| [gh.cli.sh](https://github.com/FlewToL/tcpchat/blob/master/gh.cli.sh)                       | HTTP error 401 for prompt `gh.cli.sh`            |
| [Dockerfile](https://github.com/FlewToL/tcpchat/blob/master/Dockerfile)                     | HTTP error 401 for prompt `Dockerfile`           |
| [tsconfig.tsbuildinfo](https://github.com/FlewToL/tcpchat/blob/master/tsconfig.tsbuildinfo) | HTTP error 401 for prompt `tsconfig.tsbuildinfo` |
| [tsconfig.json](https://github.com/FlewToL/tcpchat/blob/master/tsconfig.json)               | HTTP error 401 for prompt `tsconfig.json`        |
| [deployment.yml](https://github.com/FlewToL/tcpchat/blob/master/deployment.yml)             | HTTP error 401 for prompt `deployment.yml`       |
| [tsconfig.spec.json](https://github.com/FlewToL/tcpchat/blob/master/tsconfig.spec.json)     | HTTP error 401 for prompt `tsconfig.spec.json`   |
| [codeql-analytics.txt](https://github.com/FlewToL/tcpchat/blob/master/codeql-analytics.txt) | HTTP error 401 for prompt `codeql-analytics.txt` |
| [tsconfig.script.json](https://github.com/FlewToL/tcpchat/blob/master/tsconfig.script.json) | HTTP error 401 for prompt `tsconfig.script.json` |
| [commitlintrc.json](https://github.com/FlewToL/tcpchat/blob/master/commitlintrc.json)       | HTTP error 401 for prompt `commitlintrc.json`    |

</details>

<details closed><summary>typings</summary>

| File                                                                                        | Summary                                              |
| ---                                                                                         | ---                                                  |
| [environment.d.ts](https://github.com/FlewToL/tcpchat/blob/master/typings/environment.d.ts) | HTTP error 401 for prompt `typings/environment.d.ts` |

</details>

<details closed><summary>docs-markdown.dealings.conventions</summary>

| File                                                                                                           | Summary                                                                     |
| ---                                                                                                            | ---                                                                         |
| [MANAGING.txt](https://github.com/FlewToL/tcpchat/blob/master/docs-markdown/dealings/conventions/MANAGING.txt) | HTTP error 401 for prompt `docs-markdown/dealings/conventions/MANAGING.txt` |

</details>

<details closed><summary>scripts</summary>

| File                                                                                    | Summary                                            |
| ---                                                                                     | ---                                                |
| [spec-runner.js](https://github.com/FlewToL/tcpchat/blob/master/scripts/spec-runner.js) | HTTP error 401 for prompt `scripts/spec-runner.js` |
| [lint.js](https://github.com/FlewToL/tcpchat/blob/master/scripts/lint.js)               | HTTP error 401 for prompt `scripts/lint.js`        |
| [patcher.js](https://github.com/FlewToL/tcpchat/blob/master/scripts/patcher.js)         | HTTP error 401 for prompt `scripts/patcher.js`     |

</details>

<details closed><summary>scripts.shell</summary>

| File                                                                                                | Summary                                                     |
| ---                                                                                                 | ---                                                         |
| [publish-npm.sh](https://github.com/FlewToL/tcpchat/blob/master/scripts/shell/publish-npm.sh)       | HTTP error 401 for prompt `scripts/shell/publish-npm.sh`    |
| [publish-nuget.sh](https://github.com/FlewToL/tcpchat/blob/master/scripts/shell/publish-nuget.sh)   | HTTP error 401 for prompt `scripts/shell/publish-nuget.sh`  |
| [publish-nuget.ps1](https://github.com/FlewToL/tcpchat/blob/master/scripts/shell/publish-nuget.ps1) | HTTP error 401 for prompt `scripts/shell/publish-nuget.ps1` |
| [publish-npm.ps1](https://github.com/FlewToL/tcpchat/blob/master/scripts/shell/publish-npm.ps1)     | HTTP error 401 for prompt `scripts/shell/publish-npm.ps1`   |

</details>

<details closed><summary>scripts.python</summary>

| File                                                                                                         | Summary                                                          |
| ---                                                                                                          | ---                                                              |
| [run-gn-format.py](https://github.com/FlewToL/tcpchat/blob/master/scripts/python/run-gn-format.py)           | HTTP error 401 for prompt `scripts/python/run-gn-format.py`      |
| [run-clang-tidy.py](https://github.com/FlewToL/tcpchat/blob/master/scripts/python/run-clang-tidy.py)         | HTTP error 401 for prompt `scripts/python/run-clang-tidy.py`     |
| [git-import-patches.py](https://github.com/FlewToL/tcpchat/blob/master/scripts/python/git-import-patches.py) | HTTP error 401 for prompt `scripts/python/git-import-patches.py` |
| [pack.py](https://github.com/FlewToL/tcpchat/blob/master/scripts/python/pack.py)                             | HTTP error 401 for prompt `scripts/python/pack.py`               |
| [clonesource.py](https://github.com/FlewToL/tcpchat/blob/master/scripts/python/clonesource.py)               | HTTP error 401 for prompt `scripts/python/clonesource.py`        |
| [run-clang-format.py](https://github.com/FlewToL/tcpchat/blob/master/scripts/python/run-clang-format.py)     | HTTP error 401 for prompt `scripts/python/run-clang-format.py`   |
| [git-export-patches.py](https://github.com/FlewToL/tcpchat/blob/master/scripts/python/git-export-patches.py) | HTTP error 401 for prompt `scripts/python/git-export-patches.py` |

</details>

<details closed><summary>scripts.python.lib</summary>

| File                                                                                       | Summary                                                   |
| ---                                                                                        | ---                                                       |
| [git.py](https://github.com/FlewToL/tcpchat/blob/master/scripts/python/lib/git.py)         | HTTP error 401 for prompt `scripts/python/lib/git.py`     |
| [patches.py](https://github.com/FlewToL/tcpchat/blob/master/scripts/python/lib/patches.py) | HTTP error 401 for prompt `scripts/python/lib/patches.py` |

</details>

<details closed><summary>scripts.js</summary>

| File                                                                                                           | Summary                                                         |
| ---                                                                                                            | ---                                                             |
| [create-api-json.js](https://github.com/FlewToL/tcpchat/blob/master/scripts/js/create-api-json.js)             | HTTP error 401 for prompt `scripts/js/create-api-json.js`       |
| [gn-asar-hash.js](https://github.com/FlewToL/tcpchat/blob/master/scripts/js/gn-asar-hash.js)                   | HTTP error 401 for prompt `scripts/js/gn-asar-hash.js`          |
| [labels-import.js](https://github.com/FlewToL/tcpchat/blob/master/scripts/js/labels-import.js)                 | HTTP error 401 for prompt `scripts/js/labels-import.js`         |
| [labels-api.js](https://github.com/FlewToL/tcpchat/blob/master/scripts/js/labels-api.js)                       | HTTP error 401 for prompt `scripts/js/labels-api.js`            |
| [gn-asar.js](https://github.com/FlewToL/tcpchat/blob/master/scripts/js/gn-asar.js)                             | HTTP error 401 for prompt `scripts/js/gn-asar.js`               |
| [gn-check.js](https://github.com/FlewToL/tcpchat/blob/master/scripts/js/gn-check.js)                           | HTTP error 401 for prompt `scripts/js/gn-check.js`              |
| [generate-version-json.js](https://github.com/FlewToL/tcpchat/blob/master/scripts/js/generate-version-json.js) | HTTP error 401 for prompt `scripts/js/generate-version-json.js` |
| [check-patch-diff.ts](https://github.com/FlewToL/tcpchat/blob/master/scripts/js/check-patch-diff.ts)           | HTTP error 401 for prompt `scripts/js/check-patch-diff.ts`      |
| [analytics-workflow.ts](https://github.com/FlewToL/tcpchat/blob/master/scripts/js/analytics-workflow.ts)       | HTTP error 401 for prompt `scripts/js/analytics-workflow.ts`    |

</details>

<details closed><summary>source</summary>

| File                                                                     | Summary                                    |
| ---                                                                      | ---                                        |
| [main.py](https://github.com/FlewToL/tcpchat/blob/master/source/main.py) | HTTP error 401 for prompt `source/main.py` |

</details>

<details closed><summary>source.config</summary>

| File                                                                                              | Summary                                                    |
| ---                                                                                               | ---                                                        |
| [config_reader.py](https://github.com/FlewToL/tcpchat/blob/master/source/config/config_reader.py) | HTTP error 401 for prompt `source/config/config_reader.py` |

</details>

<details closed><summary>source.src.frontend</summary>

| File                                                                                                            | Summary                                                              |
| ---                                                                                                             | ---                                                                  |
| [reportWebVitals.js](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/reportWebVitals.js)     | HTTP error 401 for prompt `source/src/frontend/reportWebVitals.js`   |
| [App.test.js](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/App.test.js)                   | HTTP error 401 for prompt `source/src/frontend/App.test.js`          |
| [Registration copy.js](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/Registration copy.js) | HTTP error 401 for prompt `source/src/frontend/Registration copy.js` |
| [setupTests.js](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/setupTests.js)               | HTTP error 401 for prompt `source/src/frontend/setupTests.js`        |
| [Login.js](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/Login.js)                         | HTTP error 401 for prompt `source/src/frontend/Login.js`             |
| [Chat.js](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/Chat.js)                           | HTTP error 401 for prompt `source/src/frontend/Chat.js`              |
| [App.js](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/App.js)                             | HTTP error 401 for prompt `source/src/frontend/App.js`               |
| [Login.css](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/Login.css)                       | HTTP error 401 for prompt `source/src/frontend/Login.css`            |
| [App.css](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/App.css)                           | HTTP error 401 for prompt `source/src/frontend/App.css`              |
| [index.js](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/index.js)                         | HTTP error 401 for prompt `source/src/frontend/index.js`             |
| [Registration.js](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/Registration.js)           | HTTP error 401 for prompt `source/src/frontend/Registration.js`      |
| [Registration.css](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/Registration.css)         | HTTP error 401 for prompt `source/src/frontend/Registration.css`     |
| [index.css](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/index.css)                       | HTTP error 401 for prompt `source/src/frontend/index.css`            |
| [Chat.css](https://github.com/FlewToL/tcpchat/blob/master/source/src/frontend/Chat.css)                         | HTTP error 401 for prompt `source/src/frontend/Chat.css`             |

</details>

<details closed><summary>source.src.database</summary>

| File                                                                                              | Summary                                                       |
| ---                                                                                               | ---                                                           |
| [connection.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/database/connection.py) | HTTP error 401 for prompt `source/src/database/connection.py` |
| [models.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/database/models.py)         | HTTP error 401 for prompt `source/src/database/models.py`     |

</details>

<details closed><summary>source.src.database.queries</summary>

| File                                                                                                  | Summary                                                             |
| ---                                                                                                   | ---                                                                 |
| [messages.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/database/queries/messages.py) | HTTP error 401 for prompt `source/src/database/queries/messages.py` |
| [users.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/database/queries/users.py)       | HTTP error 401 for prompt `source/src/database/queries/users.py`    |

</details>

<details closed><summary>source.src.api</summary>

| File                                                                                 | Summary                                              |
| ---                                                                                  | ---                                                  |
| [fau.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/api/fau.py)       | HTTP error 401 for prompt `source/src/api/fau.py`    |
| [server.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/api/server.py) | HTTP error 401 for prompt `source/src/api/server.py` |

</details>

<details closed><summary>source.src.api.endpoints</summary>

| File                                                                                               | Summary                                                          |
| ---                                                                                                | ---                                                              |
| [main.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/api/endpoints/main.py)         | HTTP error 401 for prompt `source/src/api/endpoints/main.py`     |
| [messages.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/api/endpoints/messages.py) | HTTP error 401 for prompt `source/src/api/endpoints/messages.py` |
| [users.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/api/endpoints/users.py)       | HTTP error 401 for prompt `source/src/api/endpoints/users.py`    |
| [register.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/api/endpoints/register.py) | HTTP error 401 for prompt `source/src/api/endpoints/register.py` |

</details>

<details closed><summary>source.src.api.auth</summary>

| File                                                                                        | Summary                                                    |
| ---                                                                                         | ---                                                        |
| [manager.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/api/auth/manager.py) | HTTP error 401 for prompt `source/src/api/auth/manager.py` |
| [schemas.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/api/auth/schemas.py) | HTTP error 401 for prompt `source/src/api/auth/schemas.py` |
| [auth.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/api/auth/auth.py)       | HTTP error 401 for prompt `source/src/api/auth/auth.py`    |

</details>

<details closed><summary>source.src.tcp</summary>

| File                                                                                 | Summary                                              |
| ---                                                                                  | ---                                                  |
| [client.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/tcp/client.py) | HTTP error 401 for prompt `source/src/tcp/client.py` |
| [server.py](https://github.com/FlewToL/tcpchat/blob/master/source/src/tcp/server.py) | HTTP error 401 for prompt `source/src/tcp/server.py` |

</details>

---

##  Начало работы

***Requirements***

Ensure you have the following dependencies installed on your system:

* **Python**: `version x.y.z`

###  Установка

1. Clone the tcpchat repository:

```sh
git clone https://github.com/FlewToL/tcpchat
```

2. Change to the project directory:

```sh
cd tcpchat
```

3. Install the dependencies:

```sh
pip install -r requirements.txt
```

###  Запуск приложения

Use the following command to run tcpchat:

```sh
python main.py
```

###  Tests

To execute tests, run:

```sh
pytest
```

---

##  Project Roadmap

- [X] `► INSERT-TASK-1`
- [ ] `► INSERT-TASK-2`
- [ ] `► ...`

---

##  Сотрудничество

Contributions are welcome! Here are several ways you can contribute:

- **[Submit Pull Requests](https://github.com/FlewToL/tcpchat/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.
- **[Join the Discussions](https://github.com/FlewToL/tcpchat/discussions)**: Share your insights, provide feedback, or ask questions.
- **[Report Issues](https://github.com/FlewToL/tcpchat/issues)**: Submit bugs found or log feature requests for Tcpchat.

<details closed>
    <summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project repository to your GitHub account.
2. **Clone Locally**: Clone the forked repository to your local machine using a Git client.
   ```sh
   git clone https://github.com/FlewToL/tcpchat
   ```
3. **Create a New Branch**: Always work on a new branch, giving it a descriptive name.
   ```sh
   git checkout -b new-feature-x
   ```
4. **Make Your Changes**: Develop and test your changes locally.
5. **Commit Your Changes**: Commit with a clear message describing your updates.
   ```sh
   git commit -m 'Implemented new feature x.'
   ```
6. **Push to GitHub**: Push the changes to your forked repository.
   ```sh
   git push origin new-feature-x
   ```
7. **Submit a Pull Request**: Create a PR against the original project repository. Clearly describe the changes and their motivations.

Once your PR is reviewed and approved, it will be merged into the main branch.

</details>

---

##  Лицензия

This project is protected under the [SELECT-A-LICENSE](https://choosealicense.com/licenses) License. For more details, refer to the [LICENSE](https://choosealicense.com/licenses/) file.

---
