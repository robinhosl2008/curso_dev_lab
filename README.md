## curso_dev_lab - [URL do Curso](https://www.youtube.com/watch?v=W2ld5xRS3cY&amp;list=PLz_YTBuxtxt6_Zf1h-qzNsvVt46H8ziKh)

## Branchs

- develop
- main

## Título da aula 01
Node.js API [C01P01] - Iniciando o projeto configurando NodeJS, Typescript, yarn e module-alias -
[URL da vídeo-aula](https://www.youtube.com/watch?v=QyK63wEKnvA&list=PLz_YTBuxtxt6_Zf1h-qzNsvVt46H8ziKh&index=2)

#### Comandos executados no terminal

Comando utilizado para iniciar o nosso projeto node criando o arquivo package.json com uma configuração padrão.
```
    npm init -y
```

O primeiro comando adiciona ao nosso projeto o typescript e o segundo os types para o node poder trabalhar com o typescript. Ambos adicionados como dependência de desenvolvimento. O último comando é executado para iniciar um projeto typescript e adicionar o arquivo de configuração 'tsconfig.json' para o mesmo.
```
    yarn add -D typescript && 
    yarn add -D @types/node && 
    tsc --init
```

Configuramos paths no arquivo de configuração do typescript. Esse comando é executado para adicionar como dependência do projeto pois quando colocarmos o mesmo em um ambiente de produção será utilizado. Ele serve para configurarmos nossos paths para que assumam um apelido.
```
    yarn add module-alias && 
    yarn add @types/module-alias
```

###### Não esquecer

Nesse capítulo adicionamos dois scripts no arquivo packege.json. Um chamado 'build' para exportar o nosso código para JavaScript e o outro chamado 'start' que executa o comando anterior e executa o servidor em seguida.

```
    "scripts": {
        "build": "tsc",
        "start": "yarn build && node dist/src/index.ts"
    }
```

--------------------------------------------------------------------------------------------------------------

## Título da aula 02
Node.js API [C01P02] - Configurando eslint com NodeJS e Typescript.
[URL do vídeo](https://www.youtube.com/watch?v=imo0hXHQzMk&list=PLz_YTBuxtxt6_Zf1h-qzNsvVt46H8ziKh&index=3)

eslint - Instalamos esse extensão como dependência de desenvolvimento. Basicamente ela serve para nos ajudar com a análise de código estático e regras do código para termos um padrão. Ou seja, configurar os padrões de código que iremos utilizar no nosso projeto.
```
    yarn add -D @typescript-eslint/eslint-plugin eslint @typescript-eslint/parser
```