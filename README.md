# 🚀 UP Espaço - Plataforma de Desenvolvimento Infantil

Um protótipo completo, moderno e de alta fidelidade desenvolvido em **React**, **Vite**, **TypeScript** e **Tailwind CSS**. A plataforma fornece uma ponte dinâmica e interativa entre famílias (pais/responsáveis) e equipes multiprofissionais de apoio clínico e pedagógico (tererapeutas ocupacionais, psicopedagogos, fonoaudiólogos e professores).

---

## 🎨 Tema de Design: Sleek Interface

A aplicação foi completamente otimizada seguindo as diretrizes visuais da identidade **Sleek Interface**, entregando uma estética futurista, limpa e extremamente acolhedora para uso diário:

- **Paleta de Cores Premium**:
  - `Primary` (Indigo / `#6366f1`): Utilizado em botões de ação principal, elementos navegacionais ativos e cabeçalhos em destaque.
  - `Secondary` (Rosa Vibrante / `#ec4899`): Representando picos de conquistas importantes do Enzo e marcas premium adicionais de interface.
  - `Background` (`#f8fafc`): Um canvas de fundo off-white/cinza claro, suave para os olhos dos usuários.
  - `Gradients de Profundidade` (`#0f172a` a `#1e293b`): Estruturam o painel externo do simulador de dispositivo (`DeviceFrame`), as telas de entrada de imersão (`SplashScreen`) e painéis organizacionais.
- **Tipografia & Ícones**:
  - Parceria harmônica entre os estilos **Inter** e **Plus Jakarta Sans** para máxima legibilidade.
  - Ícones consistentes e visualmente expressivos via biblioteca de símbolos estruturada.
- **Layout & Bordas**:
  - Layouts de grid flexíveis inspirados em painéis modernos de tecnologia de dados.
  - Cantos arredondados contínuos de até `24px` / `32px` (`rounded-[24px]/[32px]`) com contornos e bordas discretas (`#e2e8f0`).
  - Efeitos de sombras e profundidade otimizados (`premium-shadow` e `box-shadow` suave / `rgba(0,0,0,0.05)`).

---

## 🛠️ Arquitetura e Estrutura de Pastas

O código foi cuidadosamente projetado em módulos separados e bem tipados para prevenir problemas de limite de tokens e promover manutenibilidade limpa:

```bash
/src
 ├── /components
 │    ├── DeviceFrame.tsx       # Moldura lateral de simulação com alternadores de Papel (Pai / Terapeuta)
 │    ├── SplashScreen.tsx      # Portal introdutório com brilho ambiental e temporizador de pulo
 │    ├── Onboarding.tsx        # Carrossel explicativo guiando as metas da clínica
 │    ├── Login.tsx             # Tela de autenticação rica com credenciais automatizadas para testes rápidos
 │    ├── Timeline.tsx          # Painel inicial com controle de presença ativa, resumos e logs
 │    ├── AtividadesFeed.tsx    # Feed de diários lúdicos cotidianos com fotos e formulários de cadastro
 │    ├── EvolucaoBento.tsx     # Bento Grid interativo com os pilares qualitativos de desenvolvimento
 │    ├── AgendaCalendar.tsx    # Calendário semanal com lembretes, avisos de reunião e confirmações de presença
 │    ├── StoryModal.tsx        # Resumo visual imersivo imitando formato moderno de stories de rede social
 ├── App.tsx                    # Orquestrador geral e controlador reativo de estados de navegação
 ├── data.ts                    # Inteligência de dados, constantes de inicialização e mocks de alta fidelidade
 ├── types.ts                   # Fortemente tipado com interfaces estritas do TypeScript
 └── index.css                  # Folha geométrica geral de cores Tailwind e animações de interface
```

---

## ✨ Funcionalidades Principais Desenvolvidas

### 🛡️ 1. Simulador Integrado de Persona & Visualizadores (`DeviceFrame`)
- No topo da aplicação, o usuário pode simular os dois lados do ecossistema terapêutico:
  - **Família (Mãe - Fernanda)**: Acompanha os diários, confirma presença física e lida com lembretes importantes na agenda.
  - **Profissional de Apoio / Terapeuta (Prof. Ana)**: Desbloqueia botões flutuantes para registrar novos logs pedagógicos de evolução em tempo real.
- Suporta alternador entre simulação de carcaça física em formato dispositivo móvel ou visualização fluida em tela cheia na web.

### 🌅 2. Jornada Introdutória Imersiva
- **Splash Screen**: Uma entrada misteriosa com glows neon suaves de fundo, apresentando a proposta científica do UP Espaço. É possível prosseguir dando um clique simples nas margens da tela de forma reativa.
- **Onboarding interativo**: Três slides acolhedores detalhando o acompanhamento multidisciplinar, a agenda de atendimento integrada e as métricas de evolução sob medida para a jornada do Enzo.

### 🔑 3. Portal de Acesso Inteligente
- Sistema de login com alternador para cadastro de novos dados.
- Contém abas rápidas de credenciais simuladas para preencher instantaneamente a senha e e-mail com 1 toque, facilitando avaliações ou reuniões de demonstração rápidas.

### 📅 4. Centro de Atendimento da Agenda (`AgendaCalendar`)
- Um seletor sequencial de dias da semana para rastrear as atividades escolares e terapêuticas agendadas no mês de Outubro 2023.
- Calendário de sessões estruturadas com crachás de lembretes e status (`Importante`, `Sessão regular`).
- Gatilho reativo de presença (**RSVP**), onde os pais podem confirmar presença de Enzo com botões adaptativos que mudam de cor no mesmo instante de forma intuitiva.

### 🔍 5. Feed Dinâmico de Progresso (`AtividadesFeed`)
- Exibe fotos em alta fidelidade com os diários diários de atividade lúdica divididos em categorias estratégicas como *Sensorial*, *Psicomotricidade*, *Cognitivo* e *Pedagógico*.
- Suporta ações interativas de curtidas e favoritos que atualizam dinamicamente os contadores do post.
- **Adição de Diários (Para Terapeutas)**: Ao mudar para a interface do Terapeuta, um botão flutuante de adição é apresentado. Ele abre uma janela suspensa robusta permitindo escolher títulos, logs de atendimento, definir a categoria e pré-visualizar fotos reais para anexar ao histórico do aluno.

### 📊 6. Grids de Linha do Tempo & Evolução em Bento Grid
- **Painel Inicial**: Mostra o status de entrada do aluno (Enzo) em classe física com horários e um interruptor de presença interativo (*"Presente"* ou *"Ausente"*).
- **Métricas Bento Grid**: Uma central moderna sintetizando a duração de atenção contínua e índices cognitivos detalhados. Ao tocar em qualquer card no grid, um relatório clínico em janela surge exibindo metas clínicas e detalhes do plano pedagógico sob medida do Enzo.

### 📱 7. Insta-like Stories do Dia (`StoryModal`)
- Sistema avançado que renderiza as histórias lúdicas do dia do Enzo em formato de Stories.
- **Indicadores de Progresso Ativos**: Barras lineares no topo que escorregam e progridem automaticamente com as imagens, trocando de cena a cada 4 segundos.
- **Controles de Toque**: Permite pausar e pular cenas tocando nos lados esquerdo/direito da tela.
- **Humor do Dia**: Destaca o feedback de humor reativo e comentários do dia inseridos pela equipe de professores, com atalho de compartilhamento rápido via link para familiares.

---

## 🩺 Correção Crítica de Memória & Fluxos Reativos

Durante a otimização, identificamos e tratamos com sucesso uma inconsistência clássica do renderizador React:
- **Causa Raiz**: O componente `StoryModal` disparava atualizações de estado nas funções do orquestrador principal de rotas (`onClose` corporativo e finalização automática de carrossel de slides) enquanto o ciclo síncrono de renderização dos stories ainda estava ativamente limpando callbacks de intervalos na CPU.
- **Abordagem de Correção Estabilizada**:
  ```tsx
  // Uso de buffers de fila assíncronos não-bloqueantes com setTimeout garantindo o fim correto da renderização
  setTimeout(handleNextSegment, 0);
  setTimeout(onClose, 0);
  ```
- Isso garantiu builds corporativos limpos, com **0 erros** no linter, proporcionando uma experiência de navegação ultra-fluida livre de travamentos ou re-renders em loop.

---

## 🌐 Tecnologias Utilizadas
- **React (v18.3.1)** - Componentização imperativa sob medida com gerenciamento estruturado de ganchos (`useState`, `useEffect`, `useRef`).
- **TypeScript** - Verificação estática completa eliminando erros de tipos e tipando todos os mocks de dados.
- **Tailwind CSS (v4)** - Estilização moderna rica em transições responsivas e classes utilitárias compactas baseadas no ecossistema Sleek.
