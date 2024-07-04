# ApexReplayDebugger

Este repositório contém um projeto que utiliza o Apex Replay Debugger para depurar código Apex no Salesforce.

## Índice

- [Visão Geral](#visão-geral)
- [Requisitos](#requisitos)
- [Instalação](#instalação)
- [Uso](#uso)
- [Contato](#contato)

## Visão Geral

O ApexReplayDebugger é uma ferramenta que permite aos desenvolvedores depurar o código Apex no Salesforce usando arquivos de log de depuração. Ele facilita a identificação e correção de problemas no código Apex.

## Requisitos

- Conta no Salesforce com permissões de desenvolvedor.
- Salesforce CLI instalada.
- Visual Studio Code com Salesforce Extension Pack instalado.

## Instalação

1. Clone este repositório:
    ```bash
    git clone https://github.com/seu-usuario/ApexReplayDebugger.git
    ```

2. Navegue até o diretório do projeto:
    ```bash
    cd ApexReplayDebugger
    ```

3. Autentique-se no Salesforce CLI:
    ```bash
    sfdx force:auth:web:login
    ```

4. Crie uma nova organização:
    ```bash
    sfdx force:org:create -s -f config/project-scratch-def.json
    ```

5. Instale os metadados:
    ```bash
    sfdx force:source:push
    ```

6. Abra a organização no navegador:
    ```bash
    sfdx force:org:open
    ```

## Uso

1. Gere um arquivo de log de depuração no Salesforce:
    - Execute o código Apex que você deseja depurar.
    - Navegue até Configuração > Logs de Depuração de Apex > Monitoramento de Depuração e ative o monitoramento.
    - Baixe o arquivo de log gerado.

2. Carregue o arquivo de log no Visual Studio Code:
    - Abra o Visual Studio Code.
    - Vá para a aba "Run and Debug" e selecione "Apex Replay Debugger".
    - Carregue o arquivo de log de depuração.

3. Inicie a sessão de depuração:
    - Defina pontos de interrupção no código Apex conforme necessário.
    - Inicie a sessão de depuração e analise o comportamento do código passo a passo.

## Contato

Para mais informações, entre em contato através do email: [dev.alvarojordao@gmail.com](mailto:dev.alvarojordao@gmail.com).

---

Obrigado por utilizar o ApexReplayDebugger!
