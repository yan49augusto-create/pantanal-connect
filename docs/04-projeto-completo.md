# 4. Projeto Integrador — Complementação da Proposta Pantanal Connect

**Autor:** Yan Augusto Silva Miranda  
**Instituição:** Universidade de Cuiabá — UNIC Beira Rio  
**Curso:** Ciência da Computação — 8º semestre  
**Disciplina:** Desenvolvimento de Soluções Remotas  
**Professor:** Felipe Douglas  
**Local:** Cuiabá — MT  
**Ano:** 2026

## 4.1 Usabilidade e experiência do usuário

O Pantanal Connect propõe uma estrutura de trabalho remoto para o Centro Administrativo Pantanal, organização fictícia de Cuiabá com aproximadamente 35 colaboradores.

A usabilidade representa a facilidade com que os funcionários conseguem utilizar as ferramentas propostas. A experiência do usuário (UX) considera toda a interação com os serviços, enquanto a interface do usuário (UI) corresponde aos elementos visuais e controles utilizados.

A proposta deverá priorizar eficiência, eficácia, facilidade de aprendizagem e satisfação dos colaboradores.

### Princípios de interface

- Consistência visual e padronização dos sistemas.
- Navegação simples e informações organizadas.
- Feedback claro após ações importantes.
- Visibilidade do estado de tarefas, arquivos e conexões.
- Prevenção de erros e confirmação de operações críticas.
- Design responsivo para computadores, tablets e celulares.

As plataformas escolhidas deverão apresentar interfaces intuitivas, reduzindo a necessidade de treinamentos extensos.

## 4.2 Usabilidade em soluções remotas

A solução deverá funcionar por meio de aplicações Web, ferramentas móveis e sistemas colaborativos.

Para funcionários com internet limitada, serão priorizadas ferramentas que permitam comunicação assíncrona, arquivos compactados e redução da qualidade de vídeo durante reuniões.

Também serão definidos procedimentos alternativos para períodos de indisponibilidade dos serviços.

## 4.3 Acessibilidade digital

A acessibilidade permite que pessoas com diferentes necessidades utilizem os recursos digitais com autonomia.

A proposta considera as recomendações WCAG 2.2, buscando atingir o nível AA nos sistemas e conteúdos sob controle da organização.

Serão observados:

- Contraste adequado entre textos e fundos.
- Tipografia legível e possibilidade de ampliação.
- Navegação por teclado.
- Compatibilidade com leitores de tela.
- Textos alternativos para imagens informativas.
- Legendas em conteúdos audiovisuais.
- Identificação clara dos campos de formulários.
- Mensagens de erro compreensíveis.
- Compatibilidade com tecnologias assistivas.

A conformidade deverá ser verificada por avaliações técnicas e testes com usuários.

## 4.4 Avaliação de usabilidade

Antes da implantação, será desenvolvido um protótipo ou ambiente de demonstração com os principais fluxos de trabalho.

Serão realizados testes com representantes dos setores administrativo, financeiro, atendimento, gestão e TI.

As atividades avaliadas incluirão:

1. Entrar no sistema utilizando autenticação multifator.
2. Localizar e compartilhar um documento.
3. Participar de uma reunião virtual.
4. Registrar e acompanhar uma tarefa.
5. Solicitar suporte técnico.

A avaliação utilizará observação dos usuários, questionários de satisfação e inspeção heurística baseada em princípios de usabilidade.

Os problemas identificados serão classificados por gravidade e corrigidos antes da implantação definitiva.

## 5.1 Fundamentos de redes

O projeto utiliza conceitos de redes LAN, MAN e WAN.

A LAN corresponde à rede local da empresa, conectando computadores, impressoras e outros equipamentos.

A MAN representa redes de abrangência metropolitana, enquanto a WAN conecta redes geograficamente distantes. A internet é utilizada para conectar os funcionários remotos aos serviços autorizados.

A comunicação ocorre com base no modelo TCP/IP, utilizando endereçamento IP e protocolos como TCP, UDP, HTTPS e DNS.

A infraestrutura poderá combinar conexões cabeadas Ethernet e redes sem fio Wi-Fi.

## 5.2 Redes convergentes

Uma rede convergente permite transportar diferentes serviços, como dados, voz e vídeo, sobre uma infraestrutura de comunicação integrada.

Essa abordagem evoluiu com a adoção de redes baseadas em IP e facilita a utilização de ferramentas de colaboração, telefonia e videoconferência.

No Pantanal Connect, a convergência será aplicada à comunicação entre colaboradores, permitindo reuniões virtuais, compartilhamento de documentos e serviços multimídia.

## 5.3 Protocolos e serviços de comunicação

As ferramentas de comunicação poderão utilizar tecnologias como:

- VoIP: transmissão de voz por redes IP.
- SIP: sinalização utilizada em determinadas soluções de telefonia IP.
- RTP: transporte de mídia em tempo real.
- RTCP: informações de controle e qualidade relacionadas ao RTP.
- Streaming: transmissão contínua de áudio e vídeo.
- Videoconferência: comunicação audiovisual entre participantes.
- OTT: serviços fornecidos sobre a infraestrutura de internet.

Os protocolos efetivamente utilizados dependerão das plataformas contratadas. Nem toda ferramenta de videoconferência utiliza SIP.

## 5.4 Qualidade de Serviço (QoS)

A qualidade das comunicações depende de fatores como latência, jitter, perda de pacotes e largura de banda disponível.

Latência elevada pode causar atrasos nas conversas. O jitter representa a variação do atraso entre pacotes, enquanto a perda de pacotes pode prejudicar áudio e vídeo.

A proposta prevê priorização de tráfego de comunicação em tempo real nos equipamentos de rede administrados pela organização, quando houver suporte.

Também serão recomendadas conexões estáveis e a redução de tráfego desnecessário durante reuniões.

## 5.5 Tecnologias de acesso remoto

As principais tecnologias consideradas são:

- VPN: conexão protegida para acessar recursos internos.
- SSH: administração remota segura de servidores e equipamentos autorizados.
- Remote Desktop: acesso remoto à interface de computadores.
- Virtualização: execução de ambientes virtuais sobre infraestrutura física.
- VDI: disponibilização de desktops virtuais centralizados.
- Computação em nuvem: fornecimento de aplicações e infraestrutura pela internet.
- Aplicações Web: acesso aos sistemas por navegadores.
- Armazenamento em nuvem: compartilhamento e sincronização de documentos.

O projeto prioriza aplicações Web e serviços em nuvem, utilizando VPN para sistemas internos que não possam ser disponibilizados diretamente.

SSH e acesso remoto à área de trabalho ficarão restritos a profissionais autorizados, quando necessários.

## 5.6 Arquitetura de rede proposta

A arquitetura combina serviços em nuvem, rede corporativa e acesso remoto protegido.

### Diagrama lógico simplificado

```text
       COLABORADORES REMOTOS
        Notebook / Celular
                |
          Internet / HTTPS
                |
        +-------+--------+
        |                |
        v                v
  Serviços em nuvem   VPN + MFA
  - Documentos          |
  - Comunicação         v
  - Gestão de tarefas  Firewall
                         |
                         v
                  Rede corporativa
                         |
               +---------+---------+
               |                   |
         Sistemas internos    Administração TI
```

O diagrama representa uma arquitetura conceitual, não uma infraestrutura já implantada.

O acesso aos serviços em nuvem deverá utilizar autenticação e conexões criptografadas. O acesso aos sistemas internos será realizado por VPN, com permissões específicas.

## 5.7 Segurança de redes

A segurança será organizada em diferentes camadas de proteção.

### Medidas propostas

- Firewall para filtragem das conexões de rede.
- VPN para acesso remoto a sistemas internos.
- Criptografia dos dados em trânsito.
- Autenticação multifator (MFA).
- Controle de acesso baseado em funções.
- Segmentação da rede administrativa e de visitantes.
- Atualizações e correções de segurança.
- Monitoramento de eventos e registros de acesso.
- Backup com testes periódicos de recuperação.
- Treinamento sobre phishing e proteção de credenciais.

A política de segurança deverá considerar a Lei Geral de Proteção de Dados Pessoais (LGPD), especialmente no tratamento de informações de colaboradores e clientes.

## 6.1 Objetivo do projeto integrador

Desenvolver uma proposta técnica para permitir que o Centro Administrativo Pantanal adote um modelo de trabalho remoto ou híbrido com segurança, organização, acessibilidade e continuidade operacional.

A solução é apresentada como planejamento acadêmico, sem afirmar que houve implantação real.

## 6.2 Etapas de implantação

**Etapa 1 — Diagnóstico:** entrevistas com usuários e levantamento dos sistemas existentes.

**Etapa 2 — Planejamento:** definição das ferramentas, requisitos, permissões e orçamento.

**Etapa 3 — Preparação:** configuração da infraestrutura, contas, autenticação e políticas.

**Etapa 4 — Projeto-piloto:** testes com um grupo reduzido de funcionários.

**Etapa 5 — Capacitação:** treinamento dos colaboradores e divulgação das orientações.

**Etapa 6 — Implantação:** ampliação gradual da solução aos demais setores.

**Etapa 7 — Avaliação:** acompanhamento de indicadores e correção dos problemas identificados.

## 6.3 Estimativa preliminar de custos

Os valores abaixo são hipóteses acadêmicas para planejamento, não cotações comerciais verificadas.

| Item | Tipo | Estimativa |
|---|---|---:|
| Ferramentas de colaboração (35 usuários) | Mensal | R$ 1.400 |
| Backup e armazenamento adicional | Mensal | R$ 250 |
| VPN e monitoramento | Mensal | R$ 200 |
| Treinamento inicial | Único | R$ 1.500 |
| Equipamentos e ajustes de rede | Único | R$ 3.000 |
| Configuração e implantação | Único | R$ 2.000 |

**Custo inicial estimado:** R$ 6.500.

**Custo mensal estimado:** R$ 1.850.

**Custo total estimado para o primeiro ano:** R$ 28.700, considerando o investimento inicial e doze mensalidades.

Os valores deverão ser revisados após o levantamento real das necessidades e a obtenção de propostas dos fornecedores.

## 6.4 Cronograma proposto

| Atividade | Prazo |
|---|---|
| Levantamento de necessidades | Semana 1 |
| Planejamento e seleção de ferramentas | Semana 2 |
| Configuração de infraestrutura e segurança | Semanas 3 e 4 |
| Testes de usabilidade e acessibilidade | Semana 5 |
| Treinamento e projeto-piloto | Semana 6 |
| Implantação gradual | Semana 7 |
| Avaliação e ajustes finais | Semana 8 |

O cronograma é estimativo e poderá sofrer alterações conforme a complexidade da organização.

## 6.5 Indicadores de avaliação

A avaliação da solução poderá considerar:

- Percentual de usuários que conseguem acessar os serviços sem dificuldades.
- Tempo médio para concluir tarefas frequentes.
- Quantidade de incidentes de segurança registrados.
- Disponibilidade dos serviços essenciais.
- Tempo de atendimento das solicitações de suporte.
- Satisfação dos colaboradores.
- Resultados dos testes de acessibilidade.
- Cumprimento do orçamento previsto.

As metas deverão ser definidas após o diagnóstico e o estabelecimento de uma linha de base.

## 6.6 Riscos e medidas preventivas

| Risco | Medida proposta |
|---|---|
| Instabilidade da internet | Alternativas assíncronas e plano de contingência |
| Vazamento de informações | MFA, criptografia e controle de acesso |
| Resistência dos funcionários | Treinamento e suporte |
| Indisponibilidade de serviços | Backups e procedimentos de recuperação |
| Aumento de custos | Monitoramento financeiro e revisão de contratos |
| Dificuldades de acessibilidade | Testes e correções de interface |

## 6.7 Apresentação e defesa da solução

Na apresentação, o projeto deverá ser explicado a partir do problema enfrentado pela organização, das tecnologias selecionadas e dos benefícios esperados.

O diagrama da arquitetura servirá para demonstrar a conexão entre colaboradores, serviços em nuvem e sistemas internos.

A estimativa de custos e o cronograma permitirão discutir a viabilidade da proposta.

## 7. Conclusão

O Pantanal Connect apresenta uma proposta de modernização da estrutura de trabalho remoto para uma organização fictícia de Cuiabá.

O projeto reúne conceitos de usabilidade, acessibilidade digital, redes convergentes, acesso remoto, segurança da informação e planejamento de infraestrutura.

A proposta demonstra que a adoção do trabalho remoto exige mais do que ferramentas de videoconferência: também depende de políticas, treinamento, conectividade, proteção de dados e acompanhamento dos resultados.

Conclui-se que a solução é tecnicamente plausível, mas sua implantação dependeria da validação dos requisitos, dos custos e da infraestrutura disponível.

## Referências essenciais

BRASIL. Lei nº 13.709, de 14 de agosto de 2018. Lei Geral de Proteção de Dados Pessoais.

KUROSE, James F.; ROSS, Keith W. Redes de computadores e a Internet: uma abordagem top-down.

NIELSEN, Jakob. Usability Engineering. San Francisco: Morgan Kaufmann, 1993.

ROGERS, Yvonne; SHARP, Helen; PREECE, Jennifer. Design de interação: além da interação humano-computador.

W3C. Web Content Accessibility Guidelines (WCAG) 2.2. Disponível em: https://www.w3.org/TR/WCAG22/.

As referências bibliográficas complementares estão disponíveis no arquivo de referências da raiz do repositório.
