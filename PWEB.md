FACULDADE DE TECNOLOGIA – FATEC
Análise e Desenvolvimento de Sistemas
Programação Web (PWEB)
DEVOPS: CONCEITOS, PRÁTICAS, FERRAMENTAS E BENEFÍCIOS
Atividade 2 – Pesquisa
Luiz Henrique da Silva Cervelati
Sorocaba
2026
 
1. Introdução
O desenvolvimento de software moderno exige entregas cada vez mais rápidas, frequentes e confiáveis. Historicamente, porém, as equipes de desenvolvimento (Dev) e de operações (Ops) trabalhavam de forma isolada, com objetivos conflitantes: enquanto o desenvolvimento buscava lançar novas funcionalidades rapidamente, as operações priorizavam a estabilidade dos sistemas em produção. Esse distanciamento gerava atritos, atrasos nas entregas e falhas recorrentes durante as implantações.
Nesse contexto surge o DevOps, um movimento cultural e técnico que propõe a integração entre desenvolvimento e operações por meio de colaboração, automação e medição contínua. O termo ganhou força a partir de 2009, com os eventos "DevOpsDays" organizados por Patrick Debois, e desde então consolidou-se como uma das principais abordagens para a entrega de software em escala (KIM et al., 2018).
Esta pesquisa apresenta os conceitos fundamentais do DevOps, suas principais práticas, as ferramentas mais utilizadas no mercado, os benefícios observados por organizações que o adotam e exemplos reais de aplicação, encerrando com uma conclusão sobre a relevância do tema para o desenvolvimento web e para a formação do profissional de tecnologia.
2. Conceitos Fundamentais
2.1 Definição
DevOps é a combinação de práticas, ferramentas e filosofias culturais que aumenta a capacidade de uma organização de entregar aplicações e serviços em alta velocidade, unificando os processos de desenvolvimento de software e de operações de infraestrutura (AWS, 2024). Mais do que um cargo ou uma ferramenta específica, DevOps é uma cultura organizacional que valoriza a responsabilidade compartilhada: quem desenvolve o software também participa da sua operação e monitoramento.
2.2 Os pilares CALMS
Um modelo amplamente utilizado para descrever os fundamentos do DevOps é o acrônimo CALMS:
•	Culture (Cultura): colaboração entre equipes, confiança e responsabilidade compartilhada pelos resultados;
•	Automation (Automação): eliminação de tarefas manuais repetitivas em build, testes, implantação e infraestrutura;
•	Lean (Enxuto): entregas em pequenos lotes, redução de desperdícios e foco no valor para o usuário;
•	Measurement (Medição): coleta de métricas de desempenho, disponibilidade e fluxo de entrega para orientar decisões;
•	Sharing (Compartilhamento): disseminação de conhecimento, ferramentas e lições aprendidas entre as equipes.
2.3 As "Três Maneiras" (The Three Ways)
Kim et al. (2018) descrevem três princípios que sustentam o DevOps: a primeira maneira trata do fluxo de trabalho rápido da esquerda para a direita (do desenvolvimento à produção); a segunda, do retorno rápido de informações (feedback) da produção para o desenvolvimento; e a terceira, de uma cultura de experimentação e aprendizado contínuos, na qual falhas são tratadas como oportunidades de melhoria.
3. Principais Práticas
3.1 Integração Contínua (CI)
Na integração contínua, os desenvolvedores integram seu código a um repositório compartilhado várias vezes ao dia. Cada integração dispara automaticamente a compilação (build) e a execução de testes automatizados, permitindo detectar defeitos rapidamente e reduzir problemas de integração (FOWLER, 2006).
3.2 Entrega e Implantação Contínuas (CD)
A entrega contínua (Continuous Delivery) garante que o software esteja sempre em estado implantável, com o processo de liberação automatizado até o ambiente de homologação. A implantação contínua (Continuous Deployment) vai além: cada alteração aprovada nos testes é publicada automaticamente em produção, sem intervenção manual (HUMBLE; FARLEY, 2010).
3.3 Infraestrutura como Código (IaC)
Servidores, redes e demais recursos de infraestrutura são definidos em arquivos de configuração versionados, tratados como código-fonte. Isso torna os ambientes reproduzíveis, auditáveis e menos sujeitos a erros manuais. Ferramentas como Terraform e Ansible são exemplos consolidados dessa prática.
3.4 Monitoramento e Observabilidade
Aplicações em produção são monitoradas continuamente por meio de métricas, logs e rastreamento distribuído (tracing). O objetivo é detectar anomalias antes que afetem os usuários e fornecer feedback rápido às equipes de desenvolvimento.
3.5 Microsserviços e Conteinerização
Embora não sejam obrigatórios, arquiteturas de microsserviços e contêineres (como Docker) são frequentemente associados ao DevOps, pois permitem implantar e escalar componentes de forma independente, acelerando o ciclo de entrega (BASS; WEBER; ZHU, 2015).
4. Ferramentas
O ecossistema DevOps é apoiado por um conjunto amplo de ferramentas, geralmente organizadas conforme a etapa do ciclo de vida do software:
•	Controle de versão: Git, GitHub, GitLab e Bitbucket;
•	CI/CD: GitHub Actions, GitLab CI/CD, Jenkins e Azure DevOps Pipelines;
•	Contêineres e orquestração: Docker e Kubernetes;
•	Infraestrutura como código: Terraform, Ansible e AWS CloudFormation;
•	Monitoramento e observabilidade: Prometheus, Grafana, Datadog e ELK Stack (Elasticsearch, Logstash e Kibana);
•	Comunicação e colaboração: Slack, Microsoft Teams e Jira.
É importante destacar que as ferramentas são um meio, e não um fim: a adoção de tecnologia sem a correspondente mudança cultural tende a reproduzir os mesmos silos que o DevOps busca eliminar (EBERT et al., 2016).
5. Benefícios
As pesquisas anuais State of DevOps, conduzidas pela equipe DORA (DevOps Research and Assessment), demonstram que organizações de alto desempenho em DevOps apresentam maior frequência de implantações, menor tempo entre a escrita do código e sua chegada à produção (lead time), menor taxa de falhas em mudanças e recuperação mais rápida de incidentes (FORSGREN; HUMBLE; KIM, 2018). Entre os principais benefícios, destacam-se:
•	Velocidade: entregas mais frequentes de funcionalidades e correções;
•	Qualidade e confiabilidade: testes automatizados e implantações padronizadas reduzem falhas em produção;
•	Escalabilidade: automação e infraestrutura como código permitem gerenciar ambientes complexos com consistência;
•	Colaboração: equipes compartilham responsabilidades, reduzindo conflitos entre desenvolvimento e operações;
•	Segurança: com a evolução para o DevSecOps, controles de segurança passam a ser automatizados e integrados desde o início do ciclo de desenvolvimento.
6. Exemplos de Aplicação
Grandes empresas de tecnologia foram pioneiras na adoção do DevOps. A Amazon, ao migrar para uma arquitetura de serviços e automatizar suas implantações, passou a realizar milhares de deploys por dia em seus sistemas. A Netflix tornou-se referência em resiliência ao criar ferramentas como o Chaos Monkey, que desliga componentes aleatoriamente em produção para garantir que o sistema tolere falhas. No Brasil, instituições financeiras como Itaú e Nubank e empresas de e-commerce utilizam pipelines de CI/CD, contêineres e computação em nuvem para entregar atualizações contínuas a milhões de usuários.
Em menor escala, um estudante ou uma equipe pequena também pode aplicar DevOps: versionando o código no GitHub, configurando um pipeline de build e testes com GitHub Actions e publicando automaticamente a aplicação em um serviço de nuvem a cada alteração aprovada.
7. Conclusão
O DevOps representa uma mudança profunda na forma de construir e operar software, substituindo silos organizacionais por colaboração, processos manuais por automação e decisões baseadas em intuição por métricas objetivas. As evidências apresentadas pela literatura e pelas pesquisas do setor indicam que sua adoção está diretamente associada a maior velocidade de entrega, maior qualidade e maior estabilidade dos sistemas.
Para o desenvolvedor web em formação, compreender DevOps deixou de ser um diferencial e tornou-se um requisito: práticas como versionamento, integração contínua e conteinerização estão presentes no dia a dia da maioria das equipes de desenvolvimento. Conclui-se, portanto, que o estudo do tema contribui tanto para a qualidade dos projetos acadêmicos quanto para a preparação do estudante para o mercado de trabalho.
Referências
AMAZON WEB SERVICES (AWS). O que é DevOps? 2024. Disponível em: https://aws.amazon.com/pt/devops/what-is-devops/. Acesso em: 16 ago. 2026.
ATLASSIAN. DevOps: quebrando a barreira entre desenvolvimento e operações. Disponível em: https://www.atlassian.com/br/devops. Acesso em: 16 ago. 2026.
BASS, L.; WEBER, I.; ZHU, L. DevOps: A Software Architect’s Perspective. Boston: Addison-Wesley, 2015.
EBERT, C.; GALLARDO, G.; HERNANTES, J.; SERRANO, N. DevOps. IEEE Software, v. 33, n. 3, p. 94-100, 2016.
FORSGREN, N.; HUMBLE, J.; KIM, G. Accelerate: The Science of Lean Software and DevOps. Portland: IT Revolution Press, 2018.
FOWLER, M. Continuous Integration. 2006. Disponível em: https://martinfowler.com/articles/continuousIntegration.html. Acesso em: 16 ago. 2026.
HUMBLE, J.; FARLEY, D. Continuous Delivery: Reliable Software Releases through Build, Test, and Deployment Automation. Boston: Addison-Wesley, 2010.
KIM, G.; HUMBLE, J.; DEBOIS, P.; WILLIS, J. Manual de DevOps: como obter agilidade, confiabilidade e segurança em organizações tecnológicas. Rio de Janeiro: Alta Books, 2018.
