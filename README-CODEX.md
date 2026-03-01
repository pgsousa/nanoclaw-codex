# NanoClaw Codex

Fork do [NanoClaw](https://github.com/qwibitai/nanoclaw) adaptado para usar o **OpenAI Codex** em vez do Anthropic Claude.

## Diferenças do Original

- Usa `@openai/codex-sdk` em vez de `@anthropic-ai/claude-agent-sdk`
- Requer `OPENAI_API_KEY` em vez de `ANTHROPIC_API_KEY`
- API baseada em threads (Codex) em vez de sessions (Claude)

## Quick Start

```bash
git clone https://github.com/pgsousa/nanoclaw-codex.git
cd nanoclaw-codex
```

Copia o ficheiro de exemplo e adiciona a tua API key:

```bash
cp .env.example .env
# Edita .env e adiciona a tua OPENAI_API_KEY
```

 depois segue as instruções do NanoClaw original para configuração.

## Requisitos

- Node.js 20+
- Docker (Linux) ou Apple Container (macOS)
- OpenAI API key com acesso ao Codex

## Licença

MIT
