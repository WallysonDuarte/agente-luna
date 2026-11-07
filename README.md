<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=f39c12&height=220&section=header&text=LUNA&fontColor=ffffff&fontSize=72&fontAlignY=38&desc=Marketing%20Digital&descSize=22&descAlignY=60" width="100%" />

<img src="./assets/portrait.png" width="200" alt="Luna" />

# 🌙 Luna · Marketing Digital

**Constroi aquisicao mensuravel: canal, oferta, rastreamento e campanha — com numero antes e depois, nao impressao.**

![Skills](https://img.shields.io/badge/skills-5-f39c12?style=for-the-badge)
![CLIs](https://img.shields.io/badge/CLIs-8-2980b9?style=for-the-badge)
![Idioma](https://img.shields.io/badge/pt--BR-nativo-1abc9c?style=for-the-badge)

</div>

---

## Por que usar este agente

- **Oferta conferida no produto.** Antes de escrever "gratuito", le o que o sistema realmente cobra — evita a promessa que o suporte paga depois.
- **Rastreamento desde o primeiro clique.** Parametro de origem, evento de conversao e funil montados antes do trafego.
- **Indicador com valor antes.** Toda campanha tem base de comparacao, nao apenas resultado.
- **Separa organico de pago.** Leitura honesta do que trouxe resultado.
- **Regra comercial registrada.** A oferta correta fica anotada junto a campanha, para a proxima peca nao reintroduzir o erro.

---

## Skills

| Skill | Titulo | O que resolve |
|---|---|---|
| [`estrategia-de-aquisicao`](skills/estrategia-de-aquisicao/SKILL.md) | Estrategia de aquisicao | Escolher canais por estagio e custo, definir oferta e montar o funil de entrada com indicadores por etapa. |
| [`campanhas-pagas`](skills/campanhas-pagas/SKILL.md) | Campanhas pagas | Estruturar campanhas em busca, display e redes sociais com segmentacao, palavras negativas, teste de criativo e controle de custo. |
| [`analytics-e-rastreamento`](skills/analytics-e-rastreamento/SKILL.md) | Analytics e rastreamento | Instrumentar eventos, parametros de origem e funis para atribuir resultado com honestidade. |
| [`email-marketing`](skills/email-marketing/SKILL.md) | E-mail marketing | Construir sequencias, garantir entregabilidade e medir com honestidade o canal de maior retorno. |
| [`calendario-e-social`](skills/calendario-e-social/SKILL.md) | Calendario editorial e redes sociais | Planejar e executar presencia por plataforma com cadencia sustentavel e adaptacao de formato. |

Cada skill e um arquivo markdown autocontido (`skills/<slug>/SKILL.md`): pode ser instalada
isolada, sem o resto do repositorio.

---

## Instalacao rapida

```bash
git clone https://github.com/WallysonDuarte/agente-luna.git
cd agente-luna

# Claude Code — skills nativas
cp -r skills/* ~/.claude/skills/

# Qualquer outra CLI — arquivo unico de instrucao
cat AGENT.md skills/*/SKILL.md > AGENTS.md
```

| CLI | Instalacao (Windows / PowerShell) | Onde colocar as skills | Rodar |
|---|---|---|---|
| **Claude Code** | `irm https://claude.ai/install.ps1 \| iex` | `~/.claude/skills/` | `claude -p "<pedido>"` |
| **Codex** | `irm https://chatgpt.com/codex/install.ps1 \| iex` | `AGENTS.md na raiz do projeto` | `codex exec --skip-git-repo-check "<pedido>"` |
| **Grok** | `irm https://x.ai/cli/install.ps1 \| iex` | `passado no prompt` | `grok -p "<pedido>"` |
| **Antigravity** | `irm https://antigravity.google/cli/install.ps1 \| iex` | `passado no prompt` | `agy -p "<pedido>"` |
| **Hermes** | `iex (irm https://hermes-agent.nousresearch.com/install.ps1)` | `passado no prompt` | `hermes` |
| **OpenClaw** | `& ([scriptblock]::Create((iwr -useb https://openclaw.ai/install.ps1))) -NoOnboard` | `~/.openclaw/skills/` | `openclaw agent --local -m "<pedido>"` |
| **OpenCode** | `irm https://opencode.ai/install \| iex` | `AGENTS.md na raiz do projeto` | `opencode` |
| **Kimi Code** | `irm https://code.kimi.com/kimi-code/install.ps1 \| iex` | `passado no prompt` | `kimi -p "<pedido>"` |

Passo a passo por CLI, incluindo macOS/Linux: **[install/README.md](install/README.md)**

---

## Estrutura

```
agente-luna/
├── AGENT.md                 definicao canonica do agente
├── .agent/agent.json        metadados legiveis por maquina
├── skills/
│   ├── estrategia-de-aquisicao/SKILL.md
│   ├── campanhas-pagas/SKILL.md
│   ├── analytics-e-rastreamento/SKILL.md
│   ├── email-marketing/SKILL.md
│   └── calendario-e-social/SKILL.md
├── install/README.md        instalacao nas 8 CLIs
└── assets/portrait.png
```

---

## Ecossistema

Este agente faz parte de um time de 9 agentes especializados:

[![Master](https://img.shields.io/badge/Master-00ff41?style=flat-square)](https://github.com/WallysonDuarte/agente-master) [![Nova](https://img.shields.io/badge/Nova-9b59b6?style=flat-square)](https://github.com/WallysonDuarte/agente-nova) [![Atlas](https://img.shields.io/badge/Atlas-1abc9c?style=flat-square)](https://github.com/WallysonDuarte/agente-atlas) [![Pixel](https://img.shields.io/badge/Pixel-e91e63?style=flat-square)](https://github.com/WallysonDuarte/agente-pixel) [![Forge](https://img.shields.io/badge/Forge-e67e22?style=flat-square)](https://github.com/WallysonDuarte/agente-forge) [![Cipher](https://img.shields.io/badge/Cipher-c0392b?style=flat-square)](https://github.com/WallysonDuarte/agente-cipher) [![Luna](https://img.shields.io/badge/Luna-f39c12?style=flat-square)](https://github.com/WallysonDuarte/agente-luna) [![Lira](https://img.shields.io/badge/Lira-f0932b?style=flat-square)](https://github.com/WallysonDuarte/agente-lira) [![Rank](https://img.shields.io/badge/Rank-2980b9?style=flat-square)](https://github.com/WallysonDuarte/agente-rank)

[![Hub](https://img.shields.io/badge/ver%20o%20time%20completo-f39c12?style=for-the-badge)](https://github.com/WallysonDuarte/softwarehub-agentes)

---

<div align="center">

## Apoie este trabalho

Os 9 agentes sao mantidos de forma independente e publicados abertamente.
Se este material te poupou tempo, voce pode retribuir com um cafe:

<a href="https://buy.stripe.com/bJefZi3wJ4JH18WeuEgA800">
<img src="https://img.shields.io/badge/Apoie--me-R$%2010-f39c12?style=for-the-badge&logo=stripe&logoColor=white" alt="Apoie-me com R$ 10" />
</a>

## Links

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dududev/)
[![Do Zero ao Junior](https://img.shields.io/badge/Do%20Zero%20ao%20Junior-1abc9c?style=for-the-badge)](https://dozeroaojunior.com.br/)
[![Curitiba Software](https://img.shields.io/badge/Curitiba%20Software-2980b9?style=for-the-badge)](https://curitibasoftware.com.br/)
[![SoftwareHub](https://img.shields.io/badge/SoftwareHub-00ff41?style=for-the-badge)](https://softwarehub.com.br/)


</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=f39c12&height=100&section=footer" width="100%" />
