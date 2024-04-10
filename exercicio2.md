1. Backup manual da pasta contendo os arquivos do servidor web:

Utilizei o comando sudo rsync -av /caminho/para/fonte /caminho/para/destino para copiar os arquivos da pasta do servidor web para um diretório diferente.
Substituí /caminho/para/fonte pelo caminho real da pasta contendo os arquivos do servidor web e /caminho/para/destino pelo caminho do diretório onde desejo armazenar o backup.
2. Automatização do processo de backup utilizando o serviço cron:

Editei as tarefas cron utilizando o comando crontab -e.
Adicionei uma linha ao arquivo cron para agendar a execução do backup em intervalos regulares. Por exemplo:

0 2 * * * sudo rsync -av /caminho/para/fonte /caminho/para/destino
Isso executará o backup todos os dias às 2 da manhã.
3. Verificação do funcionamento do backup:

Adicionei um novo arquivo à pasta do servidor web para simular uma mudança nos arquivos.
Esperei até o horário agendado para o backup e verifiquei se a pasta de destino foi atualizada com sucesso após a execução do backup.
Confirmei que o novo arquivo adicionado à pasta do servidor web estava presente na pasta de destino, o que indica que o backup automatizado funcionou conforme esperado.
Conclusão:

O processo de backup manual foi realizado com sucesso, seguido pela automatização do backup usando o serviço cron.
Verifiquei o funcionamento do backup adicionando um novo arquivo à pasta do servidor web e confirmando que o mesmo foi refletido na pasta de destino após a execução do backup agendado.
