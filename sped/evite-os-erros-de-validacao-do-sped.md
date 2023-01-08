# Evite os erros de validação do SPED.

A quase totalidade das críticas apresentadas na validação do SPED são referente às notas fiscais de entrada, que podem ser solucionados com as recomendações abaixo.

## Cadastros de NCM/SH (saídas)

As tributações informadas nos cadastros de NCM/SH se aplicam, exclusivamente, à SAÍDA. Muita atenção na escolha do Código da Situação Tributária dos tributos IPI, pois de 00 a 49 se refere  às SAÍDAS entradas e de 50 a 99 se refere às ENTRADAS. Enquanto nos tributos de PIS e COFINS essa ordem é invertida. As posições 01 a 49 se referem às SAÍDAS e de 50 a 99, às ENTRADAS.

## Notas de compra (entrada)

Depois da importação do XML, substitua as tributações do seu fornecedor pelas suas tributações de entrada de acordo com o destino das mercadorias, como revenda, indstrialização, consumo, patrimônio etc. Utilize o CFOp indicado para cada operação. Mantenha o CST de ICMS e aplique os CST de IPI, PIS E COFINS corretos para a operação de entrada.

Regras de tributação: Para evitar os erros de validação do SPED.

- Nunca informe numa operação de compra um CFOP de venda, ou o  contrário.

- Substitua a Situação Tributária do IPI, PIS e COFINS pelo código correto de entrada, observando a lista disponível. EX: Nunca utilize o CST 01 de PIS e COFINS  nunca entrada, nem o 50 numa saída.

- Confira as alíquotas de PIS e COFINS. Se o CST utilizado for tributado, como o 50, as alíquotas deverão ser informadas, mesmo que o fornecedor não as tenha destacado.

