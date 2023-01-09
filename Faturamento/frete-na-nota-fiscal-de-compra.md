# Frete na nota fiscal de compra

Sempre que houver cobrança de frete relativo a uma nota fiscal de compra, esse valor deverá ser informado no campo `Frete`. Responda, corretamente, a pergunta `Frete incluso na nota fiscal?`, que deverá ser SIM, somente quando o frete vier destacado na nota fiscal e fizer parte do valor total da mesma. Em ambos os casos, o valor do frete deverá compor a formação dos preços dos produtos constantes da nota fiscal.

!!!
Para  que o valor do frete seja aplicado na composição dos preços, depois de importado o XML, é necessário que se pressione A para alterar na ficha de lançamento em CADA produto e, sobre o campo `Frete` informar se o valor do frete é rateado por valor ou manual.
!!!

Se a opção for valor,  o frete será aplicado, proporcionalmente, em cada produto confirmado. Se for manual, poderá ser informado o valor do frete para cada unidade desse produto como nos casos de frete peso em que o frete costuma ser diferenciado por produto. Depois de confirmado o campo "Frete", pressione Page-down e confirme a pergunta.

Somente assim os valores e os tributos dos itens poderão ser conciliados com os valores informados nos totais da nota fiscal. Enquanto for exibida qualquer mensagem de inconsistência desses valores, a nota fiscal não poderá ser processada, pois produzirá críticas nos arquivos do Sintegra e do SPED.