# Emitir uma NF-e

Importante: Uma NF-e já enviada à SEFAZ não poderá mais ser alterada ou excluída. Caso ocorra algum problema técnico que impeça a finalização de uma NF-e, solicite, imediatamente, suporte à Audisoft e mantenha na tela a mensagem exibida. A NF-e deve permanecer intacta.

Diante de qualquer dificuldade de impressão de uma NF-e, verifique a disponibilidade do servidor do seu estado. Lembramos que, mesmo com o status positivo, costumam serem necessários no mínimo dez minutos para o serviço estar, totalmente, acessível. Acesse o link abaixo:

[http://www.nfe.fazenda.gov.br/portal/disponibilidade.aspx?versao=2.00&tipoConteudo=Skeuqr8PQBY=](http://www.nfe.fazenda.gov.br/portal/disponibilidade.aspx?versao=2.00&tipoConteudo=Skeuqr8PQBY=)

Certifique-se de que todos os produtos possuem um NCM/SH com as configurações de tributação corretamente cadastradas para as operações de venda.

Acesse Faturamento>notas fiscais>saídas. Escolha o modelo 55 e pressione ENTER e será aberta a última nota fiscal impressa. Pressione I para incluir e informe o CFOP, de acordo com a orientação da sua contabilidade. Informe em “ORIGEM” o número do pedido de venda, e todas as informações necessárias, inclusive as tributações dos produtos serão capturados, automaticamente. Pressione ESC para sair da lista de produtos e verifique se os dados do destinatário estão corretos. Nenhum campo poderá ficar vazio, sob pena de ter a validação rejeitada pela SEFAZ.

Para emitir uma nota fiscal de cobertura de um cupom fiscal, faça uma busca na pré-venda pelo número do COO impresso na parte superior do cupom fiscal e identifique o número do pedido correspondente. Informe esse número do pedido no campo ORIGEM da nota fiscal

Se a opção de frete for por conta do destinatário ou de terceiros, os dados do transportador devem ser informados na íntegra. Para isso pressione T para incluir essas informações, inclusive os dados do carregamento, como volumes e peso. O campo CFOP do frete só deverá ser preenchido se esse valor for incluso na nota fiscal.

Para incluir uma observação, pressione O, digite o texto, salve com Crtl+W e preencha os dados do empenho, se essa nota fiscal for destinada a um órgão público, se não, passe com em todos os campos e confirme a pergunta final.

Se a nota fiscal NÃO for originada de um pedido de venda, como devoluções de compra ou de venda, remessas, etc; todas as informações deverão ser lançadas, manualmente. Nesse caso, passe em branco pelo campo “origem”.  Se tiver o código do cliente, informe. Se não, pressione ENTER e digite o nome no campo seguinte e será aberta lista dos clientes cadastrados no contas a receber. Selecione e confirme. Os passos seguintes são idênticos ao modelo anterior. Nesse caso, quando finalizar a inclusão do destinatário, será aberta a opção para incluir os produtos. Se tiver o código do produto, informe. Ou pressione ENTER e busque na lista pela descrição. Confirme com ENTER e não esqueça que os CFOPs dos produtos não podem ser, totalmente, diferentes do informado na abertura da nota fiscal.

Como foi salientado no manual de devolução de compra de mercadorias, as tributações dos produtos serão lançadas como foram configuradas para VENDA. Se desejar uma tributação diferente, pressione A, sobre o produto, já lançado e faça as alterações necessárias, entrando nas informações de cada tributo, conforme orientação da sua contabilidade.

Antes de  pressionar N para impressão da NF-e, certifique de que sua internet está funcionando  e que o servidor da SEFAZ está disponível e operante. Do contrário, aguarde.

Os erros mais comuns, que impedem a emissão de uma NF-e, são: certificado digital vencido ou não instalado, tributação incorreta ou incompleta nas configurações do [NCM/SH](../Estoque/cadastro-de-ncm.md), ausência do número no campo endereço, dados incompletos do transportador quando a opção for entrega pelo emitente ou terceiros, valor negativo no ICMS retido para produtos com CST 060(vicmsret), código de barras inválido na ficha do produto e falha na conexão com o servidor da SEFAZ.  Outro erro comum é causado pelo certificado digital vencido e exibe a mensagem “XML mal formado”.  Para conferir, abra seu Internet Explorer e vá em Ferramentas>opções de internet>conteúdo>certificados e veja se existe um certificado e se a sua data de vencimento não está expirada. Adquira um novo certificado e antes da sua instalação, delete o antigo. Veja [AQUI](como-instalar-um-certificado-digital.md) como instalar.

Antes da impressão do DANFE, faça uma revisão geral em todos os campos, principalmente, dos valores esperados. Para saber que informações foram utilizadas para se chegar a esses cálculos, pressione L de lançamento sobre a tela de entrada da nota fiscal onde estão os dados do destinatário e imprima os detalhes de todas as tributações aplicadas e faça as devidas correções.

Para imprimir o DANFE, pressione N e será aberta a lista dos produtos. Pressione ENTER e confirme o processamento do estoque. Confirme se o número da NF-e informado é o mesmo o que pretende imprimir. Em relação à data de saída das mercadorias podem ser utilizadas 03 opções. A) Confirmar a data informada . B) Informar outra data. C) Deixar a data em branco para ser preenchida manualmente. Para as duas últimas opções, responda NÃO para a confirmação da data e informe a nova data desejada ou delete se pretende deixar em branco. O DANFE será impresso na impressora instalada como padrão.

Se o e-mail do seu cliente constar do cadastro, o XML será enviado automaticamente. Caso queira enviar para outro endereço, informe no campo apropriado que será exibido ao fechar o formulário do DANFE. Um DANFE pode ser impresso quantas vezes desejar, assim como o XML pode reenviado sempre que for necessário. Basta pressionar N sobre uma NF-e já impressa.

O suporte Audisoft se limita a questões técnicas. Todas as questões fiscais e tributárias devem ser encaminhadas ao setor de contabilidade da empresa.