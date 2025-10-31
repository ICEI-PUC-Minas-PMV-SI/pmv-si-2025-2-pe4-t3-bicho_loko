[Voltar](../README.md)

# Diagnóstico da situação problema

O abandono de animais é um problema de grande magnitude no Brasil. Estimativas da Organização Mundial da Saúde (OMS) indicam que existem cerca de 30 milhões de animais abandonados, sendo aproximadamente 20 milhões de cães e 10 milhões de gatos (CRMV-PB) [1]. Em grandes capitais, como Belo Horizonte, estudos locais indicam que milhares de cães e gatos vivem em situação de rua, agravando problemas de saúde pública e maus-tratos.
Segundo  informações do site da Câmara Municipal de Belo Horizonte [2], o abandono de animais é crime desde 1998, conforme Lei Federal 9.605. O último levantamento realizado pela Prefeitura de Belo Horizonte  no ano de 2022, declarou a existência de, aproximadamente, 48 mil animais de ruas na capital, em situação de abandono. A partir desse dado, o vereador Lucas Ganem apresentou o Projeto de Lei 75/2025, que prevê a realização periódica de um censo dos animais domésticos que vivem em Belo Horizonte. Conforme trecho do Projeto de Lei, art. 3º, “Além de produzir informações sobre a quantidade de cães e gatos existentes no Município de Belo Horizonte, o Censo Municipal de Animais Domésticos deverá discriminar os animais entre machos e fêmeas; tutelados e em situação de abandono; vacinados e não vacinados; castrados e não castrados; entre outros critérios que se revelem metodologicamente relevantes para orientar a formulação de políticas públicas.”

A ONG Bicho Loko, fundada em 2015, nasceu do esforço coletivo de protetores independentes que buscavam estruturar suas ações em defesa dos animais. Seu trabalho tem como eixos principais a castração, a adoção responsável e a conscientização social. Entretanto, a instituição enfrenta grandes dificuldades em gerir suas atividades, em especial pela ausência de ferramentas digitais de organização e centralização de dados. Além disso, a ausência de dados organizados pela ONG compromete o mapeamento do impacto real de suas ações, limitando o alcance de novas parcerias e investimentos. 

Atualmente, os registros de animais, adotantes, voluntários e termos de responsabilidade são realizados de forma manual e física, dificultando a recuperação rápida das informações e atrasando processos decisivos [3].  Com a organização dessas informações de maneira estruturada, será possível gerar indicadores e relatórios que evidenciem as ações realizadas pela ONG e os resultados alcançados. Esses dados serão fundamentais para apresentar de forma transparente o trabalho desenvolvido, contribuindo para sensibilizar e atrair novos parceiros, voluntários e investidores.

## **RELAÇÃO DO PROJETO COM OS ODS**

O presente projeto está diretamente vinculado ao **ODS 15 – Vida Terrestre**, que busca proteger, recuperar e promover o uso sustentável dos ecossistemas terrestres, combater a desertificação, deter e reverter a degradação da terra e frear a perda da biodiversidade. Ao proporcionar maior visibilidade ao trabalho da ONG Bicho Loko e estruturar sua gestão de dados por meio de planilhas organizadas, formulários digitais e dashboards interativos, a iniciativa contribui para a redução do abandono de animais domésticos, fomenta adoções responsáveis e fortalece parcerias com clínicas veterinárias e apoiadores.

De forma indireta, também se observa a relação com o **ODS 11 – Cidades e Comunidades Sustentáveis**, uma vez que o controle populacional de animais em situação de rua impacta positivamente a qualidade de vida urbana, reduz riscos sanitários e favorece uma convivência harmoniosa entre seres humanos e animais nos espaços urbanos.

Além disso, há correspondência com o ** 3 – Saúde e Bem-Estar**, considerando que a atuação da instituição contribui indiretamente para o controle de zoonoses e para a promoção da saúde pública. O acolhimento e a destinação responsável de animais em situação de abandono reduzem potenciais riscos epidemiológicos e fortalecem a proteção do bem-estar coletivo, abrangendo tanto a população humana quanto os próprios animais.

Assim, a proposta evidencia um alinhamento transversal a diferentes Objetivos de Desenvolvimento Sustentável, reforçando o papel da extensão universitária como instrumento de transformação social e promoção do bem-estar socioambiental.

**Quadro 1 – Relação do projeto com os Objetivos de Desenvolvimento Sustentável (ODS)**

| ODS                                             | Objetivo                                                                                                                                                                                                                    | Relação com o Projeto                                                                                                                                                              |
| ----------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **ODS 3 – Saúde e Bem-Estar**                   | Assegurar uma vida saudável e promover o bem-estar para todos, em todas as idades.                                                                                                                                          | Contribui para o controle de zoonoses e para a redução de riscos epidemiológicos, favorecendo a saúde pública e o bem-estar coletivo.                                              |
| **ODS 11 – Cidades e Comunidades Sustentáveis** | Tornar as cidades e os assentamentos humanos inclusivos, seguros, resilientes e sustentáveis.                                                                                                                               | O controle populacional de animais em situação de rua melhora a qualidade de vida urbana, reduz riscos sanitários e promove convivência harmoniosa entre pessoas e animais.        |
| **ODS 15 – Vida Terrestre**                     | Proteger, recuperar e promover o uso sustentável dos ecossistemas terrestres, gerir de forma sustentável as florestas, combater a desertificação, deter e reverter a degradação da terra e deter a perda da biodiversidade. | O projeto apoia a redução do abandono de animais domésticos, fomenta adoções responsáveis e fortalece parcerias, contribuindo para a preservação do equilíbrio ambiental e social. |

**Fonte:** elaborado pelos autores (2025).

## **LEVANTAMENTO DE REQUISITOS**

**Requisitos Funcionais:**

|   ID   |             Seção              | Descrição do Requisito                                                                                                                       | Prioridade  |
| :----: | :----------------------------: | -------------------------------------------------------------------------------------------------------------------------------------------- | :---------: |
| RF-01  |         Gerenciamentos         | O sistema deve permitir cadastrar, editar, visualizar e inativar registros de animais.                                                       | Obrigatório |
| RF-02  |         Gerenciamentos         | O sistema deve permitir cadastrar, editar, visualizar, e inativar registros de adotantes.                                                    | Obrigatório |
| RF-03  |         Gerenciamentos         | O sistema deve permitir cadastrar, editar, visualizar e inativar registros de doadores.                                                      | Obrigatório |
| RF-04  |         Gerenciamentos         | O sistema deve permitir cadastrar, editar, visualizar e inativar registros de parceiros.                                                     | Obrigatório |
| RF-05  |         Gerenciamentos         | O sistema deve permitir cadastrar, editar, consultar e inativar registros de voluntários.                                                    | Obrigatório |
| RF-06  |         Gerenciamentos         | O sistema deve permitir cadastrar, editar, consultar e inativar registros de interessados em adoção.                                         | Obrigatório |
| RF-07  |     Processos e Operações      | O sistema deve permitir registrar, consultar e atualizar informações de saúde dos animais.                                                   | Obrigatório |
| RF-08  |     Processos e Operações      | O sistema deve permitir registrar, consultar e atualizar processos de adoção.                                                                | Obrigatório |
| RF-09  |     Processos e Operações      | O sistema deve permitir registrar, consultar e atualizar doações (financeiras e em itens).                                                   | Obrigatório |
| RF-010 |     Processos e Operações      | O sistema deve permitir registrar, consultar e atualizar despesas.                                                                           | Obrigatório |
| RF-011 |     Processos e Operações      | O sistema deve permitir registrar, editar, consultar e inativar campanhas (eventos/ações).                                                   | Obrigatório |
| RF-012 | Regras específicas de processo | O sistema deve permitir associar um processo de adoção a um adotante e a um animal.                                                          | Obrigatório |
| RF-013 | Regras específicas de processo | O sistema deve permitir anexar arquivos digitais a registros do sistema, quando aplicável                                                    | Obrigatório |
| RF-014 | Regras específicas de processo | O sistema deve, ao identificar um interessado com status aprovado, criar automaticamente um registro correspondente em Adotantes.            |  Desejável  |
| RF-015 | Regras específicas de processo | O sistema deve registrar no interessado convertido o identificador do adotante criado.                                                       | Obrigatório |
| RF-016 | Regras específicas de processo | O sistema deve impedir duplicidade na criação de adotantes quando já existir registro com identificadores únicos definidos.                  | Obrigatório |
| RF-017 |   Segurança e Administração    | O sistema deve permitir ao administrador configurar perfis diferenciados de acesso (edição/visualização)                                     | Obrigatório |
| RF-018 |    Relatórios e Integrações    | O sistema deve disponibilizar dashboards com indicadores de desempenho operacional e estratégico.                                            | Obrigatório |
| RF-019 |    Relatórios e Integrações    | O sistema deve integrar um formulário online para registro de interessados em adoção.                                                        |  Desejável  |
| RF-020 |    Relatórios e Integrações    | O sistema deve armazenar automaticamente as respostas do formulário em uma aba dedicada da planilha do Google Sheets, para posterior análise |  Desejável  |

**Requisitos Não Funcionais:**

|   ID    | Descrição do Requisito                                                                               | Prioridade  |
| :-----: | ---------------------------------------------------------------------------------------------------- | :---------: |
| RNF-001 | A planilha e o painel de BI devem ser intuitivos e fáceis de usar (usabilidade) para os voluntários. | Obrigatório |
| RNF-002 | A solução deve ser implementada usando apenas ferramentas gratuitas.                                 | Obrigatório |
| RNF-003 | A planilha deve ser configurada com diferentes perfis de acesso, permitindo edição e visualização.   | Obrigatório |
| RNF-004 | A planilha deve ter um procedimento de backup mensal automático.                                     | Obrigatório |
