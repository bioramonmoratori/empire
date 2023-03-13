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

## Configurações do Empire



