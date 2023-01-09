# CIAP - Crédito de ICMS de Ativo Permanente

## Emissão de uma NF-e CIAP

Cadastre o CFOP 1604 (Crédito de ICMS relativo a CIAP). No cadastro, delete a opção NORMAL e escolha a opção AJUSTE. Deixe todos os parâmetros em branco e no campo “Observação do lançamento fiscal” informe “Crédito de ICMS relativo à entrada de bem do ativo permanente”. Essa informação será exibida na campo de Observações do SPED fiscal.

Para que saia impressa no DANFE, essa informação deverá ser lançada, também, no campo “Informações complementares”. Em ambos os casos, para salvar o texto da mensagem, pressione Ctrl=W.

Se desejar informar o mês de referência,  ou alguma outra informação, pressione O de observação, antes de imprimir a nota fiscal. Esse campo não precisa ser informado no SPED.

Antes de iniciar a nota fiscal, cadastre, no Estoque, um produto “Ativo permanente – ICMS a ser apropriado”. No campo da unidade(UN), escreva R$, com o CST 090 e o [NCM 00000000](../Estoque/ncm-00000000-uso-generico.md), que deve ter no seu cadastro, as seguintes configurações: IPI 52(tipo de cálculo 0), ICMS 090(determinação da BC ICMS 3), PIS 08 e COFINS 08; todos sem alíquota de imposto, para ser utilizado nesse produto.

Inclua a nota fiscal com o CFOP indicado em nome da própria empresa. Ignore ou escolha qualquer transportador e na opção “Frete por conta”, delete e escolha “Sem frete”

Inclua o produto com quantidade 1(um), e no valor unitário e no total do produto, informe o valor da cota do imposto recomendado pelo seu contador.

Volte à nota fiscal, pressione V de valores e informe o valor do ICMS no campo apropriado e deixe todos os outros campos em branco. Se desejar adicionar alguma informação como, mês de referência, pressione O de Observações. Imprima a nota fiscal, normalmente, e confira se foram impressos os dados corretos.

!!!
Essa operação só pode ser excutada com o acompanhamento do responsável pela contabilidade da sua empresa.   
!!!