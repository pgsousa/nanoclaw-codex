# NanoClaw Codex

Fork do [NanoClaw](https://github.com/qwibitai/nanoclaw) adaptado para usar o **OpenAI Codex** em vez do Anthropic Claude.

## Diferenças do Original

- Usa `@openai/codex-sdk` em vez de `@anthropic-ai/claude-agent-sdk`
- API baseada em threads (Codex) em vez de sessions (Claude)
- Runner de container ajustado para OpenAI Codex

## Autenticação (Codex)

### Estado atual deste fork
Este fork está configurado para **OpenAI API Key** (`OPENAI_API_KEY`) no ambiente.

### OAuth do Codex em vez de API Key?
Em teoria, o ecossistema Codex suporta login OAuth no CLI/IDE, mas **nesta implementação (SDK server-side dentro de container)** estamos a usar API key para garantir execução não-interativa e estável.

Se quiseres, no próximo passo eu faço um branch para experimentar autenticação OAuth persistida no container (com volume de credenciais), mas é uma integração separada.

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
