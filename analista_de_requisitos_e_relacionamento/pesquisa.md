# Levantamento de Requisitos de Software
## Up Espaço Multiprofissional — Faxinal do Soturno / RS
### Aplicativo de Comunicação e Acompanhamento Infantil

**Versão:** 1.0  
**Data:** Junho de 2026  
**Classificação:** Documento Estratégico — Uso Interno  
**Elaborado por:** Análise de Requisitos Sênior com suporte de pesquisa digital

---

## Sumário

1. [Resumo Executivo](#1-resumo-executivo)
2. [Apresentação da Entidade](#2-apresentação-da-entidade)
3. [Pesquisa Institucional](#3-pesquisa-institucional)
4. [Perfil dos Usuários](#4-perfil-dos-usuários)
5. [Diagnóstico das Dores](#5-diagnóstico-das-dores)
6. [Oportunidades de Solução](#6-oportunidades-de-solução)
7. [Benchmarking de Mercado](#7-benchmarking-de-mercado)
8. [Requisitos do Sistema](#8-requisitos-do-sistema)
9. [Sugestão de MVP](#9-sugestão-de-mvp)
10. [Roadmap Futuro](#10-roadmap-futuro)
11. [Conclusão](#11-conclusão)
12. [Referências](#12-referências)

---

## 1. Resumo Executivo

A **Up Espaço Multiprofissional**, localizada em Faxinal do Soturno (RS), é uma instituição voltada ao desenvolvimento infantil por meio de atendimentos terapêuticos e pedagógicos multidisciplinares. A instituição atende crianças em diferentes fases do desenvolvimento, com foco em áreas como psicomotricidade, comunicação, coordenação motora, interação social e autonomia.

O principal gargalo operacional identificado reside na **comunicação manual e fragmentada com os responsáveis pelas crianças**. A equipe profissional despende tempo significativo em tarefas repetitivas como o envio individualizado de fotos e vídeos, respostas a dúvidas recorrentes, controle de presença e atualização de evoluções terapêuticas — atividades que poderiam ser automatizadas e centralizadas por meio de tecnologia.

Este documento propõe o desenvolvimento de um **aplicativo mobile dedicado** que centralize a comunicação, o registro de atividades, a agenda, o acompanhamento de presença e a jornada evolutiva de cada criança. A solução foi concebida com base em pesquisa de mercado, análise de concorrentes nacionais e internacionais, e orientação pelos princípios da LGPD aplicados ao contexto de dados sensíveis de menores.

O MVP proposto contempla as funcionalidades de maior impacto imediato para redução de retrabalho e melhoria da experiência dos pais, com um roadmap de evolução planejado para versões futuras.

---

## 2. Apresentação da Entidade

### 2.1 Identificação

| Campo | Informação |
|---|---|
| **Razão Social** | Up Espaço Multiprofissional |
| **Localização** | Faxinal do Soturno, Rio Grande do Sul, Brasil |
| **Natureza** | Instituição privada de atendimento multiprofissional infantil |
| **Segmento** | Saúde e Educação / Desenvolvimento Infantil |
| **Público Primário** | Crianças em fase de desenvolvimento (0–12 anos) e seus responsáveis |

### 2.2 Contexto Regional

Faxinal do Soturno é um município de aproximadamente **6.846 habitantes** (estimativa IBGE 2025), localizado na região central do Rio Grande do Sul. Com uma população relativamente pequena e índice de desenvolvimento humano municipal de **0,720** (IBGE 2010), o município representa um contexto típico de interior gaúcho: comunidade próxima, forte coesão social e demanda crescente por serviços especializados de saúde e educação que historicamente estão concentrados em centros maiores como Santa Maria.

Nesse cenário, a Up Espaço Multiprofissional ocupa um papel estratégico como **referência regional** no atendimento terapêutico-pedagógico infantil, absorvendo demandas de famílias do próprio município e de cidades vizinhas.

### 2.3 Missão (Inferida)

Promover o desenvolvimento integral de crianças por meio de atendimentos multidisciplinares acolhedores, estimulando habilidades cognitivas, motoras, comunicativas e socioemocionais com abordagem lúdica e humanizada.

### 2.4 Visão (Inferida)

Ser a principal referência em desenvolvimento infantil multiprofissional da região central do Rio Grande do Sul, reconhecida pelo impacto positivo na vida das crianças atendidas e pelo alto engajamento das famílias no processo terapêutico-pedagógico.

### 2.5 Valores (Inferidos)

- Acolhimento e cuidado humanizado
- Abordagem lúdica e respeitosa ao tempo de cada criança
- Transparência na comunicação com as famílias
- Trabalho colaborativo entre profissionais
- Responsabilidade com o desenvolvimento integral

### 2.6 Diferenciais Competitivos

- Atendimento multiprofissional integrado em um único espaço
- Localização estratégica em município de interior com escassez de serviços especializados
- Abordagem afetiva e personalizada para cada criança
- Equipe com formação nas áreas de educação e saúde
- Potencial de digitalização ainda não explorado — janela de oportunidade para se diferenciar frente a concorrentes

---

## 3. Pesquisa Institucional

### 3.1 Modelo de Operação

Com base nas informações fornecidas e em pesquisa de mercado sobre instituições similares no Brasil, a Up Espaço Multiprofissional opera com o seguinte modelo:

**Fluxo atual de atendimento:**
1. Agendamento de sessões por telefone/WhatsApp
2. Recepção e encaminhamento das crianças às salas de atividade
3. Realização de sessões terapêuticas ou pedagógicas
4. Registro manual de atividades e evolução
5. Captura de fotos e vídeos durante as sessões
6. Envio individual por WhatsApp para cada responsável
7. Resposta a dúvidas via mensagem individual
8. Controle de presença em planilhas ou cadernos físicos

### 3.2 Profissionais Envolvidos (Perfil Típico de Espaços Similares)

Com base em comparação com instituições multiprofissionais semelhantes no Rio Grande do Sul, a equipe de um espaço como a Up provavelmente é composta por:

- Psicomotricistas
- Pedagogos / Psicopedagogos
- Fonoaudiólogos
- Terapeutas Ocupacionais
- Psicólogos (infantis)
- Professores de atividades complementares (música, artes, etc.)
- Equipe administrativa

### 3.3 Comunicação Atual com Famílias

O principal canal de comunicação atualmente utilizado é o **WhatsApp**, tanto para mensagens individuais quanto, possivelmente, grupos. Esse modelo, embora familiar e acessível, gera os seguintes problemas estruturais:

- Ausência de privacidade (número pessoal dos profissionais exposto)
- Dificuldade de rastreamento e histórico de comunicações
- Risco de não conformidade com a LGPD (dado de saúde de crianças trafegando em plataforma de terceiros sem controle)
- Retrabalho no envio individualizado de conteúdos idênticos para múltiplas famílias
- Ruídos de comunicação e informações perdidas

### 3.4 Desafios Identificados na Gestão

- Ausência de sistema centralizado de agenda
- Controle manual de presenças e faltas
- Falta de padronização nos registros de evolução
- Ausência de canal oficial de comunicação institucional
- Dificuldade de engajar famílias no processo terapêutico fora do horário de sessão

---

## 4. Perfil dos Usuários

### 4.1 Perfil das Crianças Atendidas

As crianças atendidas em espaços multiprofissionais como a Up Espaço geralmente apresentam:

- Faixa etária: 1 a 12 anos (com maior concentração entre 2 e 8 anos)
- Diversidade de necessidades: atrasos no desenvolvimento motor, de linguagem, cognitivo ou social
- Presença de diagnósticos como TEA (Transtorno do Espectro Autista), TDAH, Síndrome de Down, dislexia, atraso global do desenvolvimento, entre outros
- Crianças em desenvolvimento típico com necessidade de estimulação complementar
- Crianças com indicação de reforço escolar e apoio psicopedagógico

### 4.2 Perfil dos Responsáveis (Usuários Primários do App)

**Dados demográficos típicos:**
- Pais, mães, avós ou responsáveis legais
- Faixa etária: 25 a 55 anos
- Nível de escolaridade variado (ensino médio a superior)
- Familiaridade com smartphone e redes sociais (Instagram, Facebook, WhatsApp)
- Residentes em Faxinal do Soturno e municípios da região

**Necessidades emocionais e informacionais:**
- Desejam sentir-se **parte ativa** do processo terapêutico do filho
- Buscam **tranquilidade e segurança** ao deixar a criança nos cuidados da instituição
- Querem **evidências visuais** do progresso da criança (fotos, vídeos, registros)
- Precisam de **clareza e simplicidade** nas informações — sem jargões clínicos
- Valorizam **disponibilidade e agilidade** na comunicação
- Sentem-se frustrados com informações fragmentadas ou tardias
- Têm pouco tempo disponível (muitos trabalham durante o horário das sessões)

**Comportamentos digitais:**
- Usuários ativos de WhatsApp e Instagram
- Experiência média a baixa com aplicativos especializados
- Expectativa de interface simples, visual e intuitiva
- Sensíveis à exposição de imagens dos filhos — exigem privacidade e controle

### 4.3 Perfil dos Profissionais (Usuários Secundários do App)

- Professores e terapeutas com formação nas áreas de saúde e educação
- Familiaridade com smartphones, mas nem sempre com ferramentas digitais profissionais
- Necessidade de soluções rápidas que não aumentem a carga de trabalho
- Interesse em registro padronizado e histórico acessível das evoluções
- Equipe administrativa com necessidade de controle de agenda e presenças

---

## 5. Diagnóstico das Dores

### 5.1 Mapa de Dores por Dimensão

#### 5.1.1 Comunicação
| Dor | Impacto | Urgência |
|---|---|---|
| Envio individual de fotos/vídeos por WhatsApp | Alto (retrabalho diário) | Alta |
| Exposição do número pessoal dos profissionais | Alto (privacidade/LGPD) | Alta |
| Ausência de canal oficial de comunicação | Alto (inconsistência) | Alta |
| Informações perdidas em grupos de WhatsApp | Médio | Média |
| Resposta repetitiva a dúvidas frequentes | Médio (tempo) | Média |

#### 5.1.2 Organização e Agenda
| Dor | Impacto | Urgência |
|---|---|---|
| Controle manual de presenças e faltas | Médio | Média |
| Ausência de lembretes automáticos para pais | Alto (faltas não justificadas) | Alta |
| Dificuldade de comunicar alterações de horário | Alto | Alta |
| Gestão de agenda sem visão consolidada | Médio | Média |

#### 5.1.3 Registro e Evolução
| Dor | Impacto | Urgência |
|---|---|---|
| Registros em cadernos físicos sem padronização | Alto (perda de dados) | Alta |
| Pais sem acesso ao progresso entre as sessões | Alto (desengajamento) | Alta |
| Ausência de histórico evolutivo acessível | Alto (continuidade do cuidado) | Alta |
| Relatórios gerados manualmente por cada profissional | Alto (retrabalho) | Média |

#### 5.1.4 Engajamento das Famílias
| Dor | Impacto | Urgência |
|---|---|---|
| Pais sentem-se "de fora" do processo terapêutico | Alto (vínculo e confiança) | Alta |
| Baixa adesão às orientações domiciliares | Alto (resultados) | Alta |
| Dificuldade de celebrar conquistas com os pais | Médio (motivação) | Baixa |

### 5.2 Impacto das Dores

**Impacto na equipe:**
A sobrecarga comunicacional representa um **desvio de função** dos profissionais, que passam tempo valioso em tarefas administrativas ao invés de se dedicar ao cuidado e planejamento terapêutico. Estima-se que em clínicas de porte similar, cada profissional dedica entre 30 e 60 minutos diários a tarefas de comunicação e registro que poderiam ser automatizadas — um equivalente a mais de **2 horas semanais por profissional** de retrabalho evitável.

**Impacto nos pais:**
A ausência de um canal centralizado gera ansiedade nos responsáveis, que frequentemente não sabem o que acontece nas sessões e precisam aguardar até buscar a criança para obter informações. Essa lacuna pode gerar **desconfiança e menor engajamento** no processo terapêutico.

**Impacto na criança:**
O progresso terapêutico é potencializado quando os comportamentos e habilidades trabalhados em sessão são reforçados no ambiente familiar. Sem comunicação eficiente com os pais, essa **generalização** não ocorre de forma adequada, comprometendo a velocidade e consistência do desenvolvimento.

**Custos operacionais:**
- Tempo médio estimado de comunicação por profissional: 45 min/dia
- Com 5 profissionais: 225 min/dia = 3,75 horas/dia de equipe em tarefas não clínicas
- Anualizado: aproximadamente 945 horas/ano de capacidade produtiva consumida em comunicação manual

---

## 6. Oportunidades de Solução

### 6.1 Visão da Solução

Desenvolver um **aplicativo mobile multiplataforma** (iOS e Android), com painel web de gestão para profissionais, que centralize toda a comunicação, registro e acompanhamento de desenvolvimento infantil da Up Espaço Multiprofissional.

A solução deve ser:
- **Simples e acolhedora** na interface — linguagem visual próxima à identidade da instituição
- **Rápida** para os profissionais registrarem atividades sem aumentar carga de trabalho
- **Engajante** para os pais — mais parecida com um feed de bem-estar do que com um portal clínico
- **Segura e em conformidade** com a LGPD

### 6.2 Proposta de Valor por Público

| Público | Proposta de Valor |
|---|---|
| **Pais/Responsáveis** | "Acompanhe cada conquista do seu filho, de onde estiver, com segurança e carinho." |
| **Profissionais** | "Registre, comunique e organize em minutos. Sem retrabalho, sem WhatsApp pessoal." |
| **Gestão da instituição** | "Visão completa da operação, comunicação unificada e conformidade com a LGPD." |

---

## 7. Benchmarking de Mercado

### 7.1 ClassApp (Brasil)

**Descrição:** Aplicativo de comunicação escolar líder no mercado brasileiro, com mais de 600 instituições parceiras. Conecta escola, pais e alunos de forma centralizada.

**Funcionalidades Principais:**
- Agenda digital do aluno
- Troca de mensagens entre escola e família
- Compartilhamento de fotos e vídeos de eventos
- Comunicados e circulares oficiais
- Lembretes automáticos para reuniões e compromissos
- Autorização eletrônica de passeios
- Relatório de sono e banho (para berçário)
- Enquetes interativas com pais

**Pontos Fortes:**
- Substitui WhatsApp e e-mail de forma eficiente
- Conformidade com LGPD
- Confirmação de leitura de comunicados
- Interface simples e acessível
- Premiado como melhor app de comunicação escolar (Top Educação)
- Escolas parceiras cresceram até 4x mais que a média do mercado após adoção

**Pontos Fracos:**
- Focado em contexto escolar — sem funcionalidades para evolução terapêutica
- Não possui visualização de objetivos ou metas individuais por criança
- Modelo de precificação por aluno pode ser caro para espaços pequenos
- Sem módulo de acompanhamento de neurodesenvolvimento

**Oportunidade para o App da Up:** Incorporar a facilidade comunicacional do ClassApp com camadas terapêuticas que ele não oferece — como a Jornada de Evolução.

---

### 7.2 ODAPP (Brasil)

**Descrição:** Plataforma de gestão terapêutica completa focada em crianças com autismo (TEA), conectando família, terapeuta, clínica, escola e operadora de saúde.

**Funcionalidades Principais:**
- Prontuário eletrônico especializado para TEA
- Registro de evolução por sessão com gráficos
- Plano de Ensino Individualizado (PEI)
- Compartilhamento de dados entre equipe terapêutica e família
- Acompanhamento de horas de intervenção
- Conformidade com LGPD e recomendações dos conselhos de classe

**Pontos Fortes:**
- Integração real entre família, clínica e escola
- Dados distribuídos entre diferentes ambientes de intervenção
- Gráficos e relatórios especializados para TEA

**Pontos Fracos:**
- Muito técnico para pais sem formação na área
- Foco exclusivo em TEA — não serve para desenvolvimento típico ou outras demandas
- Interface clínica, sem apelo emocional ou lúdico para os responsáveis
- Custo provavelmente elevado para instituições pequenas

**Oportunidade para o App da Up:** Inspirar-se na profundidade de registro do ODAPP, mas com interface mais acolhedora e linguagem acessível para pais.

---

### 7.3 ConnectTEA (Brasil)

**Descrição:** Plataforma para aplicação de intervenção precoce baseada no método ESDM (Early Start Denver Model), conectando profissionais e famílias de crianças com autismo.

**Funcionalidades Principais:**
- Leitura fácil de objetivos e evolução da criança
- Interação entre família e equipe terapêutica
- Gráficos de fácil interpretação para não especialistas
- Dados pertencentes à família (portabilidade)
- Conformidade com LGPD

**Pontos Fortes:**
- Linguagem acessível aos pais — diferencial relevante
- Empoderamento familiar após diagnóstico
- Dados seguros e portáveis

**Pontos Fracos:**
- Escopo restrito ao método ESDM
- Não possui funcionalidades de agenda, feed ou RSVP

**Oportunidade para o App da Up:** O ConnectTEA demonstra que pais querem e conseguem entender informações de evolução quando apresentadas de forma clara — validando o conceito da Jornada de Evolução proposta para o app.

---

### 7.4 Ninsaúde Clinic (Brasil)

**Descrição:** Software de gestão clínica voltado a profissionais de saúde, com prontuário eletrônico, agenda, teleconsulta e módulos de acompanhamento de evolução.

**Funcionalidades Principais:**
- Prontuário eletrônico com validade jurídica
- Agenda ágil e completa
- Controle financeiro e faturamento de convênios
- Teleconsulta integrada
- Gráficos de evolução clínica
- CRM para segmentação de pacientes

**Pontos Fortes:**
- Solução robusta para gestão clínica
- Prontuário com validade jurídica
- Vários módulos integrados

**Pontos Fracos:**
- Não possui interface para pais/responsáveis
- Foco em gestão interna — sem canal de comunicação com famílias
- Custo elevado para pequenas instituições

**Oportunidade para o App da Up:** O Ninsaúde representa o "lado profissional" da gestão; o app da Up deve complementar com o "lado família" — o que nenhum software de gestão clínica oferece de forma nativa.

---

### 7.5 Bloomz / Remind (EUA)

**Descrição:** Plataformas americanas de comunicação entre educadores e famílias, amplamente utilizadas em escolas de educação infantil.

**Funcionalidades Principais (Bloomz):**
- Feed de sala de aula com fotos e atualizações
- Calendário de eventos e RSVP
- Mensagens privadas entre professor e família
- Portfólio digital da criança
- Controle de voluntários e compromissos

**Pontos Fortes:**
- Interface visual e amigável, similar a redes sociais
- Controle de privacidade granular por criança
- RSVP integrado ao feed de atividades

**Pontos Fracos:**
- Sem suporte a português / mercado brasileiro
- Foco escolar — sem camada terapêutica
- Funcionalidades de evolução limitadas

**Oportunidade para o App da Up:** O Bloomz valida o conceito de "feed de sala de atividades" — a abordagem visual-social proposta para o app é consistente com soluções internacionais bem-sucedidas.

---

### 7.6 Análise Comparativa

| Solução | Comunicação | Feed Atividades | Evolução Terapêutica | Agenda/RSVP | Interface p/ Pais | Mercado BR |
|---|---|---|---|---|---|---|
| ClassApp | ✅ Excelente | ✅ Bom | ❌ Não | ✅ Bom | ✅ Boa | ✅ Sim |
| ODAPP | 🔶 Parcial | ❌ Não | ✅ Excelente | ❌ Não | 🔶 Técnica | ✅ Sim |
| ConnectTEA | 🔶 Parcial | ❌ Não | ✅ Bom | ❌ Não | ✅ Boa | ✅ Sim |
| Ninsaúde | ❌ Interno | ❌ Não | 🔶 Interno | ✅ Bom | ❌ Não | ✅ Sim |
| Bloomz | ✅ Excelente | ✅ Excelente | ❌ Não | ✅ Excelente | ✅ Excelente | ❌ Não |
| **App Up (Proposto)** | **✅ Centralizada** | **✅ Feed Lúdico** | **✅ Bento Grid** | **✅ RSVP** | **✅ Acolhedora** | **✅ Sim** |

**Conclusão do benchmarking:** Existe uma **lacuna clara de mercado** para uma solução que una a comunicação visual do Bloomz, a profundidade terapêutica do ODAPP/ConnectTEA e a simplicidade do ClassApp — com interface acolhedora voltada às famílias e desenvolvida para o contexto brasileiro. O app da Up tem potencial de ocupar esse espaço com um produto genuinamente inovador.

---

## 8. Requisitos do Sistema

### 8.1 Requisitos Funcionais

#### RF01 — Autenticação e Controle de Acesso
- RF01.1: O sistema deve permitir cadastro de responsáveis mediante convite institucional (não cadastro aberto)
- RF01.2: O sistema deve suportar diferentes perfis: Administrador, Profissional, Responsável
- RF01.3: Autenticação por e-mail/senha com opção de recuperação de acesso
- RF01.4: Suporte a múltiplos responsáveis por criança (pai, mãe, avós)
- RF01.5: Cada responsável deve ter acesso apenas às informações das crianças vinculadas ao seu perfil

#### RF02 — Feed de Atividades
- RF02.1: Profissionais devem poder publicar posts com fotos, vídeos e texto descritivo das atividades
- RF02.2: Publicações devem ser direcionadas à turma/grupo ou a uma criança específica
- RF02.3: Responsáveis visualizam apenas publicações relacionadas às suas crianças
- RF02.4: Feed deve exibir postagens em ordem cronológica reversa
- RF02.5: Responsáveis devem poder reagir às publicações (curtida/coração) sem comentários abertos
- RF02.6: Profissionais devem poder moderar e deletar qualquer publicação
- RF02.7: Publicações devem suportar até 10 fotos ou 1 vídeo de até 3 minutos

#### RF03 — Agenda e RSVP
- RF03.1: O sistema deve exibir agenda semanal com eventos, sessões e compromissos
- RF03.2: Responsáveis devem poder confirmar presença ou informar falta com antecedência mínima configurável
- RF03.3: O sistema deve enviar lembretes automáticos (push notifications) 24h e 1h antes dos compromissos
- RF03.4: Profissionais e administradores podem criar, editar e cancelar eventos
- RF03.5: Cancelamento de evento pela instituição deve gerar notificação imediata a todos os responsáveis impactados
- RF03.6: Histórico de presenças e faltas deve ser registrado automaticamente

#### RF04 — Jornada de Evolução (Bento Grid)
- RF04.1: Cada criança deve ter um painel visual de evolução com áreas configuráveis (ex.: Psicomotricidade, Comunicação, Coordenação Motora, Interação Social, Autonomia)
- RF04.2: Profissionais devem poder definir objetivos e metas para cada área
- RF04.3: O sistema deve registrar metas alcançadas e exibir progresso visual (ex.: barra de progresso, ícones desbloqueados)
- RF04.4: Responsáveis devem poder visualizar objetivos, metas alcançadas e próximos passos ao clicar em cada área
- RF04.5: Linguagem das evoluções deve ser acessível — sem jargões clínicos — para leitura pelos pais
- RF04.6: Histórico evolutivo deve ser preservado ao longo do tempo
- RF04.7: Profissionais podem adicionar comentários e observações às áreas de desenvolvimento

#### RF05 — Comunicados e Avisos
- RF05.1: Administradores e profissionais podem enviar comunicados para todos os responsáveis ou para grupos específicos
- RF05.2: Comunicados devem gerar push notification e registro de confirmação de leitura
- RF05.3: Canal de comunicados deve ser unidirecional (responsáveis recebem, não respondem neste canal)
- RF05.4: Deve haver histórico de todos os comunicados enviados

#### RF06 — Controle de Presença
- RF06.1: Profissionais podem registrar presença/falta por sessão diretamente no app
- RF06.2: Responsáveis visualizam o histórico de frequência da criança
- RF06.3: Relatório de frequência deve ser exportável pela gestão

#### RF07 — Gestão (Painel Administrativo Web)
- RF07.1: Painel web para gestão de crianças, responsáveis e profissionais
- RF07.2: Geração de relatórios de frequência por período
- RF07.3: Controle de convites enviados e status de cadastro de responsáveis
- RF07.4: Visualização consolidada de todos os eventos da agenda

### 8.2 Requisitos Não Funcionais

#### RNF01 — Segurança e Privacidade

- **RNF01.1 — LGPD (Lei 13.709/2018):** O sistema deve estar em plena conformidade com a LGPD, especialmente com o Artigo 14, que regula o tratamento de dados pessoais de crianças menores de 16 anos, exigindo consentimento expresso do responsável legal.
- **RNF01.2 — Consentimento:** O cadastro de crianças no sistema deve ser precedido de aceite explícito dos Termos de Uso e da Política de Privacidade pelo responsável legal, com linguagem simples, clara e acessível.
- **RNF01.3 — Dados sensíveis:** Dados de saúde e desenvolvimento das crianças são classificados como dados sensíveis (art. 5º, II, LGPD) e devem receber proteção reforçada: criptografia em repouso e em trânsito (TLS 1.3 / AES-256), acesso restrito por perfil e logs de auditoria.
- **RNF01.4 — Imagens:** Fotos e vídeos de crianças devem ser armazenados em ambiente seguro, sem acesso público, com URL assinada e temporária (pre-signed URLs).
- **RNF01.5 — DPO:** A instituição deve designar um Encarregado de Proteção de Dados (DPO) para supervisionar a conformidade.
- **RNF01.6 — Exclusão de dados:** O sistema deve permitir a solicitação de exclusão de todos os dados de uma criança pelo responsável legal (direito ao esquecimento).
- **RNF01.7 — Portabilidade:** O sistema deve suportar exportação de dados de evolução da criança em formato aberto (PDF ou JSON) a pedido do responsável.
- **RNF01.8 — Retenção:** Definir e documentar política de retenção de dados: durante quanto tempo registros são mantidos após encerramento do atendimento.

#### RNF02 — Performance

- **RNF02.1:** O app deve carregar a tela inicial em menos de 3 segundos em conexão 4G.
- **RNF02.2:** O upload de fotos deve ser otimizado com compressão antes do envio, sem perda de qualidade perceptível.
- **RNF02.3:** O sistema deve suportar crescimento até 500 crianças cadastradas sem degradação de performance.
- **RNF02.4:** Notificações push devem ser entregues em menos de 30 segundos após disparo.

#### RNF03 — Usabilidade

- **RNF03.1:** A interface para responsáveis deve seguir princípios de design emocional — cores acolhedoras, ícones ilustrativos e linguagem afetiva.
- **RNF03.2:** O fluxo para profissionais postarem no feed não deve exigir mais de 3 toques desde a abertura do app.
- **RNF03.3:** O app deve funcionar em modo offline parcial — permitindo visualizar o conteúdo carregado anteriormente sem conexão.
- **RNF03.4:** O tamanho do texto deve ser configurável para acessibilidade (suporte a texto grande do sistema operacional).

#### RNF04 — Acessibilidade

- **RNF04.1:** Cumprir as diretrizes WCAG 2.1 nível AA para contraste de cores e legibilidade.
- **RNF04.2:** Suporte a leitores de tela (VoiceOver/TalkBack) nos elementos principais de navegação.
- **RNF04.3:** Evitar dependência exclusiva de cores para transmitir informações.

#### RNF05 — Tecnologia

- **RNF05.1:** O app deve ser desenvolvido para iOS (14+) e Android (10+).
- **RNF05.2:** Recomenda-se o uso de tecnologia cross-platform (React Native ou Flutter) para reduzir custo de desenvolvimento e manutenção.
- **RNF05.3:** Backend deve ser desenvolvido com API RESTful documentada, permitindo integrações futuras.
- **RNF05.4:** Armazenamento de mídia em serviço de nuvem confiável (AWS S3, Google Cloud Storage ou similar) com backup automático diário.
- **RNF05.5:** O painel administrativo web deve funcionar nos navegadores Chrome, Firefox, Safari e Edge nas versões dos últimos 2 anos.

#### RNF06 — Disponibilidade

- **RNF06.1:** SLA de disponibilidade mínima de 99,5% mensais.
- **RNF06.2:** Janelas de manutenção programadas fora do horário de pico (entre 00h e 05h).

---

## 9. Sugestão de MVP

### 9.1 Critérios de Priorização

O MVP foi definido com base nos critérios:
- **Maior impacto na redução de retrabalho da equipe**
- **Maior impacto na experiência dos pais**
- **Viabilidade técnica em prazo reduzido**
- **Conformidade mínima com LGPD**

### 9.2 Funcionalidades do MVP (Versão 1.0)

#### Módulo 1 — Autenticação e Onboarding
- Cadastro de crianças pelo administrador
- Convite de responsáveis por link seguro (sem cadastro aberto)
- Perfis: Administrador, Profissional, Responsável
- Aceite de Termos de Uso e Política de Privacidade com registro de consentimento (LGPD)

#### Módulo 2 — Feed de Atividades
- Publicação de fotos (até 5 por post) com texto descritivo
- Publicação por grupo/turma ou por criança específica
- Visualização no feed por responsáveis
- Reação com coração (sem comentários na v1)
- Notificação push ao responsável quando nova publicação sobre sua criança

#### Módulo 3 — Agenda e RSVP
- Cadastro de eventos e sessões recorrentes
- Visualização semanal pelos responsáveis
- Confirmação de presença ou informação de falta
- Lembrete automático 24h antes do compromisso

#### Módulo 4 — Comunicados
- Envio de avisos institucionais para todos ou grupos específicos
- Confirmação de leitura pelo responsável
- Histórico de comunicados

#### Módulo 5 — Controle de Presença
- Registro de presença/falta por profissional ao final de cada sessão
- Visualização de histórico de frequência pelo responsável

### 9.3 O que NÃO entra no MVP

- Jornada de Evolução (Bento Grid) — entra na Versão 2
- Upload de vídeos — entra na Versão 2
- Relatórios exportáveis — entra na Versão 2
- Módulo financeiro — fora do escopo atual
- Chat bidirecional — pode ser avaliado na Versão 2

### 9.4 Estimativa de Prazo para MVP

| Fase | Atividade | Estimativa |
|---|---|---|
| Fase 1 | Wireframes e validação com a equipe Up | 2–3 semanas |
| Fase 2 | Design de interface (UI/UX) | 3–4 semanas |
| Fase 3 | Desenvolvimento backend + app | 8–12 semanas |
| Fase 4 | Testes internos (beta) | 2–3 semanas |
| Fase 5 | Publicação nas lojas + onboarding | 1–2 semanas |
| **Total estimado** | | **4–6 meses** |

---

## 10. Roadmap Futuro

### Versão 2.0 — Jornada Terapêutica (3–6 meses após MVP)

**Objetivo:** Trazer profundidade ao acompanhamento terapêutico e diferenciar o produto no mercado.

Funcionalidades:
- **Jornada de Evolução — Bento Grid Interativo:** painel visual com áreas de desenvolvimento configuráveis por profissional
- Definição de objetivos e metas por área
- Registro de conquistas com datas
- Próximos passos visíveis para o responsável
- Linguagem lúdica e acessível — sem jargão clínico
- Notificação ao responsável quando nova conquista é registrada
- Upload de vídeos de atividades (até 3 minutos)
- Relatório de frequência exportável em PDF

### Versão 3.0 — Engajamento e Personalização (6–12 meses após MVP)

Funcionalidades:
- **Portfólio da Criança:** linha do tempo visual das conquistas e registros
- **Orientações domiciliares:** profissional envia dicas de atividades para praticar em casa
- **Canal de dúvidas assíncrono:** responsáveis enviam perguntas, profissional responde no momento adequado (fora do fluxo de sessão)
- Suporte a múltiplos idiomas (espanhol, inglês) para eventual expansão
- **Notificações inteligentes:** lembretes personalizados por comportamento do usuário

### Versão 4.0 — Inteligência e Relatórios (12–24 meses)

Funcionalidades:
- Dashboard analítico para a gestão: frequência, engajamento, evolução por turma
- Relatórios automáticos de progresso por área de desenvolvimento (exportáveis para laudo)
- Integração com prontuário eletrônico externo (via API)
- **Assinatura digital de documentos** (termos de consentimento, relatórios)
- Módulo de telemedicina/tele-orientação para consultas de acompanhamento remoto

### Diferenciais Inovadores (Exploração Futura)

- **"Celebre Comigo":** notificação especial com animação quando a criança atinge uma meta importante — transforma conquista clínica em momento emocional compartilhado com a família
- **Modo Convidado Temporário:** permite que um avô ou familiar distante acesse momentos específicos do feed por tempo limitado, mediante autorização do responsável
- **IA para resumo de sessão:** transcrição e resumo automático das anotações do profissional em linguagem acessível para os pais
- **Mural de Conquistas:** espaço visual dentro do app onde as conquistas da criança ficam permanentemente celebradas — similar a um "álbum de memórias terapêuticas"

---

## 11. Conclusão

A Up Espaço Multiprofissional possui uma oportunidade concreta e estratégica de transformar sua comunicação com as famílias por meio de tecnologia. O problema identificado — fragmentação da comunicação, retrabalho da equipe e baixo engajamento dos pais — não é exclusivo desta instituição, mas afeta todo o segmento de espaços multiprofissionais no Brasil.

A solução proposta vai além de um simples app de mensagens: trata-se de uma **plataforma de vínculo entre a instituição e as famílias**, capaz de transformar cada atualização de evolução em um momento de conexão emocional entre pais e filhos, mesmo à distância.

O benchmarking confirma que nenhuma solução disponível no mercado brasileiro cobre de forma integrada todas as necessidades identificadas. Há uma janela de oportunidade real para um produto genuinamente pensado para o contexto de clínicas e espaços multiprofissionais de pequeno e médio porte.

O MVP proposto é viável em 4 a 6 meses e já entrega impacto direto na redução de retrabalho da equipe e na melhoria da experiência dos pais. As versões seguintes constroem progressivamente um diferencial competitivo robusto.

A conformidade com a LGPD, especialmente no tratamento de dados sensíveis de crianças, não é apenas uma obrigação legal — é um argumento de confiança e posicionamento de mercado que deve ser comunicado ativamente à comunidade de famílias atendidas.

**Recomendação final:** iniciar imediatamente a fase de validação do produto com a equipe e com um grupo piloto de responsáveis, antes do início do desenvolvimento, para confirmar premissas e ajustar prioridades do MVP com base em feedback real.

---

## 12. Referências

1. **IBGE — Cidades e Estados:** Dados demográficos de Faxinal do Soturno/RS. Disponível em: https://www.ibge.gov.br/cidades-e-estados/rs/faxinal-do-soturno.html

2. **ClassApp — Site oficial:** Funcionalidades e posicionamento de mercado. Disponível em: https://www.classapp.com.br

3. **ClassApp — Artigo de crescimento:** Pesquisa sobre escolas parceiras. Disponível em: https://www.classapp.com.br/artigos/crescimento-escola-classapp

4. **ODAPP — Site oficial:** Plataforma de gestão terapêutica para TEA. Disponível em: https://odapp.app.br

5. **ConnectTEA — Site oficial:** Plataforma ESDM para famílias e terapeutas. Disponível em: https://connecttea.com

6. **CollectABA — Artigo sobre acompanhamento de TEA em tempo real:** Disponível em: https://www.collectaba.com/tea-aplicativo-acompanhamento-tempo-real/

7. **Ninsaúde Clinic — Blog:** Evolução clínica do paciente e acompanhamento digital. Disponível em: https://blog.apolo.app/evolucao-clinica-do-paciente-monitorando-de-forma-eficiente/

8. **LGPD — Artigo 14:** Dados pessoais de crianças e adolescentes. Disponível em: https://lgpd-brasil.info/capitulo_02/artigo_14

9. **SERPRO — LGPD e dados sensíveis:** Orientações sobre consentimento de menores. Disponível em: https://www.serpro.gov.br/lgpd/menu/protecao-de-dados/dados-sensiveis-lgpd

10. **IBDFAM — LGPD e crianças:** Proteção de dados de menores no Brasil. Disponível em: https://ibdfam.org.br/noticias/13150

11. **Escola Comunitária de Campinas — ClassApp:** Relato de implementação e motivações (LGPD/WhatsApp). Disponível em: https://ecc.br/area-administrativa/classapp-conheca-nossa-nova-ferramenta-de-comunicacao/

12. **Espaço Ninho — Psicomotricidade Infantil:** Contextualização de serviços multiprofissionais. Disponível em: https://www.espaconinho.com.br/psicomotricidade-infantil

13. **Conecta Kids — Site oficial:** Referência de modelo integrado clínica-escola para TEA. Disponível em: https://www.conectakids.com.br

---

*Documento elaborado com base em pesquisa de fontes públicas disponíveis na internet, informações fornecidas pela instituição e análise comparativa de mercado. As informações institucionais sobre a Up Espaço Multiprofissional que não puderam ser verificadas em fontes externas foram inferidas a partir de comparação com instituições de perfil similar no Rio Grande do Sul e no Brasil.*

---

**Fim do Documento**  
Up Espaço Multiprofissional — Levantamento de Requisitos v1.0 — Junho/2026
