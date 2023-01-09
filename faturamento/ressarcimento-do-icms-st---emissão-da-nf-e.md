# Ressarcimento do ICMS/ST – emissão da NF-e

Antes de emitir a nota fiscal para ressarcimento do ICMS/ST, consulte o seu contador ou a SEFAZ da sua jurisdição. Confirmada a legalidade e o direito à recuperação desse tributo, emita a nota fiscal vinculada à nota fiscal de devolução em nome do seu fornecedor.

Verifique em Faturamento>Utilitários>CFOP se o CFOP 5603 ou 6603 está cadastrado corretamente. Caso contrário, pressione I para incluir e informe o CFOP desejado. Na natureza, informe, Ressarcimento de ICMS. Em Finalidade, delete o campo Normal e escolha AJUSTE. Marque nos parâmetros, somente, o campo Tributado ICMS.

Cadastre no módulo Estoque, um produto com o nome “Ressarcimento de ICMS retido por substituição tributária” com o CST 090 e o NCM 00.
Veja [AQUI](../Estoque/ncm-00000000-uso-generico.md) o modelo de cadastro do NCM.

Inclua a nota fiscal, com o CFOP indicado, em nome do seu fornecedor. Nos dados do transportador, escolha a opção “Sem frete”. Inclua o produto “Ressarcimento de ICMS” lembrando de aplicar no produto o mesmo CFOP da nota. Informe 01 unidade do produto e no valor unitário, o total do ICMS a ser ressarcido.

Depois de lançado o item na nota, volte à tela principal e pressione V. Informe, no campo próprio, os valores da base de cálculo e do ICMS/ST, repita o valor do ST no campo Produtos para que o valor do imposto seja exibido no total da nota. Esses valores serão aplicados, automaticamente, no campo "Dados adicionais" junto à observação obrigatória.

Antes de imprimir, pressione O, para informar no campo de “Dados Adicionais”, os termos do regulamento do ICMS definidos por lei.

Para relacionar a nota fiscal do seu fornecedor, pressione R de relacionar e em seguida, I para incluir a informação. Pressione ENTER e escolha 55. Informe a chave da nota de devolução emitida para seu fornecedor.

Caso tenha dúvidas, antes da impressão definitiva, gere uma prévia dessa nota fiscal, pressionando P.

Finalmente, pressione N para imprimir.