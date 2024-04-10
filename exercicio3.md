1. Criação de dois usuários (um regular e um superusuário):

Utilizei o comando sudo adduser nome_do_usuario para adicionar um novo usuário. Por exemplo:
Copy code
sudo adduser usuario_regular
Em seguida, utilizei o comando sudo adduser nome_do_usuario sudo para adicionar o usuário recém-criado ao grupo sudo e conceder permissões de superusuário. Por exemplo:
Copy code
sudo adduser usuario_regular sudo
Repeti o processo para criar um superusuário, substituindo usuario_regular pelo nome do superusuário desejado.
2. Definição de limite mínimo de caracteres para as senhas:

Utilizei a ferramenta passwd para definir ou modificar as senhas dos usuários.
Executei o comando sudo passwd nome_do_usuario para definir a senha de um usuário. Por exemplo:
Copy code
sudo passwd usuario_regular
Durante a definição das senhas, garanti que elas atendessem ao limite mínimo de caracteres exigido pela política de segurança do sistema.
3. Definição de diretórios iniciais para cada usuário:

Verifiquei os diretórios iniciais padrão de cada usuário no arquivo /etc/passwd. O diretório inicial de cada usuário é especificado no final de cada linha.
Modifiquei os diretórios iniciais, se necessário, editando o arquivo /etc/passwd.
4. Verificação das permissões de acesso aos diretórios iniciais:

Utilizei o comando ls -l /caminho/do/diretório para listar as permissões de acesso aos diretórios iniciais de cada usuário.
Garanti que apenas os usuários apropriados tivessem permissão de acesso aos seus respectivos diretórios iniciais.
