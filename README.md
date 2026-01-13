
# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

**Data:** 12 de janeiro de 2026
**Empresa:** Abstergo Industries (Setor Farmacêutico)
**Responsável:** Valdeci Boldan

## 1. Introdução

Este relatório apresenta a proposta de implementação estratégica de serviços da Amazon Web Services (AWS) na **Abstergo Industries**. O foco central deste projeto é a **otimização financeira e operacional**, selecionando serviços que permitem reduzir custos imediatos com infraestrutura, sem comprometer a segurança e a alta disponibilidade exigidas pelo setor farmacêutico.

## 2. Descrição do Projeto

Este relatório detalha a proposta de otimização de infraestrutura em nuvem para a Abstergo Industries, focando em uma redução imediata de custos de 25% a 35% já no primeiro trimestre. Através da implementação estratégica de Amazon S3 Intelligent-Tiering para armazenamento inteligente, AWS Fargate para computação eficiente e Amazon EC2 Auto Scaling/ELB para escalabilidade sob demanda, a Abstergo Industries não apenas alcançará significativa economia financeira, mas também garantirá maior agilidade, segurança e resiliência em suas operações críticas de pesquisa e desenvolvimento farmacêutico.

A estratégia de otimização foi dividida em três pilares fundamentais: armazenamento inteligente, computação eficiente para processamento de dados e escalabilidade automatizada.

### Etapa 1: Otimização de Armazenamento de Dados de Pesquisa

* **Nome da ferramenta:** Amazon S3 com **S3 Intelligent-Tiering**.
* **Foco da ferramenta:** Redução de custos de armazenamento de objetos.
* **Descrição de caso de uso:** A Abstergo armazena terabytes de dados brutos de pesquisas clínicas e sequenciamentos genéticos. Como o padrão de acesso a esses dados é imprevisível, o *Intelligent-Tiering* moverá automaticamente os arquivos não utilizados para camadas de custo menor.
* **Impacto:** Economia de até 40% em custos de armazenamento sem necessidade de intervenção manual da equipe de TI.



### Etapa 2: Processamento de Dados Laboratoriais sem Servidor

* **Nome da ferramenta:** **AWS Fargate**.
* **Foco da ferramenta:** Computação Serverless para containers.
* **Descrição de caso de uso:** Para rodar aplicações que processam resultados de testes laboratoriais, a empresa não precisará mais manter instâncias EC2 ligadas 24/7. O Fargate executará os containers apenas durante o processamento, cobrando apenas pelos segundos de execução.
* **Impacto:** Eliminação do custo de servidores ociosos e redução da carga de gerenciamento de patches de segurança.



### Etapa 3: Gestão de Tráfego e Disponibilidade de Aplicações Internas

* **Nome da ferramenta:** **Amazon EC2 Auto Scaling** integrado ao **Elastic Load Balancing (ELB)**.
* **Foco da ferramenta:** Escalabilidade horizontal e eficiência de recursos.
* **Descrição de caso de uso:** O portal de acesso dos pesquisadores sofre picos de acesso durante o horário comercial. O Auto Scaling garantirá que o número de instâncias EC2 aumente apenas quando necessário e reduza drasticamente durante a noite e fins de semana.
* **Impacto:** Garantia de performance para os colaboradores e redução de custos operacionais em períodos de baixa demanda.



---

## 3. Conclusão

A implementação das ferramentas AWS na **Abstergo Industries** tem como benefício esperado uma redução direta nos gastos com infraestrutura de nuvem, estimada entre **25% e 35% no primeiro trimestre**. Além da economia financeira, as ferramentas promovem maior agilidade no processamento de dados científicos e garantem a segurança e integridade das informações, aumentando a eficácia competitiva da empresa no mercado farmacêutico.

Anexo 1: Estimativa de Otimização de Custos (Mensal)

Esta tabela compara o cenário de infraestrutura tradicional (sem otimização) com o cenário proposto utilizando serviços gerenciados da AWS.

### 📊 Anexo 1: Estimativa de Otimização de Custos (Mensal)

Esta tabela apresenta o comparativo financeiro entre a infraestrutura tradicional da Abstergo Industries e a nova arquitetura proposta em AWS.

| Recurso / Serviço | Custo Cenário Atual (Legacy) | Custo Proposto (AWS Optimized) | Economia Estimada | Justificativa Técnica |
| :--- | :--- | :--- | :--- | :--- |
| **Armazenamento de Dados** | $2.500,00 |$ 1.625,00 | **35%** | S3 Intelligent-Tiering para gestão de dados frios. |
| **Computação (Processamento)** | $1.200,00 |$ 480,00 | **60%** | AWS Fargate eliminando cobrança por ociosidade. |
| **Servidores Web (Portal)** | $800,00 |$ 520,00 | **35%** | Auto Scaling ajustando instâncias conforme demanda. |
| **TOTAL** | **$ 4.500,00** | **$ 2.625,00** | **41,6%** | **Economia mensal total de $ 1.875,00.** |

> [!TIP]
> **Nota de ROI:** O retorno sobre o investimento (ROI) desta implementação é estimado em apenas 2 meses, considerando os custos de migração.

Recomenda-se a continuidade deste projeto com a implementação do **AWS Budgets** para monitoramento em tempo real dos limites de gastos e a exploração de **Instâncias Spot** para processamentos em lote não críticos.

## 4. Anexos

1. **Planilha de Estimativa de Custos (AWS Pricing Calculator):** Comparativo entre o modelo atual e o modelo proposto.
2. **Arquitetura de Referência:** Diagramas detalhando a conexão entre VPC e os novos serviços.
3. **Manual de Boas Práticas de Segurança (IAM):** Definição de políticas de acesso para os colaboradores.

---

**Assinatura do Responsável pelo Projeto:**

*Valdeci Boldan*
