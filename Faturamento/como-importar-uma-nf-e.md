# Como importar uma NF-e

## Conhecimentos mínimos:
- Windows Básico
- Tributação básica
- Bravo Gestor – Estoque
- Bravo Gestor – Contas a pagar
- [Notas Fiscais de entrada e saida](notas-fiscais-de-entrada-e-saida.md)

## Escopo do treinamento:
- Salvar o arquivo na pasta de importação informada no ato da inclusão.
- Entrada do arquivo no Bravo Gestor.
- Onde lançar os tributos de saída do seu fornecedor convertidos para entrada em seu estabelecimento. Este tópico não cobre qual informação deve ser lançada.
- Vincular produtos da NF aos produtos cadastrados. Operação feita, automaticamente, pelo código de barras original cadastrado na ficha do produto.
- Cadastrar novos produtos.
- Acessar os campos de tributação.
- Emitir relatório de conferência de entrada de mercadorias.
- Emitir relatório de margem de lucro e sugestão de preço de venda.
- Formação de preços.
- Lançamento de duplicatas a pagar.
- Como o CFOP influencia a movimentação de estoque.
- Processamento da NF.

Com a importação do XML, não é necessário informar as tributações item a item. A vinculação de produtos também é automática pelo código de barras.

!!!
É importante salientar que a importação dispensa, somente, o trabalho do lançamento dos produtos e dos seus valores nos respectivos campos. Cabe, porém, ao operador, a responsabilidade da verificação e possível correção dos campos obrigatórios dos tributos de IPI, PIS, COFINS e ICMS, principalmente, se o XML apresentar valores inconsistentes e erros de cálculo. Em caso de dúvida, o responsável pela contabilidade da sua empresa deverá ser consultado. Não faz parte do suporte da Audisoft Sistemas o repasse de informações necessárias á compreensão dos cálculos e procedimentos pertinentes ao conteúdo dos documentos fiscais.
!!!

Na nota fiscal de entrada, ao pressionar I de Incluir, será feita a pergunta "Você recebeu o XML dessa nota fiscal?" Ao responder SIM, será informado o caminho da pasta para onde deve ser copiado o XML. Abra o email do XML e sobre DOWNLOAD, clique com botão direito do mouse e mande "salvar o link como" seguindo, rigorosamente todos os passos da mensagem. Ex. Computador, g:\audisoft\Bravo Gestor\dados\nfe\ano\mês\entrada e mande salvar.

Se tiver dificuldade em identificar o caminho indicado, escolha a opção "Abrir" e será aberta uma pasta. Depois de ter baixado o XML no local de sua preferência como em Downloads, Documentos, ou mesmo na área de trabalho, copie esse XML e cole dentro dessa pasta aberta pelo Bravo Gestor.

Se seu fornecedor não lhe enviou o XML, ou o enviou com defeito, acesse esse o [Portal da Nota fiscal eletrônica](http://www.nfe.fazenda.gov.br/portal/principal.aspx) e, depois de informados os dados do XML e no final da página seguinte, faça o ''Download do documento''.

Volte à nota fiscal e confirme a mensagem com ENTER. Responda SIM à pergunta seguinte e ao confirmar o número da fatura será aberta uma lista com o XML baixado. O passo seguinte permitirá consultar junto à SEFAZ a legitimidade do XML, caso queira. Informe, então o CFOP de entrada e o ST do frete, caso haja e seja incluído na nota fiscal.

As telas seguintes, permitem que você faça a conversão de forma fácil e rápida das informações tributárias de saída do seu fornecedor para os seus valores de entrada.

Serão apresentadas telas para alteração dos tributos em grupo (CFOP, IPI, PIS, COFINS e ICMS).

Caso haja alguma dúvida, entre em contato com o responsável pela contabilidade da sua empresa. Exemplos do quê perguntar a ele:

Meu fornecedor enviou a Nota Fiscal com:

- O CFOP 6403. Qual CFOP devo utilizar na entrada?
- O CST 010. Qual CST devo utilizar na entrada?
- O IPI 51. Qual CST devo utilizar na entrada?
- O PIS e COFINS 01. Qual CST devo utilizar na entrada?

!!!
Os lançamentos dos CFOP e CST de entrada vão depender dos destinos que serão dados às mercadorias dessa nota fiscal. Se são para revenda, industrialização, consumo, brinde, ativo imobilizado etc e se é permitido, ou não, o aproveitamento do crédito dos impostos desse produto. Não faça qualquer lançamento na dúvida. Consulte, antes, o seu contador. Um lançamento errado vai gerar divergências entre os seus valores informados nos  aquivos gerados para o Sintegra e o SPED e os lançamentos efetuados pelo escritório de contabilidade. E essa responsabilidade não poderá ser imputada à Audisoft Sistemas.
!!!

Para alterar os valores, pressione A para alterar e informe o valor de entrada a ser aplicado em todos os produtos configurados com o valor da coluna à esquerda. Para encerrar as alterações, pressione ESC e escolha SIM para confirmar a alteração.

Quando terminar a configuração dos tributos, será apresentada a lista de produtos. Se precisar executar as telas para alteração dos tributos em grupo novamente, pressione G.

Pressione ENTER para acessar a ficha do produto e efetue as alterações necessárias. Para vincular o item baixado com o mesmo da sua lista de produtos, pressione A de alterar, pressione enter para abrir a lista de produtos, busque o produto correspondente na lista e confirme. Faça isso em todos os produtos e, caso algum ainda não conste da sua lista, faça o cadastro obedecendo às instruções do cadastramento, em [Cadastro de produtos](../Estoque/cadastro-de-produtos.md).

Nota: Caso o seu fornecedor informe o código de barras de cada produto e que seja o mesmo constante do seu cadastro, o Bravo Gestor fará o vínculo, automaticamente. O fator de conversão (Embala e Desembala), que significa o múltiplo ou a fração da embalagem do fornecedor em relação à embalagem de venda, deve ser informado, individualmente, em cada produto, quando houver.

Para as notas fiscais a prazo, pressione D na tela de entrada, e na lista dos documentos de crédito, pressione A para alterar e completar os dados de cada documento. Ao sair com ESC, responda SIM para o lançamento dos documentos no contas a pagar.

!!!
O nome arquivo deve conter a extensão .XML, caso seu fornecedor tenha feito o envio sem essa informação, faça a correção. Do contrário a importação não será possível. Faça a revisão dos valores lançados na nota fiscal, pois pode acontecer de algum XML conter dados inconsistentes, principalmente dos tributos dos itens.. 
!!!

Muita atenção para as mensagens de alerta sobre a consistência dos valores e tributos lançados nos itens e os totais informados nos valores da nota fiscal. Faça as alterações e ajustes necessários, até que essas mensagens desapareçam. Toda nota fiscal com inconsistência de valores não passa na validação do SPED fiscal.

Finalmente, pressione P para processar a nota fiscal e concluir a entrada dos produtos no estoque.

## Erros durante a importação de uma NF-e:

Mensagem: "Este XML não possui o protocolo de autorização."
Motivo: O arquivo XML não é válido por não ter o protocolo gerado pela Secretaria da Fazenda (SEFAZ) nele. O protocolo é o "Carimbo" da SEFAZ na nota fiscal eletrônica. Sem ele, o arquivo XML é inválido.
 
Solução 1: Informe o ocorrido ao seu fornecedor e peça que lhe envie o arquivo validado e assinado pela SEFAZ.
 
Solução 2: Você pode fazer uma consulta através do link: Consultar NF-e Completa - Portal da Nota Fiscal Eletrônica e verificar manualmente a validade da NF-e. Caso ela seja realmente válida, você pode ignorar o alerta do Bravo Gestor e importar o XML normalmente.
 
Caso haja alguma dúvida sobre o protocolo existir ou não, identifique manualmente da seguinte forma: 
Abra-o utilizando o internet explorer e procure, no final do arquivo, por um trecho parecido com o seguinte:

`<protNFe xmlns="http//www.portalfiscal.inf.br/nfe" versao="2.00">`