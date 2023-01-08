# Restrições na pré-venda

- **Desconto não permitido**: Sempre que for aplicado um desconto superior ao informado no parâmetro Estoque>configurações>parâmetros>desconto a vista ou desconto especial a vista e desconto especial a prazo.

- **Cliente em atraso**: Quando o tiver algum título com dias de atraso superior ao definido nos parâmetros. Contas  receber>utilitários>alterar parâmetros>atraso

- **Prazo superior ao definido na tabela**: Quando o prazo concedido na venda for superior ao definido no parâmetro Estoque>configurações>parâmetros>prazo médio de venda. Permite atualizar os preços ou não dependendo das permissões do usuário.

- **Cliente inativo**: Solicita a atualização dos dados na ficha cadastral do cliente se sua última compra for anterior ao período definido no parâmetro Contas a receber>utilitários>alterar parâmetro>inatividade

- **Limite de crédito mensal excedido**: Quando a soma da venda e os débitos desse cliente exceder o limite de crédito mensal informado no parâmetro Contas a receber>clientes>ficha do cliente>limite mensal

- **Limite total de crédito excedido**: Quando a soma da venda e os todos débitos desse cliente exceder o limite de crédito total informado no parâmetro Contas a receber>clientes>ficha do cliente>limite total.

- **Venda a prazo somente com cheque pré-datado**: Quando é feita uma tentativa de venda a prazo ainda não cadastrado no contas a receber>clientes

- **Pedido já disponível no terminal de caixa**: Ocorre em qualquer tentativa de alteração de uma venda já enviada ao caixa. Se a venda foi enviada, indevidamente, ao caixa, faça sua exclusão na movimentação do caixa e será convertida em orçamento para as devidas correções.

- **Estoque insuficiente. Retornar a quantidade disponível.**: Sempre que a quantidade vendida de um produto for superior ao estoque disponível o usuário deve decidir se essa venda é para entrega futura. Essa operação pode ser bloqueada pelo nível de permissão do usuário

- **Cliente no SPC**: Sempre que constar em "Informações financeiras" na ficha do cliente, cheque ou documento enviado ao SPC. A liberação só possível após a quitação desses documentos.

- **Cheque devolvido**: Sempre que houver um cheque devolvido vinculado ao CPF desse cliente, como emitente ou responsável. A liberação pode ser feita com a senha de um avalista, ou quando o cheque for retirado da lista negra, após sua liquidação.

- **Data limite para cancelamento excedida**: Sempre que for feita uma tentativa de cancelamento de uma pré venda com data anterior ao número de dias determinado nos parâmetros Vendedores>utilitários>parâmetros de venda>dias.