# RIAP Super Repo

## 中文說明

這個倉庫是 RIAP 的總入口。它主要用來整理文件、PBI、後端與前端兩個獨立子專案的連結。

如果你不熟悉 `git`、`npm` 或 VS Code，可以把這份 README 當成「照著做就能跑 prototype」的說明。目標只有一個：把前端 prototype 跑起來，然後直接在瀏覽器使用。

## 你要先安裝什麼

在 Windows 上，先安裝這些工具。建議都裝在系統預設位置，`winget` 會幫你完成大部分設定：

- `Git`：用來把專案從遠端複製到你的電腦。
- `Node.js`：用來執行前端 prototype 的開發伺服器。
- `npm`：通常會跟著 `Node.js` 一起安裝，不用另外找。
- `Java 17` 與 `Maven`：只有在你要跑 `backend/` 時才需要；單純看 prototype 可以先不用裝。

如果你想用命令列安裝，Windows 可以直接在 PowerShell 執行：

```powershell
winget install --id Git.Git -e --source winget
winget install --id OpenJS.NodeJS.LTS -e --source winget
```

如果之後要跑後端，再補裝：

```powershell
winget install --id Microsoft.OpenJDK.17 -e --source winget
winget install --id Apache.Maven -e --source winget
```

## 你要把專案放在哪裡

你可以把專案放在自己電腦上的任何資料夾。以下範例使用：`D:\CodingWorkspace\SE`

## 先把專案複製到電腦

先打開 PowerShell，切到你要放專案的位置，然後 clone：

```powershell
Set-Location "D:\CodingWorkspace\ISLab\Master02\SWE"
git clone --recurse-submodules https://github.com/VerechoTJI/rental-information-aggregation-platform.git
```

如果你已經先 clone 了，但 submodule 沒有抓下來，再補這兩行：

```powershell
Set-Location "D:\CodingWorkspace\ISLab\Master02\SWE\rental-information-aggregation-platform"
git submodule sync --recursive
git submodule update --init --recursive
```

## 跑前端 prototype

前端 prototype 在 `frontend/prototype/`。你要在這個資料夾裡安裝前端套件，然後啟動開發伺服器：

```powershell
Set-Location "D:\CodingWorkspace\ISLab\Master02\SWE\rental-information-aggregation-platform\frontend\prototype"
npm install
npm run dev
```

終端機會顯示一個本機網址，通常是 `http://localhost:5173/`。把那個網址貼到瀏覽器，就可以直接使用 prototype。

如果你只是想先試 prototype，不需要先跑 `backend/`。只有在你要開發 Java 後端時，才需要另外進 `backend/` 執行 `mvn test` 或 `mvn package`。

This repository is the top-level workspace for RIAP and manages separate backend and frontend repositories alongside shared documentation.

## Layout

- `backend/`: standalone backend repository with the Java service.
- `frontend/`: standalone frontend repository for the UI.
- `docs/`: source-of-truth requirements and documentation.
- `pbi/`: per-feature PBIs and backlog tracking.

## Quick setup (clone + submodules)

Clone and fetch submodules in one step:

```powershell
git clone --recurse-submodules https://github.com/VerechoTJI/rental-information-aggregation-platform.git
```

If you already cloned without submodules, run:

```powershell
git submodule sync --recursive
git submodule update --init --recursive
```

## Prerequisites

- Java 17 (JDK) installed and `java`/`javac` available on PATH.
- Apache Maven 3.8+ (`mvn` on PATH) to build the backend.
- (Frontend) Node.js and a package manager (npm or pnpm) when frontend code is added.

On Windows you can install with winget (example):

```powershell
winget install --id=Microsoft.OpenJDK.17 -e --source winget
winget install --id=Apache.Maven -e --source winget
```

## Backend build (quick)

From the repository root you can run:

```powershell
mvn -f backend test
# or to build the artifact
mvn -f backend package
```

If `mvn` is not available you'll see an error like "mvn: The term 'mvn' is not recognized" — install Maven and ensure it's on your PATH.

## Frontend

The `frontend/` submodule is currently a placeholder. When frontend sources are added the typical workflow will be:

```powershell
# from repo root
cd frontend
# install deps (example)
npm install
# start dev server
npm run dev
# build for production
npm run build
```

## Workflow

- Keep backend and frontend work in their own repositories.
- Use the root repo to coordinate shared docs, PBIs, and cross-repo planning.

## Conventions

Branch naming

- main: protected release branch.
- feature/<ticket-id>-short-desc: new features.
- fix/<ticket-id>-short-desc: bug fixes.
- hotfix/<short-desc>: urgent fixes to `main`.

Commit messages (Conventional Commits)

- Use Conventional Commits for all commits. Examples:
  - feat: add new search endpoint
  - fix: correct null pointer in listing parser
  - docs: update API section in README
  - chore: bump maven plugin versions

Submodules

- Clone with `--recurse-submodules` or run `git submodule update --init --recursive` after clone.
- Do not attempt to commit changes inside a submodule from the super-repo — cd into the submodule, commit there, then update the super-repo's recorded submodule commit and commit that change in the super-repo.

Pull requests

- Open PRs from feature branches into `main` and require at least one reviewer.
- Include a short description and reference the ticket id (if any).

Formatting and linters

- Follow project-specific linters where configured. For Java use a standard formatter (Google Java Style or similar).
