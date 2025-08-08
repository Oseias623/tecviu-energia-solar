# 🌞 Tecviu - Energia Solar

## Projeto de Sistemas de IA para Vendas de Energia Solar

### 📋 Sobre o Projeto

Repositório dedicado aos sistemas de inteligência artificial da **Tecviu**, focados em automação de vendas, atendimento ao cliente e conversão de leads para energia solar.

### 🤖 Agentes Disponíveis

#### 🔍 SDR Qualificador
- **Localização:** `agentes/sdr-qualificador.json`
- **Função:** Agente especialista em qualificação de leads
- **Objetivo:** Coletar informações estratégicas e classificar potencial de conversão
- **Características:** Investigativo, humanizado, focado em coleta de dados e scoring interno

#### 🎯 Higor - Agente Closer
- **Localização:** `agentes/closer-higor.json`
- **Função:** Closer consultivo especializado em energia solar
- **Objetivo:** Qualificar leads e converter para agendamentos de visita técnica
- **Características:** Humanizado, empático, persuasivo e focado em resultados

### 🔄 Fluxo de Vendas Integrado

```
Lead Inicial → SDR Qualificador → Scoring/Classificação → Higor Closer → Agendamento
```

1. **SDR Qualificador** faz a triagem e coleta dados estratégicos
2. **Sistema de Scoring** classifica leads (Frio/Morno/Quente)
3. **Higor Closer** recebe leads qualificados para conversão
4. **Agendamento** de visita técnica para fechamento

### 🛠️ Ferramentas Integradas

- **enviaPontuacao:** Tool do SDR para classificar leads
- **MCP Agendamento:** Sistema de agendamento de visitas técnicas
- **Supabase Base de Dados:** Consulta de informações e cases de sucesso
- **Embeddings OpenAI:** Busca inteligente de informações
- **Postgres Tecviu:** Base de dados principal

### 📊 Estrutura do Projeto

```
tecviu-energia-solar/
├── agentes/
│   ├── sdr-qualificador.json      # Agente SDR de qualificação
│   ├── closer-higor.json          # Agente closer principal
│   └── [futuros agentes]
├── documentacao/
│   ├── implementacao.md           # Guia de implementação
│   ├── fluxos-vendas.md
│   └── guidelines.md
├── integracao/
│   ├── mcp-config.json
│   └── supabase-setup.md
└── README.md
```

### 🚀 Como Usar

#### Para o SDR Qualificador:
1. Configure o agente com `agentes/sdr-qualificador.json`
2. Implemente a tool `enviaPontuacao` no seu sistema
3. Configure scoring automático (0-100 pontos)
4. Monitore taxa de qualificação

#### Para o Closer Higor:
1. Configure o agente com `agentes/closer-higor.json`
2. Receba leads pré-qualificados do SDR
3. Foque na conversão para agendamento
4. Monitore taxa de fechamento

### 📈 Métricas de Sucesso

#### SDR Qualificador:
- **Taxa de completação** das 6 perguntas
- **Qualidade do scoring** (precisão da classificação)
- **Taxa de coleta de e-mail**
- **Distribuição de leads** por temperatura

#### Closer Higor:
- **Taxa de conversão** para agendamento
- **Qualidade dos leads** recebidos
- **Show-up rate** das visitas
- **Satisfação do cliente**

### 🎯 Sistema de Scoring

**Critérios de Qualificação (SDR):**
- 🏦 **Orçamento** (0-25 pts): Capacidade financeira
- ⏰ **Urgência** (0-20 pts): Prazo para decisão  
- 🎯 **Motivação** (0-20 pts): Dor específica identificada
- 👑 **Autoridade** (0-20 pts): Poder de decisão
- 🏆 **Qualidade** (0-15 pts): Preocupação com qualidade vs preço

**Classificação Final:**
- 🔥 **Quente** (71-100 pts): Direto para Closer
- 🌡️ **Morno** (41-70 pts): Nurturing + Closer
- ❄️ **Frio** (0-40 pts): Nurturing educativo

### 🔄 Atualizações

- **v1.1** - Agente SDR Qualificador adicionado
- **v1.0** - Agente Closer Higor implementado
- **Próximas versões:** Agentes de follow-up, atendimento pós-venda

### 📞 Contato

Para dúvidas sobre implementação ou customizações:
- Repositório: [tecviu-energia-solar](https://github.com/Oseias623/tecviu-energia-solar)
- Issues: Para reportar bugs ou solicitar features

---

**Tecviu** - Energia Solar Inteligente 🌞