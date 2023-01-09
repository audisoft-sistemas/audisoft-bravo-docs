# Vendedores

 
## Cadastro de vendedores

Conhecimento necessário: Módulo de Usuários

Acesse `Staff500>Vendedores`

Somente depois de cadastrado no módulo de USUÁRIOS, o operador poderá ser cadastrado como vendedor. Acesse Staff500>Vendedores, pressione ENTER e pressione I para incluir um novo vendedor. Informe o nome do vendedor, o código que lhe foi atribuído como usuário e o código de vendedor (é recomendável que se use o mesmo código). Informe a região à qual deve estar vinculado. O padrão é sempre LOJA. Se a empresa possui outras regiões com tabelas de preços diferenciadas, deve escolher a região adequada ao vendedor. O campo “comissão” só deverá ser preenchido se esse vendedor receber comissão com percentual único para qualquer modalidade de venda, pois serão ignorados quaisquer outros parâmetros. O campo “indexador” é utilizado quando se pretende aplicar sobre as comissões desse vendedor um indexador de acréscimo ou redução sobre as configurações gerais de geração de comissões.
Para cadastrar as rotas de atendimento, ainda na ficha do vendedor, pressione R para exibir as rotas existentes e I para incluir uma nova rota. Defina nomes de fácil identificação como dias da semana, bairro, cidade ou micro região. Após cadastrar as rotas, pressione ENTER sobre qualquer uma para visualizar a lista de clientes. Para cadastrar um cliente em uma rota, pressione I para incluir e será aberta a lista de todos os clientes que, em sua ficha de cadastro tenham sido informados o vendedor e a região aos quais está vinculado. Isso garantirá a emissão de relatórios de orientação de visitas a clientes externos para venda ou cobrança.

---
## Prepostos

Acesse `Staff500>Prepostos`

Apesar de exercerem um papel indireto das vendas, muitas empresas procuram manter os cadastros atualizados desses profissionais (ex: engenheiros, eletricistas, pintores, arquitetos etc.), para gerenciar sua capacidade de persuasão nas vendas e gerenciar o pagamento de premiações, bônus e comissões. O seu cadastro segue, basicamente, os mesmos critérios de um vendedor.

---
## Regiões

Acesse `Staff500>Regiões`

Uma região pode representar uma área territorial de atuação da empresa, um segmento de mercado ou uma opção na prática de preços diferenciados dentro da própria loja. Note que a região LOJA possui um fator de preços 100. Isso que dizer que, os preços exibidos em sua tabela são idênticos aos informados na ficha do produto, e os percentuais de comissão e descontos a vista e a prazo com valor zero significa que as condições de venda e comissão são as mesmas informadas nos parâmetros gerais. Sendo assim, caso a empresa possua um segmento em que pretenda praticar preços majorados em 5% nos produtos vendidos na loja, crie uma região e no fator “preços” informe 105. Quando o vendedor que tiver o seu cadastro vinculado a essa região acessar a tabela de preços, efetuar uma venda ou um orçamento terá todos os preços majorados em 5%. Poderão também ser criadas tabelas especiais em qualquer região. Basta pressionar T de tabela e com L de lançar ou I de incluir, informar os produtos com os preços a serem praticados nas vendas.

---
## Tabela Promocional

Acesse `Staff500>Regiões`

As tabelas de preços promocionais podem ser criadas em qualquer região, para isso pressione P de promoção na região desejada e inclua um nome para essa promoção e marque sempre NÃO para as opções: flutuante e a prazo, já que uma promoção não poderá sofrer variações nos preços, pois a tabela já foi divulgada e informe a data em que deverá entrar em vigor e a em que deverá expirar. Pressione ENTER sobre a tabela criada para incluir os produtos e pressione I de incluir. Selecione o produto, informe a quantidade a partir da qual o preço promocional informado será aplicado (o mesmo produto poderá ser lançado mais de uma vez na mesma tabela promocional se forem oferecidos preços diferenciados para quantidades mínimas distintas). Finalmente, informe o preço desejado. Os preços promocionais dos produtos passam a vigorar na primeira hora do dia informado para início e expiram na última hora do dia informado para fim, ou também com a exclusão da tabela promocional.

## Relatórios

### Relatório resumido de vendas por forma de pagamento

`Vendedores>Relatórios>Vendas>Periódico>Resumo`

--- 

### Relatório detalhado de vendas diárias a vista, a prazo, devoluções e prazo médio

`Vendedores>Relatórios>Vendas>Periódicos>Detalhado`

---

- Relatórios de vendas analítico com vendas emitidas e faturadas, a vista, a prazo, devoluções, condicionais e orçamentos.  

`Vendedores>Relatórios>Vendas>Periódicos>Analítico`

---

### Relatório de CMV (Custo das Mercadorias Vendidas)

`Vendedores>Relatórios>Vendas>Periódicas>CMV`

---

### Relatório da curva ABC de produtos

`Vendedores>Relatórios>Vendas>Produtos>Movimentação>Participação ABC`

---

### Relatório de movimentação de produtos orçados, vendidos, reservados ou devolvidos. 

`Vendedores>Relatórios>Vendas>Produtos>Movimentação>Produtos`

Marque com X a opção desejada. Se desejar listar todos os produtos, incluindo os pedidos ainda não confirmados no CAIXA, apague a palavra CAIXA e escolha PRÉ-VENDA 

---

### Relatório detalhado de comissões dos produtos vendidos

`Vendedores>Relatórios>Vendas>Produtos>Movimentação>Comissão`

---

### Relatório das margens de lucro e participação dos grupos e subgrupos.

`Vendedores>Relatórios>Vendas>Produtos>Margem de lucro`
    
Mande processar o período desejado e, sem sair do menu, escolha com seta para baixo a opção “sintético”. Responda SIM para impressão resumida da lucratividade das famílias e escolha se quer detalhada por subgrupos ou grupos.

---

### Relatório da curva ABC de clientes

`Vendedores>Relatórios>Vendas>Produtos>Quebra no preço>Processar`
    
Processe o período desejado e escolha abaixo Clientes ABC.

---

### Relatório de quebra no preço de venda

`Vendedores>Relatórios>Vendas>Quebra no preço>Processar`

Após o processamento, escolha a opção “Quebra produtos” para ver os descontos concedidos em todos os produtos vendidos no período. Para ver todos os descontos concedidos por vendedor ou formas de pagamento, pressione ENTER sobre “Quebra preço” e escolha a opção desejada.

---

### Relatório detalhado das vendas, clientes e condições de pagamento.

`Vendedores>Relatórios>Vendas>Controle>Controle`

Esse relatório é muito utilizado para conciliar informações sobre as vendas que tenham gerado dúvidas no fechamento diário do caixa. Responda NÃO, se não for para manifesto de carga.

---

### Relatório periódico de orçamentos, reservas, vendas e devoluções.

`Vendedores>Relatórios>Vendas>Controle>Pedidos`

Escolha o filtro, se desejar e marque com X a opção que pretende imprimir.

---

### Relatório do extrato das comissões de um vendedor

`Relatórios>Vendedores>extrato`
    
Esses relatórios podem ser analíticos ou sintéticos. Os extratos são individuais por vendedor.
Acesse e escolha uma das opções:
- Geradas (todas as comissões as geradas no período)
- Disponíveis (prontas para pagamento se o crédito das comissões for ao recebimento das vendas a prazo)
- Baixadas (todas as comissões quitadas) ou pendentes (quando as vendas ainda não foram quitadas pelo cliente nas modalidades de comissões no recebimento.

---

### Relatório de desempenho de vendedores

`Vendedores>Relatórios>Vendedores>desempenho`

- Orçamento
- Aproveitamento
- Quebra na venda
- Participação.

---

### Relatório das comissões geradas, disponíveis, baixadas e pendentes.

`Vendedores>Relatórios>Vendedores>Comissões`

Acesse e escolha uma das opções:
- Geradas (todas as comissões as geradas no período)
- Disponíveis (prontas para pagamento se o crédito das comissões for ao recebimento das vendas a prazo)
- Baixadas (todas as comissões quitadas)
- Pendentes (quando as vendas ainda não foram quitadas pelo cliente nas modalidades de comissões no recebimento.
Esse deve ser o único relatório utilizado para apuração das comissões dos vendedores. Em caso de questionamento, imprima o extrato do vendedor, de preferência analítico.

---

## Utilitários

No menu de Utilitários, estão as principais configurações das condições de vendas, comissões e segurança do Staff500.

### Parâmetros de vendas

#### Tabela de promoção fixa.

- SIM: mantém os preços promocionais fixos mesmo com as mudanças dos preços da ficha do produto.
- NÃO: varia os preços promocionais, proporcionalmente, conforme variam os preços da ficha do produto.

---

#### Comissão no faturamento

- SIM: o sistema disponibiliza, para pagamento ao vendedor, as comissões no ato do fechamento das vendas.
- NÃO: as comissões só são disponibilizadas, para pagamento, no ato recebimento das vendas a prazo ou da liquidação dos cheques.

---

#### Comissão a vista e a prazo.

Quando a opção de pagamento das comissões é no FATURAMENTO, o percentual de comissão para vendas a vista e a prazo costumam ser diferentes. Do contrário, costumam ser iguais.

---

#### Encargos sobre comissões.

Essa configuração define o custo adicional da empresa sobre as comissões dos vendedores decorrente dos encargos trabalhistas

---

#### Preposto único/código.

A configuração original pressupõe que empresa não trabalha com prepostos. Caso contrário, deixe as duas opções em branco para que o vendedor seja forçado a escolher na lista, o preposto a que essa venda deverá ser vinculada.

---

#### Formulário de pedido.

O Staff500 oferece vários formulários de pedido. Caso o usuário queiro optar por um modelo diferente do formato VAREJO, delete e escolha o modelo desejado.

---

#### Impressão em ordem alfabética.

Marcando X com a barra de espaço, os itens incluídos na pré-venda serão impressos na ordem alfabética. Desmarcando, a impressão será na mesma ordem em que foram incluídos.

---

#### Validade do pedido.

Define o prazo limite para garantia dos preços do orçamento, mesmo havendo alteração dos preços da tabela.

---

#### Validade da entrega.

Define a data limite para a retirada ou entrega do pedido.

---

#### Exibir estoque na lista.

O usuário pode decidir se exibe o estoque dos produtos na lista F2, na pré venda ou caixa.

---

#### Usar senha simples.

Marcando X com a barra de espaço, o usuário poderá digitar a senha como foi cadastrada. Se deixar em branco, deverá usar as teclas numéricas informadas nos boxes, pois a senha passará a ser randômica.

---

#### Usar expedição.

Com essa opção marcada, todas as mercadorias ficam aguardando para serem liberadas pela expedição após a confirmação das vendas.

---

#### Grupo.

Pressione ENTER para abrir. Essa opção possibilita configurações especiais nos grupos ou subgrupos como, margem de lucro, comissão a vista e a prazo, custo fixo e desconto máximo a vista ou a prazo. Essas configurações obedecem à prioridade em uma escala descendente. As configurações de um subgrupo prevalecem sobre as do seu grupo e esse, sobre a configuração geral. Durante a alteração, se responder NÃO às perguntas, ao passar pelos campos com zero, significa que, estará respeitando a configuração do seu nível ascendente. Se informar um valor, ou confirmar SIM com zero, estará definindo essa condição como principal.

---

#### Produto.

Pressione ENTER para abrir. Ao ser incluído nessa lista, um produto terá suas configurações respeitadas com prioridade absoluta sobre qualquer outra, como, comissão a vista e a prazo e desconto máximo a vista e a prazo.

---

#### Cancelamento.

Limita o número de dias de permissão para cancelamento de uma venda. Na tentativa de cancelamento de uma venda com data de emissão anterior ao informado nessa configuração, será exibida a mensagem “Essa venda deverá ser devolvida”.

---

#### Avanço.

Determina o número de linhas de avanço da impressora para corte do papel do pedido de venda.
