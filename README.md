# Como instalar/configurar/usar o `postfix` no `Linux Ubuntu`

## Resumo

Neste documento estão contidos os principais comandos e configurações para instalar/configurar/usar o `postfix` no `Linux Ubuntu`.

## _Abstract_

_This document contains the main commands and settings to install/configure/use the `inkscape` on `Linux Ubuntu`._

## Descrição [2]

### `postfix`

O `Postfix` é um popular servidor de email de código aberto projetado para ser rápido, fácil de configurar e altamente seguro. Ele é amplamente utilizado em servidores Unix-like, incluindo Linux. O `Postfix` gerencia o envio, recebimento e encaminhamento de emails, suportando protocolos como SMTP, SMTPS e TLS para comunicações seguras. Sua arquitetura modular e configuração flexível o tornam uma escolha confiável para hospedar serviços de email em ambientes corporativos e de servidor.


## 1. Configurar/Instalar/Usar o `postfix` no `Linux Ubuntu` [1]

Para configurar/instalar/usar o `postfix` no `Linux Ubuntu`, você pode usar o gerenciador de pacotes apt. Siga os passos abaixo:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`


2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.2 Remover pacotes `.deb` antigos ou duplicados do cache local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando: `sudo apt autoclean`

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando: `sudo apt autoremove -y`

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`: `sudo apt update`

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes: `sudo apt --fix-broken install`

    2.6 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:  `sudo apt list --upgradable`

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`: `sudo apt full-upgrade -y`
    

3. **Instale o `Inkscape`**: Depois de atualizar a lista de pacotes, você pode instalar o `Inkscape` usando o comando abaixo: `sudo apt install inkscape -y`

4. **Verifique a instalação**: Após a conclusão da instalação, você pode verificar se o `Inkscape` foi instalado corretamente executando o comando: `inkscape --version`

Se tudo estiver correto, você verá a versão do `Inkscape` instalada no seu sistema.

Esses comandos são suficientes para instalar o `Inkscape` no `Ubuntu` via `Terminal Emulator`.

## 1.1 Código completo para configurar/instalar/usar

Para configurar/instalar/usar o `inkscape` no `Linux Ubuntu` sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abra o `Terminal Emulator. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Digite o seguinte comando e pressione `Enter`:

    ```
    sudo apt clean
    sudo apt autoclean
    sudo apt autoremove
    sudo apt update -y
    sudo apt autoremove
    sudo apt autoclean
    sudo apt list --upgradable
    sudo apt full-upgrade -y
    sudo apt install inkscape -y
    inkscape --version
    ```

## Referências

[1] OPENAI. ***Instalar inkscape no ubuntu.*** Disponível em: <https://chatgpt.com/c/335f2af0-cc09-4cc1-82a0-60c6824dd07d> (texto adaptado). ChatGPT. Acessado em: 25/10/2023 10:24.

[2] OPENAI. ***Vs code: editor popular.*** Disponível em: <https://chat.openai.com/c/b640a25d-f8e3-4922-8a3b-ed74a2657e42> (texto adaptado). ChatGPT. Acessado em: 16/11/2023 10:06.

