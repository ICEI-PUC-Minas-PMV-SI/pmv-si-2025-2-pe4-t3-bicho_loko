[Voltar](../README.md)

# **METODOLOGIA**

A execução do projeto seguirá metodologia ágil, com aplicação adaptada do framework **Scrum**, permitindo entregas incrementais e acompanhamento contínuo do progresso. A função de **Scrum Master** será desempenhada por **Ana Carolina Fernandes de Assis**, responsável por organizar as tarefas, acompanhar prazos e promover a integração entre a equipe acadêmica e a ONG Bicho Loko.

As principais atividades metodológicas incluem:

- **Reuniões de levantamento de requisitos**: encontros online com a ONG para identificar necessidades e validar as informações a serem contempladas no sistema.

- **Oficinas de capacitação interna**: nivelamento dos integrantes quanto ao uso de **AppScript**, **AppSheets**, **Looker Studio** e **Google Sites**, garantindo a qualidade da entrega.

- **Construção da base de dados**: estruturação de um banco de dados integrado no **AppSheet**, organizado em tabelas temáticas que abrangem as informações sobre **animais, adotantes, voluntários, castrações, parceiros, doadores, adoções, campanhas, despesas e interessados em adoção**. A modelagem foi planejada para garantir integridade referencial, facilidade de atualização e integração com as demais camadas do sistema.

- **Criação de formulário digital**: desenvolvimento de um **formulário personalizado** por meio do **Google AppScript**, incorporado ao portal institucional e ao aplicativo interno. Esse formulário possibilita o registro de novos adotantes e o envio de informações diretamente para o banco de dados da aplicação, assegurando a coleta estruturada e automatizada dos dados.

- **Desenvolvimento do dashboard**: implementação de painéis interativos no **Looker Studio**, que consolidam os indicadores operacionais e estratégicos definidos em conjunto com a ONG. Os dashboards oferecem visualizações dinâmicas e são incorporados ao Google Sites, facilitando o acompanhamento das ações e o processo de tomada de decisão.

- **Validação incremental**: cada entrega parcial (planilha organizada, formulário ativo, dashboard inicial) será apresentada à ONG, coletando feedbacks e ajustes.

Essa abordagem permite uma implementação rápida, de baixo custo e com curva de aprendizado acessível, sem comprometer a qualidade do sistema de apoio à gestão da ONG.

## **ARQUITETURA**

Este item descreve a arquitetura de software projetada para a Organização Não Governamental (ONG) Bicho Loko, desenvolvida exclusivamente com o uso das ferramentas Google AppSheet, Looker Studio, Google AppScript e Google Sites. A solução foi concebida para operação em ambiente de nuvem, com baixo custo de implantação, facilidade de manutenção e aderência estrita aos requisitos funcionais e não funcionais estabelecidos pelo projeto.

1. **Camada de Aplicação (Frontend)**:

   **Google Sites, Looker Studio e AppSheet**

   A camada de aplicação compreende dois componentes distintos, voltados a públicos diferentes:

   - **Google Sites**: atua como o frontend público, servindo como portal institucional responsivo da ONG. Destina-se à divulgação de campanhas, histórias de adoção, informações institucionais, acesso a formulários e aplicações internas e visualização dos dashboards de BI incorporados criados a partir do Looker Studio. O portal possui páginas configuráveis, com áreas públicas e áreas restritas, de acordo com a política de acesso definida.

   - **AppSheet**: constitui o frontend e backend interno do sistema, utilizado exclusivamente pela equipe da ONG. Nessa plataforma são realizadas as operações internas, como cadastro, acompanhamento de animais, controle de adoções e gerenciamento de voluntários. O AppSheet oferece interface responsiva e integração direta com as tabelas de dados hospedadas em nuvem.
  
   - **Looker Studio**: atua como a camada de visualização analítica, transformando os dados operacionais em painéis gerenciais e estratégicos. Permite a criação de gráficos interativos, filtros dinâmicos e relatórios personalizados que são embarcados no portal institucional (Google Sites), democratizando o acesso à informação e embasando a tomada de decisão da gestão.

2. **Camada de Coleta de Dados**

   **Formulário Personalizado (AppScript)**

   - A camada de coleta de dados é responsável por capturar, registrar e integrar informações estruturadas ao sistema. O formulário, desenvolvido por meio do **Google AppScript** oferece integração direta com as planilhas do **AppSheet**.
   - As respostas são automaticamente armazenadas nas tabelas da aplicação, garantindo a centralização e integridade dos dados.
   - Além da coleta de novas informações, esta camada também contempla a **digitalização e integração de dados legados**, anteriormente registrados em formulários físicos. Esse processo faz parte do **procedimento de Extração, Transformação e Carga (ETL)**, assegurando a consolidação dos registros históricos no ambiente digital.

3. **Camada de Lógica de Negócio (Backend)**

   **AppSheet**

   - Implementação das regras de negócio, views, formulários de entrada, validações e fluxos previstos nos RFs;

   - Gerenciamento de permissões e políticas de acesso (ex.: Administrador, Voluntário com permissão de edição e Leitura apenas), em conformidade com os requisitos de segurança e privacidade;

   - Execução apenas das ações autorizadas, sem inclusão de automações, notificações ou bots não previstos nos RFs.

4. **Camada de Dados**

   **AppSheets Database**

   - Estrutura de dados organizada por entidades: Usuários, Animais, Adotantes, Voluntários, Campanhas, Parceiros, Adoções, Despesas, Atendimentos Clínicos, Resgates, Pós-adoções, Doadores, Candidatos, Hospedagens e Doações;

   - Formas de alimentação dos dados:

     - Entradas originadas por formulários Google Forms integrados;

     - Inserção manual direta no AppSheet, realizada por colaboradores da ONG a partir de registros físicos ou outros documentos existentes;

     - Inserção em tempo real pelo aplicativo AppSheet em campo (por exemplo, durante resgates).

     - Regras de validação e integridade implementadas no AppSheet para assegurar consistência dos registros e conformidade com os RFs.

5. **Camada de Business Intelligence (BI)**

   **Dashboards Looker Studio**

   - Painéis operacionais e relatórios interativos desenvolvidos no Looker Studio e incorporados ao Google Sites para consulta e acompanhamento dos indicadores previstos nos RFs.

   - Visualizações e filtros configurados conforme as necessidades operacionais da ONG, consumindo os dados estruturados pela camada de dados e oferecendo visões estratégicas sobre animais, adoções e despesas;

6. **Infraestrutura em Nuvem**

   **Hospedagem Google (serverless)**

   - Todos os componentes (Google Sites, Google Forms e AppSheet) operam em infraestrutura de nuvem, sem necessidade de servidores dedicados;

   - Solução dimensionada para o porte da ONG, com custos alinhados ao uso e às políticas de planos das ferramentas.

7. **Considerações Finais**

Todas as funcionalidades implementadas corresponderão estritamente aos requisitos funcionais e não funcionais fornecidos. Não serão incorporadas automações, notificações ou bots que não constem nos requisitos iniciais.

A arquitetura foi concebida para priorizar a autonomia operacional da ONG, o baixo custo de implantação, bem como a facilidade de manutenção e evolução.

8. **Figura da Arquitetura**

A Figura 1 apresenta o diagrama esquemático da arquitetura da solução, evidenciando o fluxo de informações entre as camadas de coleta, armazenamento, processamento operacional e visualização de dados.

![Diagrama de Arquitetura da Solução](./img/arquitetura_bicho_loko.png)

Fonte: Elaborada pelos autores (2025).


## **ESTRUTURA PARA A REALIZAÇÃO DO PROJETO**

A estrutura necessária para a execução do projeto foi definida considerando a realidade da ONG Bicho Loko e o escopo estabelecido, priorizando o uso de ferramentas de fácil acesso, baixo custo e hospedagem em nuvem. Essa configuração visa garantir a viabilidade técnica, a sustentabilidade operacional e a autonomia da instituição após a implantação da solução.

### **Estrutura Tecnológica da ONG Bicho Loko**

Atualmente, a ONG Bicho Loko realiza a gestão de adoções de forma manual, utilizando formulários impressos para registrar informações de adotantes e animais. Esses documentos são armazenados em armários cedidos por uma clínica veterinária parceira, o que limita o acesso e a atualização dos dados, além de aumentar o risco de extravio ou deterioração das informações.

A divulgação das campanhas e dos animais disponíveis para adoção é feita exclusivamente pelas redes sociais — principalmente **Instagram** e **Facebook** —, sem a existência de um **portal institucional** que concentre informações e facilite o relacionamento com o público.

Com o objetivo de **modernizar e automatizar os processos**, foi proposta uma arquitetura tecnológica integrada baseada em **Google Sites, AppScript, Looker Studio e AppSheet**. O **Google Sites** funcionará como o **portal institucional** da ONG, centralizando a divulgação de campanhas e o acesso a formulários digitais personalizados. O **AppScript** será utilizado para automatizar os formulários e integrar diretamente os dados ao banco em nuvem. Já o **AppSheet** atuará como **plataforma central de gestão**, permitindo o registro, acompanhamento e análise das informações relativas a adoções, doações, voluntários, parceiros e campanhas em um único ambiente.

Para a inteligência de dados, a solução utiliza o **Looker Studio**, que permite a geração de dashboards interativos integrados ao Google Sites. Esses painéis fornecerão uma visão consolidada das atividades da ONG, divididos em três grupos principais de indicadores:

**1. Indicadores relacionados aos animais:**

- Visão geral dos animais: quantidade total geral, total de cães, total de gatos, total de fêmeas e total de machos;

- Perfil dos animais por espécie: quantidade de fêmeas e machos entre cães e gatos;

- Perfil dos animais por porte: quantidade de fêmeas e machos dentre os portes mini, pequeno, médio e grande;

- Perfil dos animais por status: quantidade de fêmeas e machos dentre os status óbito, em tratamento, disponível e adotado.
  
**2. Indicadores relacionados às adoções:**

- Visão geral das adoções: total de adoções no último ano e no último mês, total de adoções do mês atual;

- Visão geral das devoluções: total de devoluções do último ano, do último mês e do mês atual;

- Quantidade de adoções por espécie: segmentação entre cães e gatos;

- Porcentagem de adoções por sexo: segmentação entre fêmeas e machos;

- Quantidade de adoções por porte: segmentação entre portes mini, pequeno, médio e grande;

- Taxas e perfis: taxa anual de adoções, taxa anual de devoluções, perfil etário dos adotantes e perfil etário dos adotantes que devolveram animais;

- Origem: quantidade de adoções por canal de origem (feiras, Instagram, indicação, site).

**3. Indicadores relacionados às despesas:**

- Custos gerais: total gasto em determinado período e média de despesas por mês;

- Análise de eficiência: custo médio por animal e custo médio por espécie;

- Extremos: despesa de maior custo e despesa de menor custo;

- Detalhamento: percentual de distribuição por tipo de despesa e valor em real de custos por tipo de despesa.

Esses painéis permitirão à ONG **monitorar suas atividades em tempo real**, aprimorar o planejamento e direcionar recursos de forma mais eficiente, ampliando sua capacidade de gestão e impacto social.

### **Recursos materiais e tecnológicos**

- **Computadores pessoais** dos integrantes do projeto, utilizados para o desenvolvimento e configuração das ferramentas.

- **Dispositivos móveis pessoais**, empregados para comunicação com a equipe e representantes da ONG via **WhatsApp**.

- **Conexão com a internet**, requisito essencial para utilização dos serviços em nuvem.

- **Aplicativos do Google**:

  - **AppScript**: coleta e automação de dados de adotantes e voluntários;

  - **AppSheet**: organização centralizada das informações em tabelas temáticas (Animais, Adotantes, Interessados, Voluntários, Campanhas e Parcerias) e gestão operacional;
 
  - **Looker Studio**: criação e visualização de dashboards de indicadores e relatórios de BI;

  - **Google Workspace**: armazenamento e compartilhamento dos arquivos do projeto;

  - **Google Sites**: criação do portal institucional responsivo da ONG e hospedagem dos dashboards incorporados.

### **Recursos humanos**

- **Equipe discente**, composta por alunos do curso de Sistemas de Informação, responsáveis pela análise, organização e implementação da solução.

- **Scrum Master designado pelo grupo**, encarregado da organização das atividades, do monitoramento de prazos e da facilitação da comunicação entre equipe e ONG.

- **Representante da ONG Bicho Loko**, responsável pela validação dos dados fornecidos, acompanhamento das entregas e posterior gestão da solução.

### **Justificativa da estrutura escolhida**

A adoção de ferramentas baseadas em nuvem e de fácil utilização está alinhada às necessidades e limitações da ONG, que não dispõe de infraestrutura própria de tecnologia da informação. Essa configuração garante:

- **Baixo custo operacional**, eliminando a necessidade de servidores ou licenças pagas;

- **Escalabilidade**, permitindo a expansão gradual com novos formulários e indicadores;

- **Autonomia da ONG**, possibilitando que a ONG gerencie e atualize seus próprios dados e painéis após a conclusão do projeto.

Assim, a estrutura definida assegurará uma implementação ágil, sustentável e de impacto social imediato, fortalecendo a transformação digital da ONG Bicho Loko.
