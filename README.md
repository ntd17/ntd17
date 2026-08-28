## João Victor de Assis Natividade

**Data & Risk** — crédito, seguros e analytics financeiro.

Engenheiro de Software pela Univates, técnico em Contabilidade e Finanças, pós-graduando em
Ciência de Dados e Analytics pela PUC-Rio.

Desde 2021 analiso risco de crédito para setor de seguros e imobiliário  —
e construo os sistemas que sustentam essa análise. Não são duas carreiras: é a mesma. O que me
interessa é o ponto onde o modelo encosta na decisão financeira, porque é ali que errar custa
dinheiro de verdade.

Se tem um fio comum no que eu construo, é este: **desenhar sistemas onde a informação não pode
divergir, porque as duas pontas se travam.** Aprendi isso em contabilidade — partida dobrada não
confia no lançamento, confia em que o balanço não fecha se ele estiver errado — e passei a
aplicar em software.

📍 Santa Cruz do Sul, RS

---

### Projetos

**[ChequeDigital](https://github.com/ntd17/ChequeDigital)** — Primitiva de liquidação condicional
para o trilho instantâneo brasileiro

White paper. O Pix acertou o trilho e descartou o tempo; a proposta devolve o tempo como a
variável que permite condicionar a liquidação a um fato verificável — nota fiscal emitida,
propriedade transferida, mercadoria entregue. Nenhum componente é ficção: Pix, Drex, split
payment, MED, Registrato e registradoras de recebíveis já existem em produção. A contribuição
está na composição.

`fintech` `pagamentos` `desenho de mecanismo`

---

**[ricarol-smart-contracts](https://github.com/ntd17/ricarol-smart-contracts)** — Plataforma P2P
de contratos digitais com validade jurídica

Contratos criados, assinados e arquivados de forma imutável, sem intermediário. Smart contracts
em Ethereum, armazenamento em IPFS/Filecoin, assinatura digital e prova de execução on-chain.
Prazos sensíveis ao clima se ajustam sozinhos por oráculo meteorológico.

A parte que não aparece na stack: a fundamentação jurídica é própria. A validade da assinatura
vem da MP 2.200-2/2001 e da Lei 14.063/2020; a cláusula arbitral em contrato eletrônico se apoia
no REsp 1608014/SP; e o STJ já dispensou testemunhas no art. 784, II do CPC quando há assinatura
digital ICP-Brasil — o que faz do contrato gerado pela plataforma um **título executivo
extrajudicial**, executável sem processo de conhecimento.

A conclusão mais útil é uma limitação: medi o custo real de gas e o deploy sai a R$ 657 contra
R$ 58 por contrato criado. O custo fixo inviabiliza acordos de baixo valor sem soluções de camada
superior — exatamente o público que mais se beneficiaria de dispensar o cartório.

`Python` `Flask` `Solidity` `Web3.py` `IPFS` `Celery` `Redis` `Docker` `TensorFlow`

---

**[ml-rainfall-forecast](https://github.com/ntd17/ml-rainfall-forecast)** — Previsão de chuva com
protocolo honesto

Classificação binária com dados públicos do Open-Meteo: divisão temporal (não aleatória),
baselines de persistência e classe majoritária, quatro modelos comparados, GridSearch com
TimeSeriesSplit.

Nasceu de uma auditoria do meu próprio TCC. O pipeline original reportava 93,4% de acurácia —
número alto demais para previsão a um dia, já que modelos numéricos operacionais, rodando em
supercomputador, acertam entre 85% e 90%. Fui atrás e achei vazamento de alvo: a variável
dependente estava entre as variáveis de entrada. Rastreei até a linha, documentei o mecanismo e
refiz do zero.

O resultado honesto é F1 de 0,64 contra 0,578 da persistência — margem estreita, reportada como
tal. Métrica boa demais é motivo para desconfiar, não para comemorar.

`scikit-learn` `TensorFlow` `pandas` `Jupyter`

---

**[taskflow-backend-api](https://github.com/ntd17/taskflow-backend-api)** — API REST colaborativa
estilo Kanban

Boards, listas e cards com autenticação JWT, compartilhamento entre membros e documentação
Swagger. Sobe inteiro com um `docker-compose up`: Flask e PostgreSQL conteinerizados.

O README documenta o modelo de permissões inclusive onde ele é limitado — todos os membros têm
direitos iguais, sem papel de dono. Limitação declarada vale mais que limitação descoberta pelo
usuário.

`Flask` `JWT` `PostgreSQL` `SQLAlchemy` `Docker` `Swagger`

---

**[mvp-eda-avc](https://github.com/ntd17/mvp-eda-avc)** — Análise exploratória e pré-processamento
de base clínica

5.110 pacientes, predição de risco de AVC. Hipóteses formuladas antes de olhar os dados,
desbalanceamento severo (4,87% de positivos) tratado como característica do fenômeno e não como
defeito da base, e divisão treino/teste feita antes de qualquer transformação de escala.

`pandas` `scikit-learn` `Matplotlib` `Seaborn`

---

### Stack

| | |
|---|---|
| **Dados & ML** | Python · SQL · scikit-learn · TensorFlow/Keras · pandas · validação temporal · credit scoring |
| **Backend** | Flask · SQLAlchemy · Celery · Docker · microsserviços · Apache Tomcat/TomEE |
| **Bancos** | PostgreSQL · MySQL · Redis · Neo4j (Cypher) |
| **Blockchain** | Ethereum · Solidity · Web3.py · IPFS/Filecoin |
| **Negócio** | matemática financeira e ROI · análise de crédito · prevenção a fraudes · avaliação de risco |

---

### Contato

[LinkedIn](https://www.linkedin.com/in/joao-victor-de-assis-natividade-862474281/)
