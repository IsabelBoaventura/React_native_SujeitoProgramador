# INSIDE 5

Semana React Native 

Sujeito Programador 

    https://sujeitoprogramador.com/insider-1/


Caminho no Figma

  https://www.figma.com/file/Hgb3JJjhfuG5zMXwjC72o4/React-Native-Insider-5?node-id=0%3A1  

Instalar o node.js

    Tenho instalada a versão v16.13.2

Baixar a biblioteca `expo`

    https://expo.dev

Nesta página principal  DOCS terá as informações de como instalar a biblioteca 

    https://docs.expo.dev


    npm i -g expo-cli
    expo init my-project

    npm install --global expo-cli

No terminal do VSCode a primeira linha ja deu certo. 


## Criar o aplicativo

Rodando no celular e rodando no celular ou usando o Emulador 

### Android studio

    https://developer.android.com/studio

Depois de instalar o Android Studio,abra ele ( emulador Android Studio ), instalação Padrão ... abrir .

        More Actions => SDK Manager

Para configurar a Api, qual o sistema do Android que se quer emular que se esta trabalhando.

Configurações:
    Appearance & Behavior 
        System Setting 
            Android SDK 
                => Android 10.0 Q 
                (aba) SDK Tools
                    => Android SDK Build-Tools 33-rc4
                    => Android Emulador 
                    => Android SDK Plataform-Tools 
                    => Google Play Services 
                    => Intel x86 Emulador Acelerator ( se o processador for Intel )
Apply  => ok 


Depois de tudo instalado voltar para a tela principal

    More Actions => Virtual Device Manage => Create Virtual Device => Pixel 3  => Next 
    (aba ) x86 Images  => Q => Doawnloads  
        Api Level 29    ABI ( x86_64)       Target ( Android 10.0 ( Google APIs ))
    Next
        Mudar o nome 
            Pixel 3 API 29 INSIDE
        finish

Assim abre o emulador do Celular, o meu ficou quadradão.


Como criar o aplicativo e rodar no Emulador


## blog


Nosso aplicativo se chamará  `BLOG`, para criarmos entraremos dentro da pasta onde iremos trabalhar e usaremos o comando: `expo init blog`
Dentro do cmd ele  mostrará possibilidades de criação, para o nosso exemplo será usado o `_blank` que seria equivalente a o começo de um projeto em branco. 


Criando a pasta `blog`com varios arquivos dentro. Toda a estrutura do projeto. 


### Rodar o projeto

Para rodar o projeto, ainda usando o cmd iremos entrar dentro da pasta criada 

    cd blog 

Dentro da pasta vamos dar o comando para rodar o aplicativo 

    `expo start` 

Vai gerar o QR Code do aplicativo e o endereço para acessar: `http://localhost:19002` acessando este endereço tens como ir para o site























    Tools






