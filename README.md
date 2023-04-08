Descrição:
1: Remote_BackDoor.ino:
Cria uma conta com privilégios de administrador com o nome blanka e passwd Ping@123. Também o oculta da tela de login e ativa a área de trabalho remota para ser acessível a partir de um local remoto.

Testado em:
SO : Windows 10
Usuário : Admin User
Hardware : ATtiny85 (chinês)

2: GoodOl' BackDoor.ino:
Com base no antigo truque de backdoor da chave adesiva, adicionando uma chave de registro em vez de substituir o arquivo no diretório system32. Após a execução bem-sucedida, pressione shift 5 vezes na tela de login e o prompt de comando aparecerá com privilégios de administrador.

Para remover o backdoor, execute o seguinte comando no prompt de comando com privilégios de administrador e o backdoor será removido.

REG DELETE "HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Image File Execution Options\sethc.exe

Testado em:
SO : Windows 10/7
Usuário : Usuário administrador
Hardware : ATtiny85 (chinês)
