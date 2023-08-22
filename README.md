# Receitas a la Git
## Objetivo
O objetivo desse repositorio é para auxiliar os alunos da UNIVESP a entender o funcionamento de um ciclo de colaboração no Github.

## Como utilizar
A ideia é montar um organizado de receitas, cada aluno irá efetuar:
1. O **fork** do repositorio
1. O **clone** deste repositorio _"forkado"_
1. Criar uma nova branch com o nome neste padrão **\<siglas do nome\>\-<nome da receita em [Kebab-case](https://coodesh.com/blog/candidates/dicas/convencoes-de-codificacao-do-camelcase-ao-kebab-case/#:~:text=Muito%20parecido%20com%20a%20conven%C3%A7%C3%A3o,%2Dde%2Dkebab%2Dcase.)>**;
1. Adicionar a receita na pasta **Menu** e caso tenha imagens na pasta **imagens**, recomenda-se usar **[Markdown](https://pt.wikipedia.org/wiki/Markdown)** para formatar o texto, mas se não souber pode deixar sem foratação;
1. Efetuar o Commit
1. Subir a branch para o **seu** repositorio
1. Criar uma nova **Pull Request** para o repositorio de origem na **Branch** Main

## Passo a passo
### 1. Faça o **fork** do repositorio:

Deve-se efetuar o **fork** deste repositorio [receitas-a-la-git](https://github.com/UNIVESP23/receitas-a-la-git)
clicando no botão de **Fork** no canto superior direito.
![Alt text](imagens/1.png)

E depois clique em Create Fork, isso vai duplicar o repositorio para sua conta pessoal do Github, assim voce pode efetuar qualquer edição que queira
![Alt text](imagens/2.png)

### 2. Faça o clone deste repositorio "forkado"

Na sua maquina abra o terminal do git, o `git Bash`.
Digite o caminho do local onde dexeja fazer o download do repositorio. Por exemplo eu vou salvar o repositorio em uma pasta no meu perfil chamada `repositorios`.
Digite o comando `cd [pasta de destino]` seguido pela pasta onde vai ficar o repositorio
exemplo:
``` bash
$ cd repositorios
```

Agora realize o **Clone** do seu repositorio usando o comando `git clone [repositorio]`. Lembrando que voce deve clonar o repositorio que voce **"Forkou"**, ou seja o repositorio no seu usuario do Github.
exemplo:
```bash
$ git clone https://github.com/apavanello/receitas-a-la-git.git
```

Com isso uma "copia" do repositorio será salva na sua maquina

Lembre de entrar dentro da pasta do repositorio clonado antes de realizar os proximos passos:

![Alt text](imagens/3.png)

### 3. Criar uma nova branch com o nome neste padrão \<siglas do nome\>-\<nome da receita em Kebab-case\>

Para criar uma nova **branch** rode o comando:

`git branch <nome da branch>`

Isso ira criar uma nova **branch** mas não vai trocar para a mesma de imediato. Para realizar a troca digite:

`git checkout <nome da branch>`

Caso queira realizar tudo de uma vez digite o comando:

`git checkout -b <nome da branch>`

Assim o git vai criar a **branch** caso ela não exista e já mudar o estado atual para a mesma

> obs.: pode-se ver qual a branch atual digitando o comando `git branch`, o mesmo ira listar todas as branchs criadas e colocar um "*" na frente da que está ativa

> Obs2.: Lembre da sintaxe obrigatoria para a **branch** no nosso projeto, no meu caso ela fica assim:
"`AP-farofa-do-chef-atala`"

Exemplo:
```bash
$ cd receitas-a-la-git/

$ git branch AP-farofa-do-chef-atala

$ git checkout AP-farofa-do-chef-atala
```

![Alt text](imagens/4.png)

### 4.Adicionar a receita na pasta Menu:

Agora voce já pode digitar a sua receita. Para isso crie u arquivo de texto na pasta do repositorio local, abra seu editor de texto favorido e pode começar a digitar a receita.

Para nosso exemplo vou usar o notepad por sua siplicidade, no terminal que está aberto digite o comando `notepad` para abrir rapidamente o programa.
Vou digitar a receita no formato Markdown, para mais info sobre esse formato acesse **[aqui](https://pt.wikipedia.org/wiki/Markdown)**.
Quando finalizar salve o arquivo na pasta **Menu**, de um nome que referencie a receita.
No exemplo salvei como `"Farofa-do-Chef-Atala.md"`, a extenção `.md` faz referencia a formatação **Markdown**



