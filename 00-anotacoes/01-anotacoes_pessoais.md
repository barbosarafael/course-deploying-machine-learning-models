# 1. Overview de deploy de modelos de ML

---

## 1.1. Desafios do deploy de modelos de ML

Desafios advindos do software tradicional: 

- Confiabilidade
- Reusabilidade 
- Manutenção
- Flexibilidade

Desafios advindos do Machine Learning: 

- Reproducibilidade 

Precisa de coordenação entre os times de Negócios, Engenheiros e Cientistas de dados

### 1.2. Ambiente de pesquisa/experimentação

- Conjunto de ferramentar para a construção e experimentação de modelos de ML
- Ferramentas úteis: Python para exploração

### 1.3. Ambiente de produção

- Ambiente em tempo real com configurações pré-definidas automaticamente 
- Ferramentas útéis: Docker e Python

### 1.4. Reproducibilidade

É a habilidade de reproduzir exatamente o mesmo modelo/resultado criado em algum momento do tempo. Claro, considerando que estaremos utilizando os mesmos dados. 


1. Ajuda a outras pessoas a replicar sua análise/modelo
2. Sem perda de tempo para reproduzir algo já pronto
3. Economia de tempo, também é economia de dinheiro


Nos **dados**, podemos salvar uma amostra para salvar e modelar os dados baseado nessa amostra. 

Durante a criação de features, podemos: 

- Muitos dos parâmetros são extraídos dos dados utilizados, mas, como vimos acima, os dados podem ser reprodutíveis também
- Em casos de amostras aleatórias, sempre utilizar o `random_seed`

Durante o treinamento o modelo, podemos: 

- Ordem das variáveis
- Armazenar as variáveis transformadas
- Armazenar os hiperparâmetros

Durante o deploy do modelo:

- Usar *container* para trackear as especificações do software
- Unificar todo o fluxo de análise e deploy em um único software


Links úteis sobre deploy: 

- https://trainindata.medium.com/how-to-build-and-deploy-a-reproducible-machine-learning-pipeline-20119c0ab941
- https://arxiv.org/ftp/arxiv/papers/1810/1810.04570.pdf
- https://www.rctatman.com/files/Tatman_2018_ReproducibleML.pdf
- https://petewarden.com/2018/03/19/the-machine-learning-reproducibility-crisis/
- https://opensource.com/life/15/12/why-open-source