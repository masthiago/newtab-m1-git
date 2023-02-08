# NewTab Academy - Módulo 1

## Git, HTML e CSS + Gestão de tempo 

### Resumo sobre o Git e seus principais comandos.

#### Versionadores

Os versionadores de arquivos são ferramentas que ajudam os desenvolvedores a controlar as alterações em seus projetos de software. Eles mantêm uma história de todas as alterações feitas nos arquivos código ou de outros tipos e permitem que os desenvolvedores revertam para versões anteriores se necessário. Além disso, eles também ajudam a garantir a colaboração eficiente entre equipes de desenvolvimento, pois permitem que vários desenvolvedores trabalhem no mesmo projeto simultaneamente. Alguns dos versionadores de código mais comuns são Git, SVN e também o Mercurial.

#### Git

Git é um sistema de controle de versão de código aberto que permite gerenciar e rastrear mudanças em arquivos de forma distribuída. É amplamente utilizado em todo o mundo e é uma ferramenta vital para a colaboração eficiente entre equipes, principalmente de desenvolvimento de software.

Git permite confirmar (commit) e rastrear as mudanças feitas em arquivos de código fonte, bem como criar ramificações (branches) para testar novas funcionalidades sem afetar a versão principal do código. Além disso, Git permite fundir (merge) ramificações, reverter mudanças, colaborar com outros desenvolvedores e muito mais.

A importância de Git é inegável. É uma ferramenta fundamental para a gestão de projetos de software, ajudando a garantir a qualidade, a integridade e a segurança do código. Além disso, permite aos desenvolvedores trabalhar juntos com eficiência, o que é fundamental em projetos de equipe. Portanto, aprender Git é uma habilidade valiosa para qualquer desenvolvedor.


#### Configurações

As configurações `user.name` e `user.email` são informações importantes que o Git usa para identificar o autor dos commits em um repositório. Estas configurações permitem que o Git saiba quem é responsável por cada um dos commits e facilita a colaboração entre os membros da equipe.

A configuração `user.name` é usada para especificar o nome completo do autor das confirmações, enquanto a configuração `user.email` é usada para especificar o endereço de e-mail do autor.

```
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

Observe que o argumento `--global` é usado para definir essas configurações globalmente para todos os repositórios Git no sistema. Se você quiser definir essas configurações apenas para um repositório específico, basta remover o argumento `--global`.

Também é importante destacar que essas configurações são armazenadas no arquivo de configuração global do Git, localizado em `~/.gitconfig` no sistema operacional Linux ou macOS e no Windows fica em `C:\Users\<username>\.gitconfig`. Caso precise mudar as configurações, basta editar esse arquivo ou executar novamente o comando `git config`.


#### O .gitignore

O arquivo `.gitignore` é usado para ignorar certos arquivos e pastas que não devem ser gerenciados pelo Git. Ele é criado na raiz do seu repositório Git e é usado para especificar quais arquivos e pastas o Git deve ignorar ao realizar um commit.

Por exemplo, se você tem arquivos temporários ou de log em seu repositório que não devem ser versionados, pode especificar isso no arquivo `.gitignore`. Aqui está um exemplo de um arquivo `.gitignore`:

```
# Todos os arquivos swp
*.swp

# Todos os arquivos de log
*.log

# Arquivo único
arquivo.txt

# Pastas
node_modules/
```

Observe que cada linha no arquivo `.gitignore` especifica um arquivo ou pasta que deve ser ignorado. As linhas que começam com o caractere de comentário (`#`) são ignoradas. Além disso, você pode usar *comodins* (`*`) para ignorar vários arquivos ao mesmo tempo.


#### Tags

As tags no Git são marcadores especiais que apontam para um commit específico em um repositório Git. Elas são usadas para marcar versões estáveis ou importantes do código, para que possam ser facilmente encontradas e referidas mais tarde.


#### Repositórios remotos

Os repositórios remotos no Git são cópias do seu repositório local que estão armazenadas em outro lugar, geralmente em um servidor na nuvem. Eles permitem que você compartilhe o código com outros desenvolvedores, faça backup de seu código e facilite a colaboração em projetos em equipe.

Alguns serviços de repositórios remotos:

* **GitHub** é o maior e mais popular serviço de repositórios remotos do Git, oferecendo ferramentas avançadas de colaboração, controle de versão, gerenciamento de issues (bugs) e muito mais.

* **GitLab** é uma plataforma completa para gerenciamento de ciclo de vida de desenvolvimento de software, incluindo recursos de repositórios remotos, integração contínua e implantação.

* **Bitbucket** oferece recursos avançados de colaboração, integração contínua e gerenciamento de equipes.

* **Amazon Web Services (AWS) CodeCommit** é um serviço fornecido pelo Amazon Web Services, que permite armazenar, gerenciar e compartilhar seu código com segurança.


#### Pull Request

Um pull request (solicitação de alteração) no Git é uma maneira de colaborar com outros desenvolvedores em um projeto. É uma forma de solicitar que as alterações que você fez em sua branch sejam mescladas com a branch principal do projeto.

Aqui está o processo básico para criar um pull request:

1. Crie uma nova branch para fazer as alterações que você deseja contribuir.

2. Faça as alterações em sua branch e envie (push) as mudanças para o seu repositório remoto.

3. Vá ao site do repositório remoto (GitHub, GitLab, Bitbucket, etc.) e clique na opção para criar um pull request.

4. Escolha a sua branch como a fonte do pull request e a branch principal do projeto como o destino.

5. Adicione uma descrição detalhada das alterações que você fez e envie o pull request.

6. Outros desenvolvedores no projeto receberão a notificação do pull request e poderão revisar o código, fazer comentários ou solicitar alterações.

7. Se as alterações forem aprovadas, o mantenedor do projeto pode mesclar as alterações na branch principal.

O uso de pull requests é uma boa prática para garantir que o código seja revisado por outros antes de ser mesclado na branch principal, o que ajuda a garantir a qualidade do código e a evitar erros.


##### GitHub Pages

GitHub Pages é um serviço de hospedagem de páginas da web oferecido pelo GitHub. Ele permite que você publique páginas estáticas diretamente a partir do seu repositório GitHub e acesse-as através de um URL público. É uma forma fácil e gratuita de compartilhar informações, documentação ou projetos com o público em geral.

O GitHub Pages suporta vários tipos de páginas, incluindo páginas estáticas, páginas Jekyll e projetos do GitHub. Além disso, você pode personalizar seu site usando temas e ferramentas de personalização fornecidos pelo GitHub.

Para configurar o GitHub Pages para seu projeto os passos são

1. Crie um novo repositório no GitHub ou use um já existente.

2. Vá para as configurações do repositório e clique na seção "GitHub Pages".

3. Selecione uma branch (geralmente a branch principal) para ser a fonte de sua página.

4. Escolha um modelo de tema (opcional) e clique no botão "Save".

5. Adicione os arquivos HTML, CSS e JavaScript para sua página na branch selecionada.

6. Confirme que as alterações foram publicadas e acesse o URL da sua página, que geralmente é algo como `https://<seu-usuário>.github.io/<seu-repositório>`.


#### Git GUIs

Uma GUI (interface gráfica do usuário) para Git é um tipo de software que fornece uma interface visual para o usuário interagir com o Git. Em vez de usar comandos de linha de comando, você pode realizar operações como adicionar arquivos, fazer commits, ver históricos de branch e resolver conflitos através de cliques e menus.

Algumas das principais GUIs para Git incluem:

* **Sourcetree** é uma GUI poderosa e fácil de usar para Git, com recursos avançados como visualização de histórico de branch e resolução de conflitos.

* **GitKraken** é uma GUI para Git que oferece uma interface visual intuitiva, recursos de colaboração e integração com outras ferramentas.

* **Git GUI** é uma GUI para Git que vem incluída com o Git e oferece uma interface gráfica básica para operações como adicionar arquivos, fazer commits e visualizar históricos de branch.

* **GitEye** é uma GUI para Git que oferece uma interface gráfica intuitiva, recursos de visualização de histórico de branch e integração com outras ferramentas.


* **GitHub Client** é uma aplicação de desktop que fornece uma interface gráfica para o usuário interagir com o GitHub, uma plataforma popular para hospedagem de repositórios Git. Com o GitHub Client, você pode fazer o upload de repositórios, clonar repositórios existentes, realizar pull requests e resolver conflitos, entre outras tarefas, sem precisar digitar comandos de linha de comando.


* **SmartGit** é uma GUI (interface gráfica do usuário) para Git que fornece uma interface visual para o usuário interagir com o Git. Ele oferece uma variedade de recursos, como visualização de histórico de branch, resolução de conflitos, gerenciamento de pull requests e integração com outras ferramentas. Além disso, SmartGit é uma das poucas GUIs para Git que oferece suporte a SVN (Subversion), o que significa que você pode usar a mesma interface para trabalhar com repositórios Git e SVN.

Essas são apenas algumas das GUIs para Git disponíveis. A escolha da GUI ideal para você dependerá de suas necessidades e preferências pessoais. Algumas pessoas preferem usar GUIs para tornar o trabalho com o Git mais fácil e visual, enquanto outras preferem usar o Git através de comandos de linha de comando para ter mais controle sobre suas operações.


#### Gitflow

Git Flow é uma metodologia para gerenciamento de branchs no Git que define uma estrutura para o fluxo de trabalho de equipes em projetos de software. Ele sugere a criação de diferentes tipos de branchs para diferentes fases do desenvolvimento do software, como desenvolvimento, lançamento e manutenção.

O Git Flow é uma metodologia muito útil para equipes que trabalham em projetos de software, pois ajuda a manter a organização do código e a garantir a qualidade e estabilidade do software. No entanto, ele pode ser um pouco complexo para equipes menores ou para projetos menos complexos, então é importante avaliar se ele é a melhor opção para o seu projeto antes de implementá-lo.


#### Comandos

Aqui estão alguns dos principais comandos do Git com exemplos:

* **git init** inicializa um novo repositório local Git na pasta atual.

    ```
    git init
    ```

* **git clone** clona um repositório Git remoto para a sua máquina local.

    ```
    git clone https://github.com/usuario/repositorio.git
    ```

* **git add** Adiciona um arquivo ao stage para que possa ser incluído no próximo commit.

    ```
    git add arquivo.txt
    ```

* **git commit** confirma (salva) as mudanças no histórico de confirmações do repositório local.

    ```
    git commit -m "Adicionando arquivo arquivo.txt"
    ```

* **git push** envia os commits do repositório local para o repositório remoto.

    ```
    git push origin main
    ```

* **git pull** baixa as mudanças do repositório remoto para o seu repositório local.

    ```
    git pull origin main
    ```

* **git branch** gerencia branches no repositório.

    ```
    git branch nome_branch
    ```

* **git checkout** alterna entre branches ou commits.

    ```
    git checkout uma_branch
    ````

* **git merge** unifica uma branch com a branch atual.

    ```
    git merge outra_branch
    ```

* **git log** exibe o histórico de commits do repositório.

    ```
    git log
    ```

* **git tag** adiciona uma tag para registar um commit de versão.

	```
	git tag v1.0
	```

* **git status** informa o status dos arquivos no repositório local
	```
	git status
	```

* **git diff** exibe as diferenças entre arquivos alterados atualmente e o seu status anterior

	```
	git diff arquivo.txt
	```
	