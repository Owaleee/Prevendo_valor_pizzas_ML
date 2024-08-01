# Previsão do Valor da Pizza com Streamlit e Regressão Linear

Este projeto utiliza a biblioteca **Streamlit** para criar uma aplicação web interativa que prevê o valor de uma pizza com base no seu diâmetro. A previsão é feita usando um modelo de **Regressão Linear** treinado com dados de um arquivo CSV.

## Estrutura do Código

1. **Importação de Bibliotecas**:
   - `streamlit` para criar a interface web interativa.
   - `pandas` para manipulação e análise dos dados.
   - `sklearn.linear_model` para a criação e aplicação do modelo de regressão linear.

2. **Carregamento dos Dados**:
   - O arquivo CSV `pizzas.csv` é carregado em um DataFrame `df` com pandas. Este arquivo deve conter pelo menos duas colunas: `diametro` e `preco`.

3. **Preparação do Modelo**:
   - Um modelo de Regressão Linear é criado e ajustado (`modelo.fit`) usando o diâmetro da pizza (`x`) como variável independente e o preço (`y`) como variável dependente.

4. **Interface com o Usuário**:
   - Utilizando Streamlit, uma interface é criada com um título e um campo de entrada para o diâmetro da pizza.
   - Quando o usuário insere o valor do diâmetro, o modelo prevê o preço da pizza com base no diâmetro fornecido.

5. **Exibição dos Resultados**:
   - O preço previsto é exibido para o usuário no formato de reais (R$).
   - Um efeito visual de balões é adicionado para uma melhor experiência interativa.

## Como Executar

1. Certifique-se de ter as bibliotecas necessárias instaladas:
   ```bash
   pip install streamlit pandas scikit-learn
   ```

2. Coloque o arquivo `pizzas.csv` no mesmo diretório do script.

3. Execute a aplicação Streamlit com o comando:
   ```bash
   streamlit run nome_do_arquivo.py
   ```

4. Acesse a aplicação no navegador, geralmente disponível em `http://localhost:8501`.

## Arquivo CSV Exemplo

O arquivo `pizzas.csv` deve ter a seguinte estrutura:
```csv
diametro,preco
30,20.00
35,25.00
40,30.00
```

Certifique-se de que as colunas estão corretamente nomeadas e os dados estão no formato correto para garantir que o modelo funcione adequadamente.

## Observações

- Este exemplo simples usa dados fictícios e uma regressão linear básica. Para previsões mais precisas e robustas, considere utilizar um conjunto de dados mais abrangente.
- A aplicação foi projetada para fins educacionais e de demonstração. 

---

Se houver alguma dúvida ou necessidade de ajuda adicional, sinta-se à vontade para abrir uma issue no repositório.
