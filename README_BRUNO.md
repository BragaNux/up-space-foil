# 💰 Plano de Atividades: Bruno (Orçamentos, Custos & Editais)

Olá, Bruno! Como **Diretor Financeiro (CFO)** da nossa agência no projeto **UP Espaço**, seu foco é justificar financeiramente o valor do projeto, os custos da empresa e apresentar as formas de financiar o projeto em um cenário real (editais e linhas de fomento).

Abaixo estão os dados financeiros prontos para você apresentar:

---

## 📊 1. Orçamento de Desenvolvimento do Projeto (Custo Real)

Caso este aplicativo fosse desenvolvido comercialmente para a clínica UP Espaço, o orçamento seria calculado com base em **320 horas de engenharia** de software e design, estimadas a um valor médio de **R$ 80,00/hora**:

| Fase | Escopo | Horas Estimadas | Custo Total |
| :--- | :--- | :---: | :---: |
| **UX/UI Design** | Prototipagem de alta fidelidade no Figma, definição de fluxos e branding | 60h | R$ 4.800,00 |
| **Frontend Dev** | Codificação da interface responsiva (React, Tailwind, Vite) e simulador | 100h | R$ 8.000,00 |
| **Backend Dev** | Estruturação de endpoints, lógica do CRUD, e rotas RESTful | 80h | R$ 6.400,00 |
| **Banco de Dados** | Modelagem física relacional, persistência e conexões SQL Postgres | 30h | R$ 2.400,00 |
| **DevOps & QA** | Configuração do Docker Compose, Prometheus, Grafana e testes | 50h | R$ 4.000,00 |
| **Total do Projeto** | **Desenvolvimento Completo Prontuário + Comunicação** | **320h** | **R$ 25.600,00** |

---

## 🌐 2. Orçamento de Manutenção da Aplicação (Mensal)

Custo fixo estimado para manter a aplicação hospedada em ambiente de nuvem estável e ferramentas de gestão:

* **Servidor e Banco de Dados (AWS RDS + EC2)**: R$ 350,00 / mês (postgres em container + host da build estática).
* **Armazenamento de Imagens e Histórico (AWS S3)**: R$ 50,00 / mês (fotos das atividades dos alunos).
* **Monitoramento & Observabilidade (Grafana Cloud)**: Grátis no plano básico (Prometheus raspando dados do backend).
* **Licenças de Software de Gestão**:
  * *Slack Pro (5 membros)*: R$ 120,00 / mês.
  * *Jira Cloud & GitHub Team*: R$ 80,00 / mês.
* **Custo Fixo de Manutenção do Sistema**: **R$ 600,00 / mês**.

---

## 🏢 3. Orçamento de Funcionamento da Equipe (Mão de Obra Mensal)

Custo de operação de pessoal para manter a equipe de 5 pessoas funcionando para o projeto:

* **Product Owner / Project Manager (Braga)**: R$ 4.500,00 / mês
* **Software Engineers (Damacena)**: R$ 8.000,00 / mês (R$ 4.000,00 cada)
* **UX/UI Designer & BA (Roberto e Nicolas)**: R$ 7.000,00 / mês (R$ 3.500,00 cada)
* **Encargos e Infraestrutura de Sede (Coworking)**: R$ 1.500,00 / mês
* **Custo Total Operacional da Agência**: **R$ 21.000,00 / mês**.

---

## 🏦 4. Como Financiar o Projeto (Linhas de Crédito e Editais no Brasil)

Como o projeto é realizado no formato *pro bono* para uma entidade sem fins lucrativos ou de recursos escassos, a captação de recursos pode ser feita por meio de editais e fomento à inovação de impacto social no Brasil:

1. **PIPE FAPESP / FINEP (Pequena Empresa Inovadora)**:
   * Linha de financiamento voltada ao desenvolvimento de protótipos e softwares inovadores na área de saúde e educação infantil. Permite captar subsídios de até R$ 200.000,00 (Fase 1) para cobrir a mão de obra da equipe.
2. **Editais de Impacto Social de Grandes Bancos (Itaú Social / Fundação Bradesco)**:
   * Editais anuais voltados ao desenvolvimento comunitário e apoio infantil. Financiam a compra de equipamentos e horas de desenvolvimento de startups que criem soluções para ONGs ou clínicas parceiras de reabilitação.
3. **BNDES Fundo Tecnológico (FUNTEC)**:
   * Linha de crédito subsidiada ou não reembolsável para projetos que apliquem tecnologia para resolver problemas de saúde pública e integração social (como no caso do tratamento de autismo e atrasos globais de desenvolvimento pelo SUS).
4. **Leis de Incentivo Fiscal (Pronas/PCD)**:
   * O Programa Nacional de Apoio à Atenção da Saúde da Pessoa com Deficiência permite que empresas direcionem parte do seu Imposto de Renda devido para projetos aprovados nessa área, cobrindo os custos de licenciamento e desenvolvimento de software do UP Espaço.
