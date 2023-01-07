# Notas Fiscais de entrada e saída

O módulo FATURAMENTO do Bravo Gestor oferece todas as opções necessárias e integradas para a emissão e recebimento de notas fiscais, cadastramento de fornecedores e produtos, além da formação dos preços de venda dentro da lista de itens da nota fiscal de compra.

Antes da inclusão de uma nota fiscal de compra ou venda, o operador deve ter a certeza de que o CFOP está configurado corretamente, quanto à incidência de impostos, à formação de preços e à movimentação do estoque contábil e administrativo. Para isso, acesse o menu UTILITÁRIOS e veja em CFOP as configurações pertinentes a cada operação. Caso ainda não exista, tecle I e inclua o CFOP desejado informando o termo da operação. Inclua a observação ou tecle ESC para confirmar e marque com X em todos os campos referentes às tributações e configurações necessárias.

As regras abaixo devem ser rigorosamente obedecidas, pois não poderão mais ser alteradas as configurações dos CFOPs já utilizados em lançamentos de notas fiscais de entrada ou saída.

## CFOP nas notas fiscais de saída.

Para a empresa optante pelo Simples (EPP ou Micro), a configuração do CFOP não deve conter nenhum tributo, marcando apenas CONTÁBIL, já que não deve ser destacado qualquer imposto e mesmo o estoque administrativo deve ficar em branco, pois ele já é baixado no ato da pré venda, EXCETO, nos casos em que a operação exigir os destaques dos tributos como nas devoluções para fornecedores.
Para a empresa de maior porte, devem ser marcados todos os tributos dos quais é contribuinte, como ICMS, IPI ou ST, além do estoque contábil.
Configurações especiais: TRANSFERÊNCIA, para a empresa que possui movimentações entre depósito fechado e loja, CONSUMIDOR, para operações de cobertura das vendas no ECF, ou nas vendas para consumidor de outro estado, em que se aplica a tributação interna do estado de origem, ou COMPLEMENTAR, quando somente os valores do tributos assinalados podem constar na nota fiscal. Essa última observação vale para ambos o CFOPs de entrada ou de saída.

!!!
Nota: Pode haver necessidade, também, de variações de um CFOP, como por exemplo, 5102-1, quando um CFOP for utilizado numa mesma operação com finalidade diferente. Como no caso em que a venda para um consumidor ou contribuinte for tributada de ICMS e esse mesmo produto, quando vendido para um produtor rural possui diferimento ou isenção. Nesse caso utiliza-se o mesmo CFOP com uma variação tipo 5102-1 configurado com o imposto em questão, nesse caso, desmarcado.
!!!

## CFOP nas notas fiscais de entrada.

Na compra de mercadorias para revenda, as opções ESTOQUE, CONTÁBIL e FINANCEIRO, devem ser obrigatoriamente marcadas para que haja movimentação dos produtos nos dois estoques e gere informações para a formação de preços, além de todos os tributos incidentes como ICMS, IPI para as operações sujeitas a esses tributos e ICMS, IPI e SUBSTITUIÇÃO TRIBUTÁRIA para as operações sujeitas também ao pagamento de ICMS por substituição tributária. É importante frisar, que o Bravo Gestor só disponibiliza o preenchimento dos campos referentes à tributação assinalada no CFOP. Ex: Se o CFOP utilizado no cabeçalho de nota fiscal, não tiver marcado SUBSTITUIÇÃO TRIBUTÁRIA, os campos base de cálculo e valor do ST, passam em branco. Lembrando que é não permitido um CFOP na abertura sem um correspondente em pelo menos um item da nota fiscal.

No caso dos itens da nota fiscal, vale a configuração do CFOP individual de acordo com o destino de cada produto, podendo ser utilizados diversos CFOPs nos itens, o CFOP do cabeçalho seja utilizado ao menos uma vez.

Quando uma nota fiscal possuir nos itens um CFOP de substituição tributária e outro de tributado integralmente como 1403 e 1102, deve-se utilizar no cabeçalho da nota, o de ST, para que sejam disponibilizados, pelo Bravo Gestor, os campos de base ST e valor de ST.

## Lançamento da nota fiscal de entrada

I - de incluir

O sistema fará a pergunta “você possui o XML desta nota fiscal?” Se sim, e a empresa for emitente de NF-e e detentora de certificado digital, será aberta uma pasta onde deverá ser copiado o XML correspondente a essa NF-e. Essa tarefa é necessária, porque é obrigatório, por lei, o armazenamento de todos os arquivos XML correspondentes às NF-e de entrada.

Informe o CFOP de compra, não o de venda do fornecedor.

O campo ST se refere à situação tributária do frete, quando incluso na nota fiscal. Na ausência do frete, quando se referir a um conhecimento de frete deve se preencher o campo com código 90.

Informe o número da nota fiscal, tecle ENTER e abra a lista de modelos indicados para cada tipo de documento ou digite o número, como, 01 para nota fiscal mod. 1A, 55 para NF-e, 08 para conhecimento de frete e assim por diante. O campo seguinte é a série do documento, que deverá ser copiado da nota fiscal, podendo passar em branco no próximo campo que se refere à subsérie.

O campo data de emissão, é a data constante do documento fiscal.

A seguir, informe o código do fornecedor, não tendo em mãos, tecle ENTER e escreva o nome do fornecedor para que seja aberta a lista de nomes. Caso não conste dessa lista, tecle I de inclui sobre ela, que será aberta uma ficha em branco para que seja feito o cadastro. Depois de concluído, tecle ENTER, esse fornecedor terá seus dados lançados na nota fiscal.

O campo CONDIÇÕES DE PAGAMENTO deve ser deixado em branco para pagamento à vista. Sendo a prazo, informe o número de dias como 30, 21/28/35 ou 30/60/90, que o Bravo Gestor criará os documentos de crédito correspondentes. Nota: antes do processamento da nota fiscal, tecle D de duplicatas e acesse os documentos, depois do ENTER e na ficha do documento, pressione A para alterar e complete os dados de cada documento, que depois de concluídos e com ESC, o sistema perguntará se pretende lançar as duplicatas agora. Uma vez confirmadas, essas duplicatas serão gravadas no contas a pagar. Se o pagamento ao fornecedor utilizar cheque a vista ou pré-datado, crie os documentos da mesma forma da condição a prazo e faça a quitação dos documentos com cheque no módulo contas a pagar, informando a data de vencimento do cheque. Aí sua empresa passará a ser devedora dos cheque e não mais dos documentos de créditos.

Os campos seguintes dos valores devem ser preenchidos, rigorosamente de acordo os constantes da nota fiscal, com atenção para as mensagens de alerta pertinentes a integridade dos valores digitados. O campo FRETE deve ser preenchido, mesmo que não seja integrante da nota fiscal, pois servirá para compor as formações de preços dos produtos. No caso do frete incluído na nota fiscal, bem como despesas acessórias e seguro, deverá ser respondida a pergunta se permite a recuperação do ICMS, opção, que só será SIM, para as empresas contribuintes de ICMS pelo sistema de apuração de débito e crédito, à exceção de notas fiscais de produtos isentos, não tributados, ou sujeitos ao regime de substituição tributária.

Nesse caso, se seu contador lançar os valores citados em um CFOP específico, informe esse CFOP no campo CFOP do frete e a alíquota correspondente. Se o campo CFOP for deixado em branco, o valor do frete, e as outras despesas, serão distribuídos, proporcionalmente, em cada CFOP dos produtos correspondentes.

Um detalhe muito importante a ser observado, é que o total dos produtos deve ser líquido, ou seja, a soma dos totais brutos dos itens, já somados com acréscimos ou abatidos os descontos, se houver. Caso a nota fiscal não venha com os valores constituídos dessa forma, deve ser corrigida, aplicando o desconto ao valor informado na nota fiscal, pois o valor total da nota é a soma dos produtos mais todos os outros valores como ICMS ST, frete quando incluso, IPI, despesas acessórias e seguro. No caso de uma NF-e, se preenchida corretamente, essa relação de valores foi modificada, pois, havendo desconto, os valores dos produtos devem vir já líquidos e o destaque do valor do desconto é apenas informativo. Nesse caso, não há necessidade de informar o desconto no ato da entrada da nota fiscal.

No campo OUTROS, devem ser informados quaisquer outros valores, não constantes da nota fiscal, mas que fazem parte do custo total da compra, como descarga, acondicionamento ou pagamentos adicionais ao fornecedor.

O CFOP e a alíquota de ICMS do frete, só são relevantes quando se tratar de frete incluído na nota fiscal e devem ser aplicados sob orientação do responsável técnico pela contabilidade da empresa. Finalmente a opção do frete: 01 ou 02 deve ser a constante da nota fiscal.

Concluída a operação de inclusão dos dados principais da nota fiscal, será aberta, automaticamente, a opção de lançamento do código do produto, que na ausência dele tecla-se ENTER e faz-se a busca pela descrição. Encontrado o produto, confirme com ENTER, para que seja lançado na nota fiscal. Caso o produto não seja encontrado e deseja-se cadastrá-lo, sobre a lista de produtos e já sem a busca ativada, tecla-se a letra F de ficha para abrir uma tela de cadastramento para o novo produto, que depois de concluído o cadastro, tecla-se ESC para sair de uma nova inclusão e outro ESC para posicionar na lista geral de produtos e então tecla-se ENTER para que seja lançado na nota fiscal e assim por diante, até que sejam lançados todos os itens na mesma ordem como estão impressos na nota fiscal.

Seguidos os passos acima, na inclusão do item,informe o CFOP indicado para essa operação de compra, como o destino a que vai ser dado, ou seu enquadramento tributário, como, mercadoria para revenda tributada ou ST, ou mesmo para consumo, situações que o usuário deve ter pleno conhecimento.

!!!
A ordem dos produtos deve ser, rigorosamente, idêntica à impressa na nota fiscal do seu fornecedor. Caso tenha perdido essa ordem, devido a alteração ou exclusão de um item, entre em cada produto, pressione A de alterar e informe a ordem correta. Não pode haver intervalo na ordem dos produtos pois, além de perder a conciliação com as informações da nota fiscal, produz erros na geração dos arquivos do SPED fiscal.
!!!

Informe o CST de acordo com a situação tributária do produto, 000 para tributado integralmente, ou 010 para tributado de ICMS e substituição tributária. Normalmente, quando se trata de mercadoria para revenda, esse CST é idêntico ao informado em cada item da nota fiscal.

Porém, em se tratando de outras operações, como aquisição de materiais para consumo, patrimônio, ou operações nas quais não se aproveita o crédito de ICMS, usa-se o CST 090 (Informações complementares no final desse texto).

O campo, “Embala e desembala” é utilizado para calcular o fator de conversão, quando a unidade de compra (unidade de venda do seu fornecedor), for múltiplo da sua unidade de venda. EX. Se o produto é vendido em UN e na nota fiscal, é oferecido com caixa com 24, com preço de caixa, informe, o tipo de volume, a unidade de compra 24 e unidade de venda 1, que sistema fará o cálculo do estoque e o preço unitário de cada peça.

A quantidade deve ser informada, idêntica, ao que está escrita na nota fiscal, assim como o valor unitário, e se caso o valor total gerado pelo sistema for diferente do nota fiscal, decorrente de algum desconto ou arredondamento, informe esse valor para que ele possa fazer os ajustes necessários.

Deverão ser lançados, do lado direito, os mesmos dados do esquerdo, pois pressupomos nota fiscal integral em suas compras, porém caso não seja, informe as quantidades adquiridas no lado esquerdo e as descritas na nota fiscal no direito. Lembramos, porém, que além de se tratar de uma prática ilícita, o Bravo Gestor não se valerá desses artifícios para compor, corretamente, seus preços de custo.

Nas operações com redução de base de cálculo, como os CSTs 020 ou 070 deve ser informado esse percentual, não havendo, pule com ENTER e informe nos campos correspondentes as alíquotas de impostos constantes da nota fiscal como ICMS e IPI para os tributados integralmente e no caso dos CSTs 010 e 070, serão disponibilizados, além dos tributos citados acima, os campos para lançamento do ICMS de destino, já informado pelo sistema, pressupondo que seja a mesma tributação interna do estado, mas caso não seja, informe alíquota correta para o cálculo. Informe. Finalmente, o MVA (margem de valor agregado) para que seja efetuado o cálculo do ICMS de substituição tributária.

Como se pode notar, o cursor sempre disponibiliza a possibilidade de alteração dos valores gerados a partir dos percentuais informados, para o caso de não se alcançar os mesmos informados na nota fiscal, nesse caso, deve-se fazer as correções necessárias. (Ver informações complementares no final desse texto)

!!!
A Audisoft não se responsabiliza pela orientação nas consultas dos percentuais referentes ao ICMS por substituição tributária e nem no processo de cálculo reverso de percentuais a partir dos valores informados na nota fiscal.
!!!

## Formação de preços

Depois de lançados todos os produtos da nota fiscal, posicione sobre o primeiro item da lista e, sobre a ficha de lançamento, onde estão destacados os tributos, tecle P de preços para acessar a ficha de formação de preços de custo e definição dos preços de venda. A pergunta “atualizar o preço de venda” deve ser respondida SIM, se quiser ter preservada a margem atual praticada nesse produto, então será apresentado o preço de venda sugerido que poderá ser alterado, gerando um percentual de margem correspondente. Se o usuário pretender compor seus preços a partir da sua estrutura de custos operacionais, deve inserir esse dados diretamente, ou por meio de configurações para conhecer seu lucro líquido pretendido. O Bravo Gestor oferece, também, a partir de mudança na configuração, não só a decomposição dos preços de venda para se chegar ao lucro líquido, como a composição das margens de venda a partir de lucro líquido mínimo pretendido. Finalizada a operação, o sistema voltará para o item na nota fiscal. Então pressione seta para baixo e repita a operação e assim sucessivamente até o último item.

Note que, no canto inferior direito da tela de formação de preços, é exibido o preço praticado atualmente para que sirva de referência na formação do preço de venda atual.

Para que seja concluída a inclusão da nota fiscal e os produtos sejam lançados no estoque, deve-se teclar P de processar e responder as perguntas até o final, lembrando que o cursor já está posicionado nas respostas mais recomendadas. No caso de responder NÃO em “atualizar os preços de venda na ficha do produto”, esses preços serão mantidos intactos na tabela de preços e a margem de lucro será atualizada pela proporção entre o novo preço de custo e o preço de venda. Porém, ser for respondido SIM, será atualizado, proporcionalmente, e preço de venda, preservando a margem de lucro atual desse produto. Em ambos os casos os preços de custo serão atualizados INCONDICIONALMENTE.

Nota: na tela principal, onde estão os dados do fornecedor, pode se imprimir vários relatórios, que podem ser consultados na tecla F1, como R de relação em que são listados os produtos para conferência. Nesse mesmo relatório, se a resposta for NÃO, será gerada a relação das mercadorias, com todos os dados da composição dos preços de custo e a sugestão dos preços de venda com base nas margens então aplicadas a cada produto. É recomendável que esse relatório seja emitido antes do processamento da nota fiscal, para que sirva de base na formação dos preços de venda.

Para cancelar uma nota fiscal de entrada, tecle C de cancela e responda as perguntas referentes aos preços. Se quiser voltar aos preços de venda de antes do processamento responda NÃO à pergunta “manter os preços de custo e de venda dos itens dessa nota fiscal”, caso queira mantê-los intactos diga SIM. E então responda a pergunta final da opção de cancelamento. Caso venha processar de novo uma nota fiscal cancelada, atenção para as perguntas sobre preço, nesse caso somente de custo novamente.

ORIGATORIEDADE

Todos os documentos fiscais de aquisição de produtos e serviços sujeitos a tributação do ICMS devem ser lançados para geração dos livros fiscais e Sintegra, como mercadorias para revenda e consumo, telefonia, frete e energia elétrica, tendo o cuidado de informar o CFOP correto e também o tipo de documento, além da série constante no documento. No lançamento do item, a menos que se faça uso crédito de ICMS, fato raro, o CST utilizado deve ser 090. Todos esses serviços devem ser cadastrados como produtos utilizando sempre o CST 090, com descrições sugeridas como: telefone, energia elétrica, frete e consumo.

No caso de consumo, não é necessário o cadastramento de todos os produtos, lança-se um único item chamado consumo com o valor total da nota fiscal.

Ao contrário das mercadorias para revenda, os CFOPs utilizados nessas operações devem conter todas as configurações em BRANCO, a menos que a atividade da empresa permita o aproveitamento do crédito dos impostos.

Tecla F2 - Esse atalho permite o acesso à lista geral de produtos e no caso do faturamento exibe os dois estoques. Teclando F2 sobre um item da nota fiscal, será feita a exibição desse produto na lista geral. Na lista do F2, em qualquer parte do Bravo Gestor, teclando-se F de ficha será exibida a tela do produto, que oferece as mesmas opções do módulo de ESTOQUE, como kardex, fornecedores, depósitos, preços etc.

## CFOP - configurações

Importante: Lembramos que, a recomendação correta sobre qual CFOP deve aplicado a cada operação, deve ser de exclusiva responsabilidade do contador da empresa. Cabe à Audisoft, tão somente fornecer uma lista básica, à qual devem ser acrescentados outros CFOPs na medida em que seu uso for exigido. Caso sejam necessárias mais de uma configuração em um mesmo CFOP, deve se repetir o seu cadastro acrescido de uma variação 1, 2 ou 3 e assim por diante, aplicando os parâmetros necessários como tributação ou movimentação de estoque. Ex. Digamos que o CFOP 5102 está sendo utilizado para vender produtos tributados integralmente, mas que dependendo do cliente, esse mesmo produto deve ser vendido com ICMS diferido. Então, para que seja possível o cadastramento de uma tributação diferenciada na ficha do produto, é necessário que seja cadastrado um novo CFOP 5102-1, ou a variação disponível, desmarcado o destaque do ICMS. É essa variação, que permite várias configurações em mesmo CFOP.

Como foi visto, no Bravo Gestor, os destaques dos impostos nas notas fiscais de saída e as informações fiscais apresentadas no Sintegra ou SPEED, ou as movimentações dos estoques fiscal ou administrativo, dependem das configurações marcadas nos parâmetros do CFOP.

A exemplo disso são as empresas optantes pelo Simples federal, que não podem conceder aos seus clientes o direito a crédito de ICMS E IPI nas operações de venda, e, portanto devem ter essas opções desmarcadas nas configurações dos CFOPs, mas que no caso de uma devolução de compra de mercadorias, em que o fornecedor depende do destaque dos impostos para a recuperação dos mesmos, as configurações devem condizer com essa necessidade.

Outro ponto importante nas configurações dos CFOPs é a baixa ou lançamento do estoque. Nos CFOPs de compra, além dos tributos exigidos nas informações para o Sintegra, no caso de mercadorias para revenda, devem ser marcados movimentação dos estoques administrativo e contábil e, também, financeiro, pois essa opção influencia na composição dos preços de custo e o registro da nota fiscal deve efetuar a entrada dos produtos dos dois estoques.

Para os operações de saída, devem ser marcados os tributos que devem ser destacados na nota fiscal, como ICMS, IPI e ICMS ST. No caso da empresa optante pelo simples, esses tributos devem ser desmarcados, exceto nas operações em que deve destacar o imposto, como devoluções e outras situações específicas. Para efeito de movimentação dos estoques, marca-se, normalmente, apenas o contábil, pois o físico é baixado pela conclusão na pré venda.

## Informações complementares

Com a advento da NF-e 2.0 e o SPED tornou-se obrigatória a inclusão de várias informações, na nota fiscal de entrada, nos mesmos moldes da nota fiscal de saída, que depende das configurações corretas dos NCMs para que sejam aplicados, corretamente, os tributos. Sendo assim, os tributos, IPI, PIS, COFINS, ICMS deverão passar pelo mesmo processo de preenchimento utilizado nas configurações dos NCMs para a nota fiscal de saída.

Após o preenchimento do campo CST, escolha no campo seguinte a definição do enquadramento tributário pertinente a esse produto. Os campos dos tributos devem preenchidos abrindo as listas de opções. Em caso de dúvida, o profissional responsável pela contabilidade da empresa deverá consultado, pois a omissão dos dados ou o seu preenchimento incorreto inviabilizará, completamente, a validação do SPED fiscal e essa informação é de inteira responsabilidade da empresa informante. Porém algumas dicas podem ser úteis. Por exemplo, no caso de uma empresa de comercialização, que não faz uso do crédito de IPI, pode-se escolher opção 04 - entrada imune, o tipo de cálculo - percentual e informar a alíquota, quando houver.

No PIS, caso a nota fiscal do seu fornecedor não venha destacado esse imposto, poderia se utilizar a opção 50 (Operação com direito a crédito), tipo de cálculo percentual e outros campos, aplique os valores informados no XML. Se sua empresa for optante pelo Simples Nacional, a opção recomendada é a 70(Operação de aquisição sem direito a crédito) . Para o COFINS, vale a mesma regra aplicada ao PIS. 

Para os cálculos do ICMS e ICMS-ST, escolha o CST indicado para a operação e a seguir o CSOSN correspondente ou o descrito na nota fiscal se o seu fornecedor for optante pelo Simples Nacional.

No ICMS, a determinação da base de cálculo, com exceção de produtos especiais, como cimento, bebidas e outros, que são tributados sobre pautas, é sempre a opção 3-valor da operação. Esses casos especiais devem ser consultados com o seu contador, seu fornecedor ou o site da Receita Estadual. Informe o percentual de redução da base de cálculo de ICMS e a pauta, quando houver e alíquota de ICMS destacada na nota fiscal.

Se o produto for tributado integralmente apenas de ICMS, passe com ENTER sobre todos os campos abaixo e finalize a inclusão, mas, havendo destaque de ICMS-ST, escolha a opção 4-margem de valor agregado na determinação da BC ICMS ST e informe, a seguir esse percentual. Se houver redução da base de cálculo, informe esse percentual e a seguir o valor da pauta, quando for o caso. Finalmente, informe a alíquota de ICMS-ST, que é a alíquota de destino, nesse caso, o seu estado. Para a maioria dos produtos, em Minas Gerais, é aplicada a alíquota de 18%, exceto produtos com benefícios fiscais específicos.

Nota: Lembramos, novamente, que não se trata de orientação fiscal, que é prerrogativa do contador da sua empresa, e não poderá ser imputada à Audisoft essa responsabilidade, mas um treinamento para uso mais racional na inclusão de dados.

## Conhecimento de frete, energia elétria e telefone

Para lançar um conhecimento de frete é necessário que antes tenha sido cadastrado no estoque um produto com a descrição FRETE e CST 090. Não é necessário informar quantidade em estoque ou preço. Vá agora em Faturamento>notas fisccais>entrada e inclua com o CFOP indicado para esse tipo de documento. Caso esse CFOP ainda não tenha sido cadastrado no Bravo Gestor, vá em Utilitários>CFOP e faça a inclusão deixando em branco todos os parâmetros de tributação e estoque. Preencha os campos dos valores da nota fiscal como qualquer outro produto. Se o frete não for tributado de ICMS informe apenas o valor total do frete nos campos "Produtos e Total da nota" e deixe em "branco" o campo CFOP junto ao transportador e a alíquota deve ser zero. Não deixe de lançar o "produto" frete com quantidade "um" e o valor unitário e total iguais ao valor total informado no conhecimento de frete, aplicando as devidas tributações informadas no conhecimmento. Se sua empresa pretende aproveitar o crédito de ICMS (consulte o seu contador), informe o CST 000 com destaque da alíquota de ICMS, se não, o CST deve ser 090 e a alíquota deve ser zero. Ao final, faça o processamento como uma nota fiscal qualquer de mercadorias. Nota: Essa mesma orientação deve ser aplicada também nas inclusões das notas fiscais de serviço de energia elétrica e telefonia.

# Devolução de compra de mercadorias

A devolução de mercadorias para um fornecedor deverá ser feita diretamente no faturamento na nota fiscal de saída. Insira o CFOP recomendado pela contabilidade e os dados completos do fornecedor. Passe em branco no campo “origem”, pois os itens deverão ser lançados individualmente e diretamente na nota fiscal. Deixe vazios todos os campos de valores, eles serão preenchidos pelo próprio sistema depois de lançados todos os produtos. ATENÇÃO para o detalhe a seguir. Ao incluir um produto na nota fiscal, os valores do IPI, PIS, COFINS e ICMS serão lançados de acordo com as configurações informadas nos NCM/SH para venda. Portanto, para que sejam aplicadas aos produtos as tributações desejadas na nota fiscal de devolução como IPI, ICMS, ICMS-ST, PIS e COFINS, pressione A de alterar sobre o produto já incluído. Entre com ENTER em cada uma dessas tributações e aplique os percentuais corretos para gerar os valores necessários para a impressão correta da nota fiscal. Caso precise de ajuda, ou não chegue aos valores esperados, vá até a tela inicial da nota fiscal e pressione L de lançamento, imprima os tributos lançados e envie ao seu contador ou ao seu fornecedor para que informem corretamente o preenchimento de cada campo. De posse dessa informação, vá novamente aos produtos e faça as correções necessárias e imprima a nota fiscal.

## Devolução de venda de mercadorias

A devolução deve ser feita sobre o pedido de venda. Pressione ENTER sobre a venda para acessar os itens e então pressione D para disponibilizar os produtos para devolução. Os produtos serão exibidos com quantidade zero. Posicione sobre o produto a ser devolvido e pressione ENTER. Se a devolução do item for na quantidade total, confirme com ENTER. Se for parcial, informe a quantidade desejada. Repita essa operação em todos os itens que deseja devolver movendo com a seta do teclado. Lembrando que, os itens já devolvidos não ficam mais disponíveis para uma nova devolução. Depois de incluídos todos os itens na devolução, pressione P de pedido para finalizar e imprimir o documento. As opções dinheiro, abatimento e a creditar, podem ser ignoradas, pois devem ficar a cargo do operador do caixa no ato da confirmação.  Apenas confirme SIM à pergunta e imprima o comprovante. Para ser concluída toda devolução deverá ser confirmada no terminal de caixa, da mesma forma como é confirmada uma venda. Observe que será exibida a letra R no lançamento indicando que é uma devolução. Confirme com ENTER e escolha a opção “Dinheiro”, se for devolver o dinheiro ao cliente. Se a compra foi a prazo e o débito do cliente ainda não foi quitado, escolha a opção “Abatimento” e com ENTER  acesse o documento. Pressione ENTER novamente e informe o valor da devolução no campo desconto. Confirme a operação respondendo SIM à pergunta final. Lembramos que, se a venda foi efetuada com parcelamento no prazo, o valor da devolução poderá ser aplicada em qualquer em qualquer uma das parcelas ou distribuída, proporcionalmente, em todas elas, movendo as setas do teclado para acessar os documentos desejados. Se a venda foi efetuada a prazo, porém já teve os documentos quitados e empresa são deseja devolver o dinheiro, poderá escolher a opção “A creditar”e será lançado um crédito na ficha desse cliente para ser utilizado nas próximas compras. É importante lembrar que uma devolução, depois de confirmada no caixa, não poderá mais ser revertida, podendo, no entanto ser abortada. Para isso basta pressionar E de excluir no caixa.