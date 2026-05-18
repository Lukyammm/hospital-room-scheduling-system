# 🚀 Sistema de Agendamento de Salas — Caso real de transformação operacional

## Introdução estratégica
Este projeto foi construído como uma solução de operação real para ambientes com alta demanda de coordenação entre pessoas, salas, turnos e prioridades.  
A proposta foi simples e objetiva: **tirar o agendamento do modo “planilha manual” e levar para um fluxo digital confiável, auditável e com visão gerencial em tempo real**.

Mais do que uma tela bonita, o sistema entrega **orquestração operacional**: organiza cadastros, reduz conflitos de uso, melhora rastreabilidade e dá previsibilidade para quem decide e para quem executa.

---

## 🧩 Contexto do problema operacional
Antes da digitalização, o cenário típico envolvia:

- registros distribuídos e inconsistentes;
- atualização manual suscetível a erro;
- baixa visibilidade de ocupação por turno;
- dificuldade para identificar gargalos de salas;
- pouca rastreabilidade sobre quem alterou cada informação.

Em operações assistenciais e administrativas, esse tipo de fragilidade impacta produtividade, qualidade e tempo de resposta.

---

## ✅ Como o sistema melhorou o processo
A solução implementada com Google Apps Script + Google Sheets trouxe uma mudança prática de rotina:

- **centralização da operação** em uma interface web única;
- **padronização de cadastros** (especialidades, categorias, ilhas e salas);
- **monitor operacional em tempo real** para leitura rápida do cenário;
- **controle por data e turno** para planejamento mais preciso;
- **filtros inteligentes** que aceleram buscas e decisões;
- **logs de auditoria** para segurança e governança.

Resultado: menos retrabalho, menos erro manual e maior fluidez entre gestão e execução.

---

## 🛠️ Diferenciais técnicos e funcionais
- Arquitetura simples e sustentável para ambiente Google Workspace.
- Separação clara entre **camada de interface** (`index.html`, `style.html`, `script.html`) e **camada de regras** (`Code.gs`).
- Modelo de dados orientado a operação usando Google Sheets como backend estruturado.
- Interface com linguagem de produto: navegação por módulos, painéis de gestão, estados de uso e feedback visual.
- Expansível para integrações com Gmail, Drive, Docs, Calendar e rotinas de relatório automatizado.

---

## ⚙️ Principais automações
- Autenticação e controle de acesso.
- Atualização dinâmica da interface sem recarga completa da página.
- Persistência automática das alterações na base.
- Gestão de status de salas (livre, ocupado, bloqueado, reservado).
- Registro de alterações para auditoria e histórico operacional.
- Consolidação de informações para análise gerencial e acompanhamento de performance.

---

## 📈 Resultados e impacto
Mesmo sem alterar a estrutura principal da operação, o sistema eleva o nível de maturidade do processo:

- **Redução de falhas manuais** em registros e remarcações.
- **Ganho de velocidade** na tomada de decisão por turno/dia.
- **Melhor governança** com trilha de auditoria.
- **Maior transparência** para equipes e liderança.
- **Base pronta para evolução** (analytics, alertas e relatórios executivos).

> Em termos de produto, a solução reposiciona a planilha: de ferramenta manual para **motor de dados de um WebApp operacional**.

---

## 🧪 Tecnologias utilizadas
- Google Apps Script
- Google Sheets
- HTML5
- CSS3
- JavaScript
- Chart.js
- Font Awesome
- Google Fonts (Inter)

---

## 🖼️ Prints / mockups destacados
> Espaço reservado para evidências visuais do projeto em produção.

- **Tela de Login e Segurança**  
  `./docs/screenshots/login.png`

- **Monitor Operacional de Salas**  
  `./docs/screenshots/monitor.png`

- **Painel de Cadastros e Gestão**  
  `./docs/screenshots/gestao.png`

- **Dashboards e Indicadores**  
  `./docs/screenshots/dashboard.png`

---

## Conclusão (produto e solução real)
Este projeto representa uma entrega com visão de produto: resolve um problema concreto de operação, melhora o fluxo diário de trabalho e cria base confiável para escala.  

É uma solução pragmática, sustentável e orientada a resultado — com equilíbrio entre tecnologia, usabilidade e governança.
