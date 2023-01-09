# Cadastro de produtos
Para cadastrar um produto, existem duas maneiras:

Diretamente no estoque:
Acesse Bravo Gestor, Estoque e, depois de informar o usuário e senha, quando houver, siga com ENTER, escolhendo a primeira opção dos menus, até acessar a lista de produtos. Tecle ENTER para que seja aberta uma ficha qualquer de produto. 
Cadastramento em linha, através da lista de produtos (F2):
Tecle F2, escolha o produto e tecle F para acessar a ficha.

Tecle I para incluir e um código interno será gerado, automaticamente, pelo sistema, ou informe um código próprio da sua preferência. Caso a empresa utilize o sistema de endereçamento de produtos, informe esse endereço no campo LOCAL, se não passe com ENTER e informe a unidade de venda do produto: UN, M3, KG, etc. Os dois campos seguintes se referem ao sistema de embalagem utilizado pela empresa. Ex. se a empresa comercializa o produto acondicionado em embalagens de 30 unidades, e quer que seja informado na nota fiscal um volume para cada 30 unidades vendidas, informe no primeiro campo, o número de unidades para cada volume e em seguida, repita a unidade de venda utilizada.

O campo CST é o código da situação tributária utilizado para a venda desse produto na impressora fiscal.

Pode ser digitado diretamente, ou escolhido dentro da lista aberta com ENTER. Pode se notar que ao escolher um CST tributado, deverá ser informado o ICMS, cujas alíquotas deverão ser ordenadas na mesma seqüência em que foram cadastradas no ECF. Normalmente a Audisoft disponibiliza as quatro principais alíquotas na ordem cujas alíquotas 01-07%, 02-12%, 03-18% e 04-25% que são as mesmas mais utilizadas pelos interventores nas impressoras fiscais. Porém, havendo necessidade de outras, acesse o módulo Estoque > Configurações > Tributação e inclua essa tributação depois de tê-la cadastrado no ECF. Para saber a ordem das alíquotas, imprima uma leitura X e confira. Em nenhuma hipótese, um produto poderá ser cadastrado sem uma alíquota cadastrada no ECF, sob pena de ter sua venda recusada pelo caixa.

Ex: Se um produto possui um CST 000(nacional tributado integralmente) e alíquota de ICMS de18%, ficará 000-03, obrigatoriamente. Se o CST for 060, deve ser informada a opção FF, ficando 060-FF e assim por diante.

Lembramos, no entanto, que essas informações fiscais só devem ser cadastradas sob orientação do contador da empresa e a Audisoft estará isenta de qualquer responsabilidade nesse sentido.

O campo código de fábrica deve ser utilizado se a empresa utilizar o número de referência do fabricante ou código especial interno para busca do produto.

Os campos tamanho e cor só são utilizados por empresas que agrupam suas mercadorias por grade de produtos, como sapatarias e lojas de confecções.

O campo NCM/SH só aceita o preenchimento manual se o código já tiver sido cadastrado em Estoque > Configurações > NCM/SH. Conhecidos, também como nomenclaturas, esses códigos são compostos de oito dígitos e indicam famílias de mercadorias e as tributações a que estão sujeitas como IPI, ICMS, ISSQN, PIS e COFINS e só podem ser cadastrados e configurados com o acompanhamento presencial do responsável pela contabilidade da empresa. Sempre que for informado, nesse campo, um NCM ainda não cadastrado, será aberta a lista de cadastro para busca ou inclusão. [Pressione I para incluir e siga todos os passos do cadastro](Cuidados-no-cadastro-de-NCM.md).

Produto é a descrição básica da mercadoria como é conhecida para venda.  

Barras é o código de barras identificado no produto ou em sua embalagem individual. Se o produto não possui o código de barras do fabricante, responda NÃO à pergunta para que seja um código simulado. Lembrando que esse produto será enviado com código em branco à nota fiscal eletrônica.

No campo “especificação” pode-se incluir dados adicionais como: cor, bitola, modelo etc. A propósito, uma particularidade muito útil no Bravo Gestor é a possibilidade ordenação das bitolas em polegadas desde que cadastre corretamente, do tipo: 3/16”, l/4”, ½”, ¾”(muito usado em brocas, ferros de construção e conexões roscáveis) ou mesmo bitolas combinadas como ¼”x2”, 3/16”x5” (muito usado em parafusos franceses). Se o campo especificação for deixado em branco será feita a pergunta “esse produto exige uma especificação?”. Se não, passe em branco, se sim confirme sim e esse produto ao ser vendido obrigará ao vendedor a adicionar informações complementares, como cor da tinta, ou número do serial.  Ao ser digitada uma marca, o sistema checará o cadastro e não havendo, perguntará se pretende fazê-lo agora. O cadastro das marcas poderá ser feito, também, previamente, em Estoque > Estoque > Marcas.

No campo “subgrupo”, caso os grupos e os subgrupos já tenham sido cadastrados, tecle ENTER para abrir o grupo e os subgrupos devem ser selecionados com seta para a direita e confirmados com ENTER. Lembramos que, não é possível o cadastro de um produto sem o cadastro prévio do seu grupo e subgrupo.

Nesse caso será mostrado, detalhadamente, como deve ser feito esse [cadastro de famílias de produto](familias-de-produtos.md).

Acesso o módulo Estoque > Estoque > Grupos, abra a lista com ENTER, e tecle I de inclui e informe o nome do grupo. Por ex. elétrico, hidráulico, genérico, masculino etc., e confirme com ENTER todos os campos de configurações especiais seguintes, caso tenha. Lembrando que, todas as configurações especiais se sobrepõem às gerais, como descontos, comissões etc.

Para cadastrar os subgrupos ou famílias em grupo ainda sem subgrupo, tecle sobre ele F de filho e informe o nome do subgrupo, como fios, tubos, antibióticos, calças etc. e, nos mesmos moldes dos grupos, confirme as configurações desejadas e assim sucessivamente. Se pretender acrescentar um subgrupo a uma família já existente, tecle I de inclui sobre a lista e prossiga com o cadastro.

Note que, o Bravo Gestor possui uma árvore infinita de famílias, podendo ser criada qualquer quantidade desejada de famílias e subfamílias necessárias para o agrupamento refinado dos produtos de acordo com as necessidades peculiares de cada empresa.

Para aplicar o fornecedor, tecle ENTER e escolha na lista. Caso o fornecedor não seja cadastrado, sobre essa lista pressione a tecla I para incluir, informe todos os dados solicitados e confirme a inclusão. O fornecedor poderá também ser cadastrado, previamente em Contas a pagar > Fornecedores.

Caso queira, poderá ser informado o preço de venda, porém o preço de custo deverá ser informado através de P de precificação, onde poderão ser formados os preços de custo e de venda. O preço de custo médio é calculado pela média ponderada das quantidade de compra e estoque e, caso seu cálculo for contaminado por um lançamento errado, deve-se fazer a correção manual.

A venda mínima, que informamos é 01, podendo, no entanto ser adequada à necessidade de cada produto. Ex.: se um piso só pode ser vendido em caixa de 02 metros, informe 02, se o preço for de metro. Se um prego só pode se vendido de 100 em 100 gramas, informe 0,100, se o preço de for em Kg. Se é permitida a venda de qualquer fração, informe 0,001, como é o caso de produtos de balança.

A quantidade do estoque, também só poderá ser informada através da [conferência](conferencia-de-estoque.md), que é tratada em um capítulo específico.

A inclusão só é concluída após responder SIM, à pergunta final.