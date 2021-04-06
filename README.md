<h1 align="center">Começando com o Git 🚀</h1>
<img src="./midias/github.png">

## 🛠 O que é um sistema de controle de versoões?
<p>Git é um sistema de controle de versão utilizado pela maioria de desenvolvedores e por grande parte das empresas de tecnologia. Com ele é possível criar histórico de alterações no código do projeto e facilmente voltar para qualquer ponto.</p>
<br/>
<p> Além disso, o Git nos ajuda a criar ramificações que são formas de termos uma mesma versão do código sofrendo alterações e recebendo commits de diferentes fontes e de diferentes desenvolvedores.</p>
<br/>
<p>Dessa forma, nós podemos trabalhar em duas ou mais versões do mesmo projeto, um time de desenvolvedor pode inicialmente estar trabalhando em um MVP do projeto e a partir dessa versão outra é criada na qual se dará incio ao produto final com outro time de desenvolvedor.</p>
<br/>
<img  src="./midias/git-workflow.png" >

<sub>Foto de https://leanpub.com/git-flow/read <sub>
<br/>
<br/>

## 💻 Comandos básicos Git
<p><b>Criando um novo repositório:</b></p>
<p>crie uma nova pasta, abra-a e execute o comando para criar um novo repositório.</p>

```
    git init
```
<br/>
<p><b>Obtenha um repositório:</b></p>
<p>crie uma cópia de trabalho em um repositório local executando o comando.</p>

```
    git clone /caminho/para/o/repositório
```
<p>quando usar um servidor remoto, seu comando será</p>

```
    git clone usuário@servidor:/caminho/para/o/repositório
```
<br/>
<p><b>fluxo de trabalho</b></p>

Seus repositórios locais consistem em três "árvores" mantidas pelo git. a primeira delas é sua `Working Directory` que contém os arquivos vigentes. a segunda `Index` que funciona como uma área temporária e finalmente a `HEAD` que aponta para o último commit (confirmação) que você fez.

<br/>

<p><b>adicionar & confirmar:</b></p>
<p>Você pode propor mudanças (adicioná-las ao Index) usando</p>

```
    git add <arquivo>
    git add *
```
<p>Este é o primeiro passo no fluxo de trabalho básico do git. Para realmente confirmar estas mudanças (isto é, fazer um commit), use</p>

```
    git commit -m "comentários das alterações"
```
<p>Agora o arquivo é enviado para o HEAD, mas ainda não para o repositório remoto.</p>
<br/>

<p><b>Enviando alterações</b></p>
<p>Suas alterações agora estão no HEAD da sua cópia de trabalho local. Para enviar estas alterações ao seu repositório remoto, execute</p>

```
    git push origin master
```
<p>Altere master para qualquer ramo (branch) desejado, enviando suas alterações para ele.</p>
<br/>
<p>Se você não clonou um repositório existente e quer conectar seu repositório a um servidor remoto, você deve adicioná-lo com</p>

```
    git remote add origin <servidor>
```

<p>Agora você é capaz de enviar suas alterações para o servidor remoto selecionado.</p>
<br/>

<p><b>Ramificando</b></p>
<p>Branches ("ramos") são utilizados para desenvolver funcionalidades isoladas umas das outras. O branch master é o branch "padrão" quando você cria um repositório. Use outros branches para desenvolver e mescle-os (merge) ao branch master após a conclusão.</p>
<p>crie um novo branch chamado "funcionalidade_x" e selecione-o usando</p>

```
    git checkout -b funcionalidade_x
```
<p>retorne para o master usando</p>

```
    git checkout master
```
<p>e remova o branch da seguinte forma</p>

```
    git branch -d funcionalidade_x
```

<p>um branch não está disponível a outros a menos que você envie o branch para seu repositório remoto</p>

```
   git push origin <funcionalidade_x>
```

<br/>
<p><b>Atualizar & mesclar</b></p>
<p>para atualizar seu repositório local com a mais nova versão, execute<p>

```
    git pull
```
<p>na sua pasta de trabalho para obter e fazer merge (mesclar) alterações remotas.
para fazer merge de um outro branch ao seu branch ativo (ex. master), use</p>

```
    git merge <branch>
```
<p>em ambos os casos o git tenta fazer o merge das alterações automaticamente. Infelizmente, isto nem sempre é possível e resulta em conflitos. Você é responsável por fazer o merge estes conflitos manualmente editando os arquivos exibidos pelo git. Depois de alterar, você precisa marcá-los como merged com</p>

```
    git add <arquivo>
```
<p>antes de fazer o merge das alterações, você pode também pré-visualizá-las usando</p>

```
    git diff <branch origem> <branch destino>
```
<br/>

## 🔗 Links
- [git - the simple guide](https://rogerdudler.github.io/git-guide/index.html)
- [Comandos iniciais do Git](https://tableless.com.br/alguns-comandos-git/)
- [O que é github](https://www.hostinger.com.br/tutoriais/o-que-github)
- [A importancia do git em um  negócio](https://rockcontent.com/br/blog/o-que-e-github/)
- [Controlando versões com Git e GitHub](https://www.casadocodigo.com.br/pages/sumario-git-github)
- [Comandos Git do básico ao avançado](https://comandosgit.github.io/)

<br/>

---
<div align="center">

###  ✏️ Autor
<p align="center>
<table>
  <tr>
    <td align="center"><a href="https://www.linkedin.com/in/igorpaz/"><img style="border-radius: 50%;" src="./midias/perfil.jpg" width="100px;" alt=""/><br /><sub><b>Igor Gabriel Paz</b></sub></a> <a href="https://www.linkedin.com/in/igorpaz/" title="igorpgaz">👨‍🚀</a><br/>
    <p>Feito com 💜 por Igor Paz 👋 Entre em contato!</p>
    <a href="https://www.linkedin.com/in/igorpaz/">
        <img src="https://img.shields.io/badge/-igorgpaz-blue?style=flat-square&logo=linkedin&labelColor=blue">
    </a>
    </td>
  </tr>
</table>
</p>
</div>

---