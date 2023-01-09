# Creditamento do imposto pago antecipadamente na compra de arroz (Lucro Real - MG).

!!!
Legislação aplicável no estado de MG para as empresas enquadradas no Lucro Real
!!!

Para obter o crédito do imposto pago antecipadamente na compra de arroz deverá ser emitida e escriturada uma nota fiscal, em nome da própria empresa, destinada a esse fim.

a. CFOP - 1949 ou 2949 Caso esse cfop já esteja cadastrado ou utilizado no sistema, cadastre novamente acrescentando uma variação. Ex: 19491, 19492 etc. Na natureza, informe: Antecipação do ICMS - Arroz. Na finalidade, informe: Ajuste. Nos parâmetros, deixe marcados somente, Tributado de ICMS e FInanceiro. 

b. NCM/SH - Cadastre um ncm/sh com o código 99 com as seguinte configurações. IPI 52, ICMS 090, PIS e COFINS 08, todos com alíquotas ZERO. Siga esse [modelo](../Estoque/ncm-00000000-uso-generico.md).

c. Produto - Cadastre um produto chamado "Antecipação do ICMS - Recebimento de Arroz" com a mesma tributacão e vinculado ao ncm/sh 99.

## Emitindo a nota fiscal:

- Informe o cfop configurado para esse fim.
- Informe os dados da sua própria empresa.
- No campo Frete por conta, informe Sem frete.
- Inclua o produto "Antecipação do ICMS - aquisição\recebimento de Arroz" informando o cfop corretamente. Informe a - quantidade UM e no valor unitário, o valor do imposto.
- Volte à tela principal da nota e presione V de valores para informar o valor do imposto no campo ICMS. 
- Para para referenciar a nota fiscal, pressione R e em seguida I para incluir. Pressione Enter e escolha o modelo 55.
- Informe a chave da nota fiscal do fornecedor.
- Finalmente pressione O e faça a citação legal que será impressa no campo Dados adicionais.
- Antes de imprimir pressione P para visualizar a prévia e conferir se está OK. Se sim, imprima a nota fiscal pressionando N.