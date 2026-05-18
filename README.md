# 🏥 Sistema de Agendamento de Salas (Google Apps Script + Google Sheets)

## Descrição objetiva
Este projeto é um **WebApp operacional** para gestão de salas e agendamentos, desenvolvido em **Google Apps Script** com dados persistidos em **Google Sheets**. O sistema centraliza a rotina de marcação, bloqueio, monitoramento e auditoria de uso das salas em uma única interface web, com atualização contínua e foco em confiabilidade para operação diária.

## Problema que o sistema resolve
Em operações com múltiplas salas e equipes, o agendamento manual em planilhas dispersas costuma gerar:

- conflito de horários;
- retrabalho para ajustar ocupação;
- baixa visibilidade do status por turno;
- dificuldades para auditoria de alterações;
- dependência excessiva de pessoas-chave para “organizar a casa”.

Este sistema transforma a planilha em uma **base de dados estruturada**, com regras de negócio no Apps Script e uma interface de uso rápido para gestão real de rotina.

## Principais funcionalidades
- 🔐 **Login com acesso restrito** por matrícula/senha.
- 🖥️ **Monitor em tempo real** para visualização do status das salas.
- 📅 **Navegação por data e turno** (manhã, tarde, noite ou dia completo).
- 🧭 **Filtros avançados** por especialidade, categoria, status e ilha.
- 📝 **Planejamento operacional** com fluxo de atualização direto na base.
- 📊 **Dashboards e relatórios** para apoio à decisão.
- 🧩 **Painel de cadastros** (especialidades, categorias, ilhas e salas).
- 👨‍⚕️ **Acompanhamento de médicos** e análise de produtividade.
- 📚 **Logs e auditoria** para rastreabilidade de ações.
- 🚫 **Controle de bloqueio e status de sala** com governança operacional.

## Tecnologias utilizadas
- **Google Apps Script** (backend, regras e integração com Google Workspace)
- **Google Sheets** (persistência de dados e estrutura operacional)
- **HTML5** (estrutura da interface)
- **CSS3** (estilo e responsividade)
- **JavaScript (client-side)** (interação e estado da UI)
- **Chart.js** (visualização gráfica em dashboards)
- **Font Awesome** (ícones)
- **Google Fonts (Inter)** (tipografia)

## Estrutura do projeto
```bash
.
├── Code.gs       # Regras de negócio e integração com Google Sheets (Apps Script)
├── index.html    # Estrutura principal da interface WebApp
├── style.html    # Estilos CSS injetados via HtmlService
├── script.html   # Lógica client-side e chamadas google.script.run
├── README.md
└── PORTFOLIO.md
```

> Observação: os arquivos `style.html` e `script.html` seguem o padrão do ambiente Google Apps Script (HtmlService), por isso não usam extensão `.css`/`.js` isolada no deploy.

## Fluxo de funcionamento
1. **Usuário acessa o WebApp** e realiza autenticação.
2. **Frontend (`index.html`)** carrega estilos e scripts via includes (`style.html` e `script.html`).
3. **Ações de tela** (filtros, cadastro, edição, bloqueios) chamam funções no `Code.gs` com `google.script.run`.
4. **Apps Script processa as regras** e lê/escreve dados na planilha.
5. **Resposta retorna para interface**, que atualiza monitor, painéis e indicadores.
6. **Eventos críticos são registrados** em logs para auditoria.

## Capturas de tela
> Substitua os caminhos abaixo pelos prints reais do sistema.

### Login e controle de acesso
![Tela de login](./docs/screenshots/login.png)

### Monitor de salas e filtros
![Monitor operacional](./docs/screenshots/monitor.png)

### Painel de gestão e cadastros
![Painel de gestão](./docs/screenshots/gestao.png)

### Dashboard e indicadores
![Dashboard](./docs/screenshots/dashboard.png)

## Como executar
### 1) Pré-requisitos
- Conta Google com acesso ao **Google Apps Script**.
- Uma planilha Google Sheets para servir como base de dados.

### 2) Configuração no Apps Script
1. Abra o Apps Script vinculado à planilha (ou crie um projeto standalone e depois vincule a base).
2. Crie/atualize os arquivos com os mesmos nomes deste repositório:
   - `Code.gs`
   - `index.html`
   - `style.html`
   - `script.html`
3. Ajuste no `Code.gs` os IDs/nomes de abas e constantes da operação conforme seu ambiente.

### 3) Deploy do WebApp
1. Clique em **Deploy > New deployment**.
2. Escolha o tipo **Web app**.
3. Defina:
   - **Execute as**: sua conta (ou conta de serviço operacional).
   - **Who has access**: conforme sua política interna.
4. Autorize os escopos solicitados pelo Apps Script.
5. Copie a URL gerada e acesse no navegador.

### 4) Permissões
- Garanta permissão de leitura/escrita na planilha para a conta executora.
- Restrinja acesso do WebApp para perfis autorizados.

## Melhorias futuras
- ✅ Exportação avançada de relatórios (PDF e envio automático por e-mail).
- ✅ Alertas proativos de conflito de agenda e indisponibilidade crítica.
- ✅ Trilhas de auditoria com filtros salvos por perfil.
- ✅ Camada de configurações administrativas versionadas.
- ✅ Indicadores históricos por período, especialidade e ilha.

## Autor
**Time de Desenvolvimento / Operação Gama**  
Sistema desenhado para uso institucional com foco em eficiência operacional, rastreabilidade e redução de falhas manuais.
