<div align="center">

  # skills-pack
  *Uma coleção de skills prontas para Claude Code, Kiro Code, VSCode,* **Qualquer lugar que aceite skills**

  [![Licença](https://img.shields.io/badge/licença-MIT-blue?style=flat-square)](LICENSE)
  [![Skills](https://img.shields.io/badge/skills-23-green?style=flat-square)](#skills)

  [Skills](#skills) • [Como usar](#como-usar) • [Contribuindo](#contribuindo)

</div>

---

Coleção de skills prontas para uso no [Claude Code](https://claude.ai/code) e no [Kiro](https://kiro.dev). Cada skill é uma pasta com um `SKILL.md` que instrui a IA a executar tarefas específicas de forma consistente e previsível.

## Como usar

### Kiro

Copie as pastas das skills que quiser para `.kiro/skills/` no seu projeto:

```
.kiro/
└── skills/
    ├── caveman/
    ├── code-review/
    └── ...
```

### Claude Code

Copie as pastas para o diretório de skills do Claude Code:

```bash
cp -r skills-pack/caveman ~/.claude/skills/
```

> [!TIP]
> Você não precisa instalar todas — copie só as que fazem sentido pro seu fluxo de trabalho.

## Skills

### Modo caveman
Conjunto de skills para comunicação ultra-comprimida, economizando tokens sem perder precisão técnica.

| Skill | O que faz |
|---|---|
| `caveman` | Ativa modo de resposta telegráfico — corta filler, mantém substância. Economiza ~65% de tokens no output |
| `cavecrew` | Delega tarefas a subagentes comprimidos (investigador, builder, reviewer) para sessões longas |
| `caveman-commit` | Gera mensagens de commit no padrão Conventional Commits de forma enxuta |
| `caveman-compress` | Reescreve arquivos de memória (`CLAUDE.md`, etc.) em caveman para economizar tokens de input |
| `caveman-help` | Referência rápida de todos os modos e comandos caveman |
| `caveman-review` | Code review compacto e acionável: localização, problema, correção — uma linha por achado |

### Engenharia
Skills para o ciclo completo de desenvolvimento de software.

| Skill | O que faz |
|---|---|
| `code-review` | Review de PR em dois eixos paralelos: padrões do repo + fidelidade à spec |
| `codebase-design` | Design de arquitetura antes de codar, com ADRs e decisões documentadas |
| `diagnosing-bugs` | Loop de diagnóstico estruturado para bugs difíceis e regressões de performance |
| `grill-with-docs` | Interroga documentação para extrair respostas precisas sem achismos |
| `implement` | Implementa uma feature seguindo uma spec definida, sem improvisar |
| `improve-codebase-architecture` | Analisa o codebase e sugere melhorias de arquitetura com relatório HTML |
| `prototype` | Cria protótipos throwaway para validar lógica ou explorar UI antes de codar de verdade |
| `research` | Pesquisa técnica estruturada antes de tomar decisões de implementação |
| `to-spec` | Transforma uma ideia vaga em spec técnica formal |
| `wayfinder` | Navega um codebase desconhecido e monta um mapa mental do projeto |

### Produtividade
Skills para pensar melhor e trabalhar com mais clareza.

| Skill | O que faz |
|---|---|
| `grill-me` | Faz perguntas difíceis sobre sua própria ideia para revelar pontos cegos |
| `grilling` | Versão mais elaborada do `grill-me`, com profundidade maior |
| `handoff` | Documenta o estado atual da sessão para passar a outra sessão ou agente |

### Outras
| Skill | O que faz |
|---|---|
| `create-readme` | Gera READMEs completos e bem estruturados para projetos |
| `interview-me` | Extrai o que você realmente quer antes de qualquer plano, spec ou código |
| `output-skill` | Proíbe a IA de truncar output — sem `// ...`, sem esqueletos, sem "quer que eu continue?" |
| `taste-skill` | Skill de frontend anti-slop para landing pages, portfólios e redesigns |

## Contribuindo

Sinta-se à vontade para modificar e melhorar! Crie um fork e publique as suas mudanças.
