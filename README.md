# Império Lords - Backend, Bot & Plataforma de Atendimento

## 1. Objetivo e Finalidade
Servidor backend robusto com integração a WhatsApp (Baileys), autenticação de operadores e gestão de filas de atendimento.

## 2. Tecnologias Utilizadas
- Node.js, TypeScript, Docker, Bun, QR Code, REST API

## 3. Arquitetura e Estrutura de Diretórios
Monorepo estruturado na pasta `packages/`, orquestrado via TypeScript e Bun. Suporte a execução em container Docker para alta disponibilidade do bot de atendimento.

## 4. Principais Arquivos e Responsabilidades
- `packages/`: Módulos de mensageria, API REST e conectores de banco.
- `processData.json`: Configurações de fluxos de processamento.
- `scripts/`: Scripts operacionais de deploy e inicialização.
- `start.md`: Documentação passo a passo para execução do bot.

## 5. Funcionalidades Identificadas
- Geração de QR Code no terminal para pareamento com WhatsApp
- Atendimento automatizado e encaminhamento para atendentes humanos
- Arquitetura preparada para mensageria assíncrona

## 6. Como Compilar ou Executar
```bash
bun install
bun run dev
# Execução via Docker: docker build -t imperio-lords . && docker run imperio-lords
```

## 7. Estado Atual do Projeto
**Completo**

## 8. Pendências e Limitações Identificadas
Persistência do histórico de conversas em banco de dados relacional.
