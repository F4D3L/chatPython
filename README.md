Aplicativo de Chat em Python
Este é um aplicativo de chat que permite que várias pessoas conversem em tempo real através de um servidor central.

Pré-requisitos:

Python 3 instalado em todas as máquinas que vão rodar o chat.
Configuração e Uso
Coloque todos os arquivos (server.py e client.py) em um mesmo diretório (pasta) no seu computador(Caso não estiver).

Configure o IP do Servidor:

Abra server.py e client.py com um editor de texto.
No arquivo server.py, defina o IP do host para o endereço IP da máquina que será o servidor:

host = "SEU_IP_AQUI"  # Substitua "SEU_IP_AQUI" pelo IP da máquina do servidor
port = 3308  # Porta que será usada para o chat

No arquivo client.py, faça a mesma coisa para a linha que conecta o cliente ao servidor:

client.connect(("SEU_IP_AQUI", 3308))  # Use o mesmo IP e porta do servidor

Execute o Servidor:

Abra os arquivos .bat e mude o diretório c: para o localizado em sua maquina
tanto para o servidor quanto para o cliente


Para sair, basta fechar a janela do cliente.

Observações:
Certifique-se de que todos os dispositivos estão conectados na mesma rede.
Se houver firewall ativo, permita o uso da porta 3308.