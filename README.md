Fora da Caixa é um app desenvolvido para auxiliar no treinamento de Analistas de testes;
O app simula um aplicativo bancário com algumas funcionalidades 'implementadas';
Os dados são salvos localmente numa base de dados, e toda vez que o app é removido a base é removida também;
Projeto roda em Android e iOS; 
Projeto não possui Integration Testing nessa versão;


## Comandos para verificar versões

    detalhes gerais: flutter doctor -v
    verificar versão do flutter: flutter --version
    local de instalação do flutter: where flutter 
    verificar versão do dart: dart --version
    local de instalação do dart: where dart

## Getting Started

    Users para logar:
        CPF: 929.035.400-39
        CPF: 050.209.090-17
        CPF: 971.147.000-40

    Users para transferir pix: 
        Os mesmos acima. 
        Dica 1: cadastre chaves pix para os usuários e use elas;
        Dica 2: os CPFs em si já estão cadastrados como chave pix por default;
    
    Senha para logar com os users: 
        172839
    Token válido para cadastrar chave pix: 
        123456 (qualquer outro é considerado inválido)    
    Pin válido: 
        1234

## O que esse app faz?
    
    App simula um aplicativo financeiro, com as seguintes funcionalidades:
        Login:
            Valida usuários válidos e inválidos e informa ao usuário;
            Durante o primeiro login solicita ao usuário permissão de Localização;
        Transferência pix:
            Processo completo de transferência com debito em conta;
            Agendamento de transferência pix;
            Comprovante de transferência pix;
        Cadastro de alguns tipos de chaves pix:
            Algumas chaves podem ser cadastradas, outra não;
        Histórico de transferências e recebimentos:
            Ao tocar no saldo do usuário é possível visualizar o histórico;
        Diversos bugs e pontos de melhorias:
            Este é um app de treinamento para QAs, nada melhor que alguns bugs para cadastrar :)


## Para gerar apk de debug

    flutter build apk --debug

## Para rodar o projeto em modo release (útil quando rodar em device físico iOS)
    
    flutter run --release