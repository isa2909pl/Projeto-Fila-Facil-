# Projeto-Fila-Facil-
📱 Fila Fácil

Objetivo:
Criar um sistema para organizar filas de atendimento, permitindo que o cliente entre na fila e acompanhe sua posição sem precisar ficar esperando presencialmente.

Usuários:

Cliente: entra na fila e acompanha sua senha.
Funcionário: controla a fila e chama os clientes.
Administrador: cadastra estabelecimentos, serviços e usuários.

Principais funções:

Cadastro e login
Cadastro de estabelecimentos e serviços
Entrada na fila
Geração de senha
Acompanhamento da posição
Chamada do próximo cliente
Finalização/cancelamento do atendimento
Histórico de atendimentos

Banco de dados:

Usuários
Funcionários
Estabelecimentos
Serviços
Filas
Senhas/Atendimentos

Tecnologias sugeridas:

HTML + CSS + JavaScript
PHP
MySQL

Regras do sistema

Vamos definir algumas regras desde já para facilitar a programação.

Regra 01: Um usuário pode estar em apenas uma fila ativa por vez.

Regra 02: Cada senha pertence a uma única fila.

Regra 03: A senha recebe um número automaticamente.

Regra 04: O funcionário só pode chamar uma senha por vez.

Regra 05: Depois que uma senha for finalizada, ela passa para o histórico.

Regra 06: O cliente pode cancelar sua senha enquanto estiver aguardando.

Regra 07: O funcionário não pode chamar uma senha que já tenha sido atendida ou cancelada.

Regra 08: Cada estabelecimento pode possuir vários serviços.

Regra 09: Cada serviço pode possuir uma fila própria.
Cliente → Escolhe estabelecimento → Escolhe serviço → Entra na fila → Recebe senha → Acompanha posição → É chamado.

Tipos de usuários

Teremos 3 tipos de acesso:

👤 Cliente
Pode:

Criar conta
Entrar no sistema
Escolher estabelecimento
Escolher serviço
Entrar na fila
Acompanhar posição
Cancelar sua senha
Consultar histórico

👨‍💼 Funcionário
Pode:

Visualizar fila
Chamar cliente
Iniciar atendimento
Finalizar atendimento
Cancelar atendimento
Visualizar histórico

👑 Administrador
Pode:

Gerenciar usuários
Gerenciar funcionários
Gerenciar estabelecimentos
Gerenciar serviços
Gerenciar filas
Consultar relatórios
Fluxo principal:



Área do funcionário

O funcionário terá um painel para controlar a fila.

Dashboard

Mostrar:

Pessoas aguardando
Pessoas atendidas
Próxima senha
Tempo médio de espera
Fila atual
Botões principais:

[ CHAMAR PRÓXIMO ]

[ INICIAR ATENDIMENTO ]

[ FINALIZAR ATENDIMENTO ]

[ CANCELAR SENHA ]

Como o sistema vai funcionar
👤 CLIENTE

O fluxo será:

Cadastro/Login → Escolher estabelecimento → Escolher serviço → Entrar na fila → Receber senha → Acompanhar fila → Ser chamado


Exemplo:

João chega a uma clínica, mas não precisa ficar esperando na recepção. 

Ele entra no Fila Fácil:

Clínica Saúde
↓
Consulta
↓
Entrar na fila

O sistema gera:

Senha: A023
Pessoas à sua frente: 4
Posição: 5º

Conforme os atendimentos acontecem, a posição diminui.
