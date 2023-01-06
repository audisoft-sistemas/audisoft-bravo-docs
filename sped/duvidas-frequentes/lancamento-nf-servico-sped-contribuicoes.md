# Lançamento de NF de serviço no SPED Contribuições

Lançamento de NF de serviço no SPED Contribuições

!!!
Antes de fazer o lançamento das notas no validador, o sped já deve está pronto e sem outros erros além dos que são corrigidos diretamente no validador. 
!!!

- Abra o validador como administrador, localize o arquivo para validação:
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/01.png)

- Após importar o arquivo, clique na opção de gerar apuração das contribuições:
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/02.png)

- Após a apuração, clique em verificar pendências de escrituração, para o arquivo ser validado novamente:
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/03.png)

- Após a nova validação, os erros mudam, agora as notas de serviço podem ser lançadas.
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/04.png)

- Clique em escrituração - efd contribuições
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/05.png)

- Clique em informações dos estabelecimentos e no cnpj da empresa:
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/06.png)

- Clique no estabelecimento e em itens para cadastrar o produto serviço
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/07.png)

- Clique em mais para incluir o novo registro
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/08.png)

Cadastre o produto serviço com essas informações: código (123456 para não ter conflito com outro produto), nome, unidade de medida, tipo do item e código do gênero: 
Após preencher, clique em salvar.
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/09.png)

Clique em cadastro de participantes para cadastrar os clientes e fornecedores das notas de serviço
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/10.png)

Clique em incluir novo registro: 
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/11.png)

- Preencha os dados do participante. Apenas a Inscrição estadual não é obrigatória, os outros campos devem ser preenchidos.
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/12.png)

- Preencha os dados do fornecedor/cliente de acordo com as informações da nota fiscal. O código vai ser o cnpj/cpf sem pontos nem traços mais a sigla do estado referente. Para localizar o município com mais facilidade, acesse o site do ibge, tecle ctrl F para buscar mais facilmente. 
Exemplo: 
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/13.png)

Informando o código da cidade no sped, ele já localiza:
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/14.png)

O cadastro do participante ficará dessa forma:
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/15.png)

Exemplo de nota fiscal de entrada de serviço.  
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/16.png)

## Após a inclusão do item serviço dos participantes, cadastre as notas fiscais de serviço.

## Lançamento de nota fiscal de serviços prestados pelo contribuinte (nota fiscal de saída):
- Clique em informações do estabelecimento - selecione o estabelecimento - documentos fiscais de saídas - A100 NF de serviços 
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/17.png)


- Clique em incluir registro 
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/18.png)

- Preencha os dados de acordo com a nota fiscal, no participante localize na lista.
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/19.png)

- Os dados obrigatórios são indicador do emitente, participante, situação do documento, número do documento, data de emissão, data de execução, tipo de pagamento, valor total do documento, base de cálculo do PIS/Pasep, base de cálculo do Cofins, valor do pis/pasep e valor do cofins. 
    - Indicador do emitente sempre será 0 - Emissão própria, situação sempre regular e o tipo de pagamento a vista. - Nos campos de valor total e base de cálculo pis/cofins, informe o valor total da nota. 
    - Para calcular os valores, use o seguinte cálculo:
    ```
    Pis/Pasep: valor total da nota x 1,65%
    Cofins...: valor total da nota x 7,60%
    ```
    - Após preencher as informações, clique em salvar. 
    !!!
    As alíquotas mudam quando o cliente é lucro presumido, nesse caso as alíquotas são PIS/Pasep 0,65% e Cofins 3%. 
    !!!

![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/20.png)


- Para cadastro do item na nota fiscal, clique em cima da nota que já fica selecionada após a inclusão e na parte de baixo escolha itens do documento:
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/21.png)


- Clique em incluir registro e preencha os dados. 
    - Os campos obrigatórios são número sequencial, código do item, valor total, cst pis/pasep, cst cofins, base de cálculo pis/pasep, base de cálculo cofins, alíquota pis/pasep, alíquota cofins, valor do pis/pasep, valor do cofins e conta analitica contábil. 
    - O número sequencial sempre será 1
    - O código do item será 123456, como foi cadastrado anteriormente
    - O valor total e as bases de cálculo, são os valores totais da nota
    - O cst para saída é 01
    - A alíquota de pis/pasep é 1,65%
    - A alíquota de cofins é 7,60% 
    - Os valores são os mesmos que foram obtidos anteriormente com o cálculo:
    ```
    Pis/Pasep: valor total da nota x 1,65%
    Cofins ..: valor total da nota x 7,60%
    ```
    - A conta analitica é `REVENDA DE MERCADORIA`

Após preencher as informações, clique em salvar. Para lançar outras notas de saída, repita o procedimento. 
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/22.png)

## Lançamento de nota fiscal de serviços prestados ao contribuinte (nota fiscal de entrada):

- Clique em documentos fiscais de entrada - NF de serviço 
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/23.png)

O procedimento é parecido com das notas de saída, clique na opção incluir registro e preencha os campos:
Campos obrigatórios: indicador do emitente, participante, situação do documento, número do documento, data de emissão, data de execução, tipo de pagamento, valor total do documento, base de cálculo do PIS/Pasep, base de cálculo do Cofins, valor do pis/pasep e valor do cofins.

Para o cálculo do valor, a regra é a mesma: 
```
Pis/Pasep: valor total da nota x 1,65%
Cofins ..: valor total da nota x 7,60%
```
![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/24.png)

- Após incluir a nota, inclua o item. 

![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/25.png)





- Inclua o registro e preencha os dados: 
    - Os campos obrigatórios são: número sequencial, código do item, valor total, natureza da base de cálculo do crédito, - origem do crédito, cst pis/pasep, cst cofins, base de cálculo pis/pasep, base de cálculo cofins, alíquota pis/pasep, - alíquota cofins, valor do pis/pasep, valor do cofins e conta analitica contábil. 
    - O número sequencial sempre será 1
    - O código do item será 123456, como foi cadastrado anteriormente
    - O valor total e as bases de cálculo, são os valores totais da nota
    - O cst para entrada é 50
    - A alíquota de pis/pasep é 1,65%
    - A alíquota de cofins é 7,60% 
    - Os valores são os mesmos que foram obtidos anteriormente com o cálculo:
    ```
    Pis/Pasep: valor total da nota x 1,65%
    Cofins ..: valor total da nota x 7,60%
    ```
    A conta analitica é `COMPRA PARA COMERCIALIZAÇÃO.`

    Após preencher as informações, clique em salvar e a nota estará lançada. Para lançar outras notas de entrada, repita o procedimento. 

![Alt text](../../assets/lancamento-nf-servico-sped-contribuicoes/26.png)


# Gerar apuração das contribuições

Após a inclusão das notas, clique novamente em gerar apuração das contribuições e depois em verificar pendências de escrituração, corrija os erros dos registros e valide o arquivo novamente. Após o arquivo estar sem erros, está pronto para ser enviado para a contabilidade. 
