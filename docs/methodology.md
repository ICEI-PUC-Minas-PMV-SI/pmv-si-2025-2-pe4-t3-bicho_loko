# **METODOLOGIA**

A execução do projeto seguirá metodologia ágil, com aplicação adaptada do framework **Scrum**, permitindo entregas incrementais e acompanhamento contínuo do progresso. A função de **Scrum Master** será desempenhada por **Ana Carolina Fernandes de Assis**, responsável por organizar as tarefas, acompanhar prazos e promover a integração entre a equipe acadêmica e a ONG Bicho Loko.

As principais atividades metodológicas incluem:

- **Reuniões de levantamento de requisitos**: encontros online com a ONG para identificar necessidades e validar as informações a serem contempladas no sistema.

- **Oficinas de capacitação interna**: nivelamento dos integrantes quanto ao uso de **Google Forms**, **Google Sheets** e **Looker Studio**, garantindo a qualidade da entrega.

- **Construção da base de dados**: organização de uma planilha única no Google Sheets, estruturada em abas temáticas (animais, adotantes, voluntários, castrações, parceiros, campanhas e interessados em adoção).

- **Criação de formulário digital**: desenvolvimento de um formulário online para pessoas interessadas em adotar animais da ONG.

- **Desenvolvimento do dashboard**: configuração do **Looker Studio**, conectado à planilha, com visualizações dinâmicas das métricas selecionadas em conjunto com a ONG.

- **Validação incremental**: cada entrega parcial (planilha organizada, formulário ativo, dashboard inicial) será apresentada à ONG, coletando feedbacks e ajustes.

Essa abordagem permite uma implementação rápida, de baixo custo e com curva de aprendizado acessível, sem comprometer a qualidade do sistema de apoio à gestão da ONG.

##

## **ARQUITETURA**

A arquitetura proposta para o sistema é **baseada em ferramentas em nuvem gratuitas ou de baixo custo**, garantindo viabilidade técnica e sustentabilidade para a ONG. A estrutura é composta pelos seguintes componentes:

1. **Camada de coleta de dados**

   - **Google Forms** integrados à planilha, destinados a diferentes finalidades:

     - Prospecção de adotantes, com informações como dados pessoais, tipo de moradia, outros animais no domicílio e canal de contato.

     - Cadastro de voluntários interessados em colaborar com a ONG.

   - Os formulários alimentam automaticamente abas específicas no Google Sheets, reduzindo erros manuais e centralizando registros.

2. **Camada de armazenamento e organização**

   - **Google Sheets** como repositório central de dados.

   - Estrutura organizada em abas temáticas:

     - **Animais**: dados de identificação, saúde, histórico de resgate.

     - **Adotantes**: informações de contato, termos de responsabilidade, status da adoção.

     - **Interessados**: dados provenientes do formulário de prospecção de adotantes, incluindo aprovação ou recusa.

     - **Voluntários**: perfil e disponibilidade.

     - **Campanhas**: registro de eventos, arrecadações, dados financeiros.

     - **Parcerias:** informações de contato, tipo de parceria, disponibilidades.

3. **Camada de visualização e análise**

   - **Looker Studio** como ferramenta de BI, conectado diretamente ao Google Sheets.

   - Criação de dashboards interativos com indicadores-chave definidos nos RFs:

     - **Eficiência de adoção por canal** (Instagram, feiras, indicações).

     - **Mapa de custos por etapa** (castração, vacinas, tratamentos, transporte).

     - **Taxa de devolução por perfil do adotante** (tipo de moradia, região, faixa etária).

   - Painéis configurados para atualização automática, sempre que novos dados forem inseridos na planilha.

Essa arquitetura, por utilizar ferramentas de fácil acesso e hospedagem em nuvem, dispensa investimentos em servidores dedicados e permite que a própria ONG gerencie seus dados após a entrega, garantindo **escalabilidade** e **autonomia**.

![][image1]

**Figura 1 – Arquitetura proposta do sistema da ONG Bicho Loko**

Fonte: elaborado pelos autores (2025).

## **ESTRUTURA PARA A REALIZAÇÃO DO PROJETO**

A estrutura necessária para a execução do projeto foi definida considerando-se a realidade da ONG Bicho Loko e o escopo estabelecido, priorizando ferramentas de fácil acesso, baixo custo e hospedagem em nuvem.

### **Recursos materiais e tecnológicos**

- **Computadores pessoais** dos integrantes do projeto, utilizados para o desenvolvimento e configuração das ferramentas.

- **Conexão com a internet**, requisito essencial para utilização dos serviços em nuvem.

- **Aplicativos do Google**:

  - **Google Forms**, para coleta de dados de adotantes e voluntários.

  - **Google Sheets**: organização centralizada das informações em abas temáticas (Animais, Adotantes, Interessados, Voluntários, Campanhas e Parcerias).

  - **Google Drive**, para armazenamento e compartilhamento dos arquivos gerados e salvos.

- **Looker Studio**, ferramenta de Business Intelligence que possibilita a construção de dashboards interativos e de fácil interpretação.

### **Recursos humanos**

- **Equipe discente**, composta por alunos do curso de Sistemas de Informação, responsáveis pela análise, organização e implementação da solução.

- **Scrum Master designado pelo grupo**, encarregado da organização das atividades, do monitoramento de prazos e da facilitação da comunicação entre equipe e ONG.

- **Representante da ONG Bicho Loko**, responsável pela validação dos dados fornecidos, acompanhamento das entregas e posterior gestão da solução.

### **Justificativa da estrutura escolhida**

A opção pelo uso de ferramentas baseadas em nuvem e de fácil acesso é coerente com as necessidades e limitações da ONG, que não dispõe de infraestrutura própria de TI. Dessa forma, garante-se:

- **Baixo custo operacional**, sem necessidade de aquisição de servidores ou licenças de software.

- **Escalabilidade**, permitindo a expansão gradual do sistema com novos indicadores e formulários.

- **Autonomia da ONG**, que poderá gerenciar e atualizar seus próprios dados e dashboards após a entrega, sem depender exclusivamente da equipe acadêmica.

Assim, a estrutura definida viabiliza a implementação do projeto de forma ágil, sustentável e com impacto social imediato.
