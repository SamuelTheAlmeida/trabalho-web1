Tecnologia em Análise e Desenvolvimento de Sistemas

Setor de Educação Profissional e Tecnológica - SEPT

Universidade Federal do Paraná - UFPR

---

*DS120 - Desenvolvimento de Aplicações Web 1*

Prof. Alexander Robert Kutzke

**[Instruções para submissão de tarefas e trabalhos](http://gitlab.tadsufpr.net.br/ds120-alexkutzke/ds120-material-2017-2/blob/master/instrucoes_submissao_tarefas_e_trabalhos.md);**

# Equipe
* [**Gustavo Kovalski Saporiti** @grr20175454](http://gitlab.tadsufpr.net.br/grr20175454)
* [**Samuel Toledo de Almeida** @grr20176288](http://gitlab.tadsufpr.net.br/grr20176288)
* [**Thiago Cezario** @grr20175458](http://gitlab.tadsufpr.net.br/grr20175458)

# Spotted

Spotted é uma ferramenta gratuita onde se pode deixar mensagens para que outros possam ler, parecido com anúncio de jornais. Você pode simplesmente desabafar, mandar uma cantada para aquele(a) garoto(a) de quem você gostou, jogar papo fora e até mesmo usar como achados e perdidos. A aplicação foi inspirada em páginas de redes sociais criadas nas universidades.


### Pré-requisitos
Para a instalação e funcionamento correto da aplicação, é necessário possuir as seguintes ferramentas:

```
Servidor Apache 2.x.x
MySQL 5.7.x
PHP 7.1

```
Para facilitar, recomendamos a utilização de utilização de um WAMP ou XAMP (Pacote com todos os programas necessários)


[WAMPServer - para Windows](http://www.wampserver.com/en/)  
[XAMPP - para Linux/Windows](https://www.apachefriends.org/xampp-files/7.1.11/xampp-linux-x64-7.1.11-0-installer.run)



## Instalação
* Com o git instalado
    1. Fazer um fork do projeto
    2. Na pasta www do servidor web, realizar um git clone do seu fork
    3. Abrir o arquivo 'db_credentials.php' e se necessário alterar com suas informações de acesso ao banco de dados.
    4. Executar o arquivo 'db_install.php' visitando a página no localhost. Certifique-se de estar com seu servidor web em execução.
    5. A aplicação estará pronta para uso.

* Sem o git
    1. Baixar o projeto compactado
    2. Na pasta www do servidor web, extrair os arquivos e pastas do projeto
    3. Abrir o arquivo 'db_credentials.php' e se necessário alterar com suas informações de acesso ao banco de dados.
    4. Executar o arquivo 'db_install.php' visitando a página no localhost. Certifique-se de estar com seu servidor web em execução.
    5. A aplicação estará pronta para uso.

## Utilizando a aplicação
Ao acessar a página inicial, você irá visualizar os posts mais recentes, e poderá fazer login ou se cadastrar para enviar um novo post.
### Para se cadastrar
* Na página inicial, clique na opção Cadastrar no menu de navegação
* Insira um nickname, uma senha e a confirmação de senha. Opcionalmente, pode-se adicionar seu número de telefone e endereço de email
* Ao clicar em cadastrar, se tudo estiver de acordo, você será logado e redirecionado para a página inicial

### Para fazer login
* Na página inicial, clique na opção Login no menu de navegação
* Insira corretamente seu nickname e senha e clique em Login
* Você será redirecionado para a página inicial

### Enviando um novo spotted
* No menu de navegação, clique na opção Novo Spotted (é necessário estar logado para acessar)  
  
Selecione uma categoria para o post. Por padrão, estas são as tags disponíveis:  

* "Viu aquela pessoa e quer mandar uma cantada"
* "Coisas aleatórias que não são cantadas direcionadas"
* "Coisas de utilidade pública"
* "Achou ou perdeu alguma coisa?"
* "Pra vc que mora longe e precisa de uma carona pra ir pras aulas"

* O número máximo de caracteres para um post é de 300 caracteres.

Após enviar um spotted, ele ficará pendente de aprovação por um administrador.

### Aprovando spotteds
Todos os posts enviados devem ser aprovados antes de serem publicados.  
Contas de administradores estão habilitadas para acessar a página de aprovação.
* Na página de login, entre com uma conta de administrador. Por padrão, foi predefinida uma conta:
```
    nickname: master  
    senha: 123
```

No menu de navegação, clique no seu nickname "master". Você será redirecionado para a página do administrador.  

Na página do administrador, você verá todos os posts pendentes de aprovação, e poderá aprovar, modificar ou rejeitar.

* Ao aprovar, o post será publicado na página inicial
* Ao modificar, o post terá seu conteúdo alterado e continuará pendente de aprovação
* Ao rejeitar, o post será removido da base de dados

### Alterando sua senha
* Na barra de navegação, clique na engrenagem no canto superior direito.
* No formulário, digite seu nickname, sua senha atual, e a nova senha desejada, respectivamente, e clique em Alterar
* O tamanho mínimo da senha é de 8 caracteres, e o usuário master não pode ter sua senha alterada.

---

## Ferramentas utilizadas no desenvolvimento
* [HTML5](https://developer.mozilla.org/pt-BR/docs/Web/HTML/HTML5) - Conteúdo das páginas e validação front-end
* [CSS3](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS3) - Front-end
* [Semantic UI](https://semantic-ui.com/collections/grid.html) - Framework front-end, utilizado para o grid de exibição dos posts
* [Font Awesome)](http://fontawesome.io/) - Biblioteca de ícones utilizada no header
* [JavaScript](https://www.javascript.com/) - Validação front-end e máscara de telefone
* [jQuery](https://jquery.com/) - Front-end
* [PHP 7.1](http://www.php.net/) - Back-end
* [MySQL](https://www.mysql.com/) - Banco de Dados utilizado
* [Apache](https://www.apache.org/) - Servidor Web utilizado no desenvolvimento


