# [compsci-tips](https://suasuasuasuasua.github.io/compsci-tips/)

<p align="center">
  <img src="https://i.kym-cdn.com/photos/images/newsfeed/001/562/650/cd0.jpg" />
</p>

---

<!-- Allow people to click the link to go back to the repo from the GitHub Pages -->
## [Flowchart](https://github.com/suasuasuasuasua/compsci-tips#flowchart)

The nodes in the flowchart can be clicked on. Try it!

(_for Pages users, click on the title to view the flowchart_)

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

  subgraph BasicsGraphs[Basics]
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

  click start "https://github.com/suasuasuasuasua/compsci-tips/tree/main/setup/basics"
  click wsl "https://github.com/suasuasuasuasua/compsci-tips/tree/main/setup/wsl"
  click editors "https://github.com/suasuasuasuasua/compsci-tips/tree/main/editors"
  click bash "https://github.com/suasuasuasuasua/compsci-tips/tree/main/programming-languages/bash"
  click git "https://github.com/suasuasuasuasua/compsci-tips/tree/main/git(hub)/git"
  click github "https://github.com/suasuasuasuasua/compsci-tips/tree/main/git(hub)/github"
```

## Tree View

### Basics

- [Setup](./setup/basics/)
  - For Windows Users: [WSL](./setup/wsl/)
- [Code Editors](./editors/)
- [bash](./programming-languages/bash/)
- [git](./git(hub)/git/)
- [GitHub](./git(hub)/github/)
