# [compsci-tips](https://suasuasuasuasua.github.io/compsci-tips/)

<p align="center">
  <img src="https://i.kym-cdn.com/photos/images/newsfeed/001/562/650/cd0.jpg" />
</p>

---

```mermaid
flowchart TB
  %% Definitions
  start[Start Here]
  wsl[WSL]
  bash[bash]
  git[git]
  github[GitHub]
  editors[Code Editors]

  %% Begin
  start --> editors
  start-->|Windows Users| wsl

  subgraph BasicsGraphs[" "]
    direction TB

    subgraph SetupGraph[" "]
      direction LR
      git --> github
    end %% SetupGraph

    wsl --> editors
    editors --> bash
    bash --> SetupGraph
  end %% Basics

  %% subgraph LanguagesGraphs[" "]
    %% direction TB
    
  %% end %% Languages

  click start "https://github.com/suasuasuasuasua/compsci-tips/tree/main/setup"
  click bash "https://github.com/suasuasuasuasua/compsci-tips/tree/main/programming-languages/bash"
  click git "https://github.com/suasuasuasuasua/compsci-tips/tree/main/general/git"
  click github "https://github.com/suasuasuasuasua/compsci-tips/tree/main/general/github"
```

---
