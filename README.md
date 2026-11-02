# 📋 SGAP — Sistema de Gestão de Atividade e Produtividade
### v2.0 · Everest Consultoria em Gestão Empresarial

Sistema web completo para gestão de atividades, produtividade e relatórios de equipe.  
Funciona 100% no navegador — sem servidor, sem instalação.

---

## 🚀 Como usar

### Opção 1 — GitHub Pages (recomendado)
1. Faça fork deste repositório
2. Vá em **Settings → Pages → Branch: main → Save**
3. Acesse: `https://seuusuario.github.io/sgap`

### Opção 2 — Local
1. Baixe o `index.html`
2. Abra no Chrome ou Edge
3. Pronto!

---

## 👤 Usuários Padrão

| Login | Senha | Perfil |
|-------|-------|--------|
| `admin` | `sgap2026` | Administrador (acesso total) |
| `diretor` | `diretor2026` | Diretor (vê toda a equipe) |
| `colaborador` | `colab2026` | Colaborador (vê apenas o próprio) |

> ⚠️ Altere as senhas em **Configurações → Usuários** após o primeiro acesso.

---

## 📋 Módulos

| Módulo | Descrição | Acesso |
|--------|-----------|--------|
| 📅 **Agenda** | Hoje / Atrasadas / Próximos 7 dias | Todos (filtrado por usuário) |
| 📊 **Dashboard** | KPIs, gráficos, produtividade | Todos |
| 📋 **Plano de Ação** | Ações com histórico de edições | Todos (filtrado) |
| ✅ **Atividades** | Atividades com pendências e histórico | Todos (filtrado) |
| 👥 **Equipe** | Ranking 🏆 pódio de produtividade | Diretor/Admin |
| 📄 **Rel. Mensal** | Relatório de feedback com PDF | Todos |
| ⚙️ **Cadastros** | Funcionários, Setores, Funções | Admin |
| 📍 **Localizações** | Lojas, filiais, locais | Admin |
| 👤 **Usuários** | Permissões por módulo | Admin |
| 🔗 **Google Sheets** | Sincronização de dados | Admin |

---

## 🔐 Controle de Acesso

- **Diretor/Admin**: Vê todos os dados, pode filtrar por colaborador
- **Colaborador**: Vê **apenas suas próprias** atividades e ações
- Permissões configuráveis por módulo em **Configurações → Usuários**

---

## 📝 Histórico de Edições

Toda edição em Atividades e Plano de Ação registra automaticamente:
- Data e hora da edição
- Usuário que editou
- O que foi alterado (ex: "Status: Pendente → Realizada")

---

## 🏆 Ranking da Equipe

Pódio visual com 🥇🥈🥉 calculado por nota ponderada:
- Produtividade (30%)
- Alinhamento com Diretrizes (25%)
- Pontualidade (15%)
- Foco no Cliente (15%)
- Liderança (10%)
- Qualidade (5%)

---

## 📄 Relatório Mensal de Performance

Gerado automaticamente com:
- Parágrafo de abertura personalizado por nível
- ✅ Pontos Fortes e Conquistas
- ⚠️ Pontos de Atenção com severidade
- 🧠 Análise de Desenvolvimento Profissional
- 📐 Indicadores Comportamentais
- 💬 Mensagem da Liderança
- 🎯 Sugestões de Metas para o próximo mês
- Exportação em PDF com campo de assinatura

---

## 🔗 Integração Google Sheets

### Passo a passo:
1. Crie uma planilha no Google Sheets
2. Vá em **Extensões → Apps Script**
3. Cole o conteúdo do arquivo `google_apps_script.js`
4. Coloque o ID da sua planilha na variável `SPREADSHEET_ID`
5. Execute a função `setupPlanilha()` uma vez
6. Publique como **Aplicativo da Web** (acesso: qualquer pessoa)
7. Copie a URL e cole em **Configurações → Google Sheets** no sistema

### Dados sincronizados:
- ✅ Atividades
- 📋 Plano de Ação

---

## 📊 Relatórios de Produtividade

Disponíveis por:
- 👤 **Pessoa** — Equipe e Rel. Mensal
- 🏢 **Setor** — Dashboard
- 📍 **Localização/Loja** — Dashboard
- 📅 **Período** — filtro em Equipe e Rel. Mensal

---

## 🛠️ Tecnologias

- HTML5 + CSS3 + JavaScript puro (sem frameworks)
- Chart.js para gráficos
- localStorage para persistência local
- Google Apps Script para sincronização com Sheets

---

## 📁 Estrutura

```
sgap/
├── index.html              # Sistema completo (arquivo único)
├── google_apps_script.js   # Script para Google Sheets
└── README.md               # Este arquivo
```

---

## 👨‍💼 Desenvolvido por

**Everest Consultoria em Gestão Empresarial**  
Sistema SGAP © 2026 — Todos os direitos reservados
