# Framework Empire - Anotações

O Empire é um software de pós-exploração. Ou seja, ele facilita a manipulação do sistema após o estabelecimento da conexão entre o alvo (denominado `AGENT`) e o servidor contendo o Empire, também chamado de servidor de comando e controle (denonimado `C2`).

Após a conexão, o Empire permite executar funções como:

- Aplicar Shell Scripts
- Monitorar Keyloggers
- Mover, pegar e deletar arquivos
- Salvar capturas de tela

## Requisitos

Para testes de intrusão, é ideal que se use um servidor cloud, como por exemplo o EC2 ou Lightsail da AWS (C2). É importante que o servidor tenha o firewall aberto para as portas que serão configuradas no Empire. Sem isso, o Agent não se conectará com o C2.

Para o primeiro exemplo, um computador Windows completamente desprotegido, sem antivírus e com o Firewall desligado, será necessário. Ele será nosso alvo.

## Instalando o Empire

O Empire pode ser instalado seguindo as orientações do repositório abaixo e clonando os arquivos no seu servidor:

- git clone https://github.com/EmpireProject/Empire

## Configurando o Empire

Após inicializar o Empire (certifique-se de abri-lo com o comando `sudo`, para dar permissões de administrador), é possível ver a lista de comandos do framework por meio do comando `help`. Os três principais componentes são: `modules`, `listeners` e `agents`. Mais informações serão passadas ao longo dessas anotações.

O primeiro passo é criar um `Listener`. Ele será responsável por ficar "ouvindo" uma porta de conexão do servidor C2, na esperança de encontrar o alvo infectado tentando se conectar por ela.



