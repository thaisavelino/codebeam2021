This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.js`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.



_________________

_________________


# Guia em Português para colaboradores BR


O Design e todas as imagens do projeto estão no Figma



Repositório do github :
https://github.com/felipecotto/codebeam2021



## Como colaborar no projeto?


1. Primeiro abre o terminal e escolha aonde quer salvar seu projeto. Vamos salvar no Desktop, neste exemplo:

```
cd Desktop
```
 
2. Git clone no repositorio, para trazer o código do site para seu computador:

```
git clone git@github.com:felipecotto/codebeam2021.git codebeam
```

Neste comando estamos fazendo o clone do repositório e colocando tudo em uma pasta chamada "codebeam"

3. Instale as dependências. Para isso precisa entrar na pasta do codebeam

Entre na pasta codebeam
```
cd codebeam
```

Instale as dependencias

```
npm install
```

*se não tiver o npm instalado na máquina, vai precisar instalar. Se precisar, peça ajuda ao meu amigo:
https://www.google.com/


4. Vamos ver se está funcionando? 

Rode o servidor para ver o projeto compilado localmente:
```npm run dev```

Entre no navegador para ver a landing page:
http://localhost:3000




## Como fazer a codificação?


Bom, se tudo deu certo até aqui, você já pode começar a trabalhar no código.

1. Trabalhar em homologação primeiro
Quando estiver fazendo atualizações no código, trabalhe na branch develop, que é a de homologação.

```git checkout develop```

2. Publique o código em homologação, para outras pessoas fazerem o QA
Quando quiser publicar o código no ambiente de homologação e qualquer pessoa poderá revisá-lo no endereço para testes:

[https://codebeambr-homol.vercel.app/](https://codebeambr-homol.vercel.app/)

Veja em qual branch está:
```git branch```

Vá para branch develop:
```git checkout develop```

Quando quiser publicar o código em homologação:

```
git add .
git commit -am “seu comentário”
git push origin develop
```



### Publicar o site em produção:
Quando tudo estiver certo. Mude para a branch main e dê um push, que a nova versão será publicada em produção no site da Code Beam BR:
[CodeBeamBR](https://www.codebeambr.com/)

*Certifique-se de que deu o push na develop, nos passos anteriores*

Vá para a branch main:

```
git checkout main
```

Traga o código que fez na branch develop para cá:

```
git pull origin develop
```




## Dúvidas sobre a organização dos arquivos :


#### Onde encontrar as imagens?
As imagens ficam na pasta Public, organizadas da sequite forma:

* Ícones do footer ficam na pasta:
**Public/icons**
* Os vídeos da home, ficam em:
**Public/thumbs**
* As fotos dos palestrantes ficam nas pastas referente ao tipo de apresentação:
**Public/keynotes, Public/panels ou Public/talks**

#### Onde encontrar o CSS?
Dentro da pasta de cada sessão tem o CSS dele, e é nesse arquivo que colocamos coisas específicas.
O css global fica em **src/globals.scss** nele colocamos as fonte, reset padrão, e tudo que é global do projeto
A home é uma página então tem CSS próprio, que fica em **src/Home.module.scss**


Se precisarem de alguma ajuda, podem chamar @ThaisAvelino
