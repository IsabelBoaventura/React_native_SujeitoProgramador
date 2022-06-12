# React_native_SujeitoProgramador

INSIDE 5

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

Vai gerar o QR Code do aplicativo e o endereço para acessar: `http://localhost:19002` acessando este endereço tens como ir para o site. 

Esta é a primeira tela do site:

![image](https://user-images.githubusercontent.com/1613816/172027210-d795e43c-7ab3-429f-b4dc-852ea5bafdcd.png)

Rodando no Emulador

![image](https://user-images.githubusercontent.com/1613816/172027229-fe563eb9-6be0-4759-8bfe-7824cb548e34.png)


Para ter acesso no próprio celular, tem de baixar o `Expo Go` depois abre a camera do celular e aponta para o QRCode .

## Vamos programar


`App.js` é a nossa páginma principal. 


![image](https://user-images.githubusercontent.com/1613816/172027733-33f60ca3-98f8-4662-bf80-fcac0084cbcd.png)

Para começar vamos limpar tudo o que já venho pré programado, e começar o nosso do zero. 


Importando o React;
A medida que for criando os codigos será comentado dentro dos códigos.

Criando novas pastas e arquivos:

- (pasta) src
   - (pasta) pages
        - (pasta) Home
            - (arquivo) index.js

O arquivo da página Home, foi levado para o arquivo app.js ,entretanto no meu codigo esta apresentando erros. 


No arquivo dele esta aparecendo o conteudo do Home dentro do arquivo App.js(). Entretanto o mesmo nao acontece com o meu.

Achei que pudesse ser algo referente a cor,  ja que antes aparecia quando o fundo estava escuro, fiz as modificações,  e até agora nada. 

## Vamos seguir

Apesar de estar acusando erro,  vamos seguir com os codigos;

Aogra precisaremos ter uma biblioteca para fazer a navegação entre as páginas 

    https://reactnavigation.org/
    
 React Documents => Installation 
 
    https://reactnavigation.org/docs/getting-started/
    
    https://reactnavigation.org/docs/getting-started/
    
    
    
    npm install @react-navigation/native
    
Vamos parar o projeto, no terminal   `CTRL` + `c`  para parar o projeto. 

Escrevemos o comando, no video o comando foi  `expo install @react-navigation/native`  mas o meu terminal recusou este comando.

No meu terminal  o comando que funcionou foi: `npm install --save @react-navigation/native`

Interessante,  os comandos da expo ( expo install ... ) nao estao funcionando dentro do sistema, assim as bibliotecas que o sistema precisa, estou instalando com o `npm`;

Próxima biblioteca:
    `npm install --save react-native-screens react-native-safe-area-context`
    
Instalado com sucesso.

Agora para aparecer em tipo pilha na tela `stack`

   `npm install --save @react-navigation/native-stack`
   
Instalado com sucesso.

Agora rodar novamente o projeto `expo start` .

Interessante 'expo start' não funciona dentro do terminal do VSCode,  mas no terminal normal funciona. 




Voltando para o sistema.
Dentro da pasta `src` será criado o arquivo `routes.js`para a navegação do sistema.

Criada a rota, e exportado para o arquivo app.js 

![image](https://user-images.githubusercontent.com/1613816/172032049-c11d7ad9-36b3-4140-9d54-7720542dcb23.png)


Estou abrindo no navegador, e Emulador tem de aprender a trabalhar com ele. 

Agora vamos criar as páginas seguintes,  pelo menos a estrutura delas. 

- (pasta) pages
  - (pasta) Details [ detalhes ]
    - index.js 
  - (pasta) Category [ Categorias dos Posts ]
    - index.js
  - (pasta) Search [ Pesquisa ]
    - index.js

Agora importar cada uma destas pastas nas configurações das rotas, assim como havia sido realizado com o Home.

E dentro da pasta Home ,  importar o Metodo que faz a navegação entre as páginas.

Estrutura das páginas criadas e organizadas com o básico apenas para o teste de navegação.

Organizada a pagina principal. 

Agora vamos para o Back-end


## Back-end

Para ter acesso as informações que iram aparecer no sistema precisaremos do Back-end ( serviço que será consumido pelo nosso app ).

Para isto teremos de usar um CMS para gerenciar o conteudo.

### CMS

"Um Sistema de Gerenciamento de Conteúdo  (Content Management System), ou simplesmente CMS, é um software executado no navegador permite que você crie, gerencie e modifique um website e seu conteúdo sem a necessidade de conhecimento de programação." ( explicação retirada da internet ).

O CMS escolhido para este projeto foi o `strapi`  que pode ser encontrado em `https://strapi.io/` .

Comando para criar o projeto `npx create-strapi-app@latest my-project`

Fora da pasta do projeto ( no nosso caso a pasta 'blog') criar o projeto do CMS.

Para ficar mais facil a identificação futura criamos assim: `npx create-strapi-app@latest blog-api`

Depois de instalado, o sistema oferece tipos de criação, foi escolhido o `Quickstart`;

O proprio sistema me redirecionou para a pagina http://localhost:1337/admin/ onde  preenchi os dados .. salvei a senha `Strapi123`



Area administrativa do nosso projeto:

![image](https://user-images.githubusercontent.com/1613816/173201070-389fcae6-8cb3-4263-8190-59da679ffd40.png)

Como entrar nele 
![image](https://user-images.githubusercontent.com/1613816/173201092-8f854e00-b921-41f1-99a9-9051183f26ef.png)


`Content-type-builder`

`Create new colletion type `

![image](https://user-images.githubusercontent.com/1613816/173201139-397d3b61-9eb5-4429-9f20-b8fca3bebea9.png)

Criado 'Category' com dois campos um deles de texto 'nome' e outro de imagem  'icon';

![image](https://user-images.githubusercontent.com/1613816/173201298-ca66428b-e2bb-4536-8e48-0bf3ebfa466c.png)




**













