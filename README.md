# curso_dev_lab
https://www.youtube.com/watch?v=W2ld5xRS3cY&amp;list=PLz_YTBuxtxt6_Zf1h-qzNsvVt46H8ziKh

# Título da aula
Node.js API [C01P01] - Iniciando o projeto configurando NodeJS, Typescript, yarn e module-alias

# Comandos executados no terminal

'npm init -y' - Comando utilizado para iniciar o nosso projeto node criando o arquivo package.json com uma configuração padrão.

'yarn add -D typescript && yarn add -D @types/node && tsc --init' - O primeiro comando adiciona ao nosso projeto o typescript e o segundo os types para o node poder trabalhar com o typescript. Ambos adicionados como dependência de desenvolvimento. O último comando é executado para iniciar um projeto typescript e adicionar o arquivo de configuração 'tsconfig.json' para o mesmo.

'yarn add module-alias && yarn add @types/module-alias' - Configuramos paths no arquivo de configuração do typescript. Esse comando é executado para adicionar como dependência do projeto pois quando colocarmos o mesmo em um ambiente de produção será utilizado. Ele serve para configurarmos nossos paths para que assumam um apelido.

# Não esquecer

Nesse capítulo adicionamos dois scripts no arquivo packege.json. Um chamado 'build' para exportar o nosso código para JavaScript e o outro chamado 'start' que executa o comando anterior e executa o servidor em seguida.

"scripts": {
    "build": "tsc",
    "start": "yarn build && node dist/src/index.ts"
}