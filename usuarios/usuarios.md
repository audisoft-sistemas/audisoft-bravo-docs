# Usuários

O sistema de gerenciamento de usuários do Staff500 é muito amigável e fácil de usar. 
Foi criado para ser utilizado pelo próprio cliente e as configurações de restrições e níveis de acesso devem refletir a real função, dentro da empresa, de cada operador.

Alguns detalhes importantes devem ser observados para que os cadastros sejam feitos corretamente.

Observações

- O sistema possui dois níveis de acesso. O nível “1” tem acesso restrito e deve ter suas permissões definidas dentro das chaves de acesso. O nível “9” possui acesso irrestrito, e não depende das definições de atribuições e só pode ser usado pelo administrador da empresa, pois dá poderes absolutos ao usuário.
- Todo vendedor só terá seu cadastro aceito depois de ter sido cadastrado como usuário, pois esse código será solicitado no ato da sua inclusão no módulo de vendedores. O usuário não vendedor pode efetuar vendas, se tiver permissão, porém deverá escolher o vendedor ao qual será atribuída essa venda.
- As definições das permissões de acesso são feitas nos grupos de usuários, pois facilitam o cadastro de vários usuários com a mesma função.
- Quando um usuário acessa o Staff500, libera esse terminal para a abertura de quantos programas forem necessários. Portanto, ao sair de qualquer um desses programas, se pedir para encerrar a seção desse usuário, estará encerrando também em todos os módulos ainda abertos.
- Se um usuário estiver logado em um terminal e tentar entrar em outro, será informado que esse usuário está usando outro terminal. Se for selecionada a opção "Continuar", a seção será encerrada no outro terminal.
- O módulo de pré venda é o único que encerra, automaticamente, a seção do usuário no encerramento do programa.


## Como efetuar o cadastro de um usuário:

No programa de usuários, pressione ENTER em usuários para abrir a lista. Para incluir um novo usuário, pressione I de inclui e informe um código a ser utilizado, como o próprio nome, ou numérico, tipo 001, 002 e assim por diante, se esse usuário for também vendedor. Escreva o nome do usuário, e informe o seu nível e confirme ativo SIM. Lembrando que existem dois níveis, “1” e “9”, devendo ser respeitadas as orientações do item 01 da lista de observações.
Depois de cadastrado o usuário, volte ao menu principal e, em GRUPOS, cadastre um grupo de usuários com a mesma função como, vendas, escritório, faturamento, caixa etc. e em seguida uma descrição do grupo e pressione S de sim em ativa. Depois de cadastrado o grupo, pressione ENTER para abrir a lista e I de incluir o usuário nesse grupo. Sobre a lista selecione o usuário e confirme com ENTER. E assim sucessivamente com todos os usuários que terão a mesma função. O mesmo usuário pode ser cadastrado em mais de grupo com funções complementares. Caso um usuário tenha uma função que não se enquadre em nenhum dos grupos, crie um especialmente para ele usando o procedimento citado acima e então defina suas atribuições.
Para definir as permissões de acesso, posicione sobre o grupo desejado e pressione C de chaves e com a seta do teclado, escolha o módulo do Staff500 que deseja acessar e vá até a lista de funções e com ENTER defina a permissão SIM ou NÃO.
Nas opções SIM, pode ser ativada a função LOG, pressionando L, caso a empresa queira monitorar as ações desse usuário. Nas opções marcadas NÃO, todos os acessos autorizados por um superior, terão suas ações gravadas automaticamente.

## Pendências

Sempre que um usuário tentar um acesso não permitido lhe será solicitada a permissão de um superior. Essa operação poderá liberada no ato se o responsável estiver presente, caso contrário e desejar liberar remotamente, basta que usuário solicitante pressione ENTER e será feita a pergunta se deseja enviar a solicitação ao servidor, com a opção de descrever a justificativa da solicitação. Nesse caso o usuário avalista poderá acessar o módulo de usuários>pendências e, com ENTER liberar, ou com R, responder o motivo da não liberação, ou com E, excluir o pedido. Se o pedido for liberado, basta que o usuário solicitante pressione ENTER novamente para seguir adiante com a operação.

## Auditoria

Todas as operações marcadas para gerar LOG e as que tiveram pedidos de senha liberados por algum usuário avalista serão gravadas nesse local. Para buscar uma ação específica, pressione B, para visualizar a tela referente, pressione ENTER ou excluir com a tecla E