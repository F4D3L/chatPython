
# Socket / Threading Chat - Python

Este é um programa python para criação de um chat em grupo. O programa funciona em computadores diferentes por meio da utilização de Sockets e Threading.



## Funcionalidades

- Chat ao vivo com múltiplas pessoas na mesma sala.
- Mensagens privadas entre usuários de uma sala.
- Conexão com o servidor a partir do hosting em roteadores. 



## Instalação
Para que o programa funcione corretamente você deve ter o Python 3.11.4 ou superior instalado no seu computador. Clone o projeto para seu local desejado e acesse a pasta utilizando o comando "cd" junto com o caminho para o diretório onde você colocou as pastas.

```bash
  git clone https://github.com/F4D3L/chatPython.git
  cd "C:\..."

```
    
## Rodando localmente

Com o projeto clonado, você precisará editar o IP e a Porta para que o programa funcione. Com o editor de código de sua preferência, abra a pasta, localize os arquivos `cliente.py` e `server.py` e abra no editor. Na linha 8 do arquivo `client.py` e na linha 5 do arquivo `server.py` você irá ver a faixa de código: 

```bash
  server.bind(("127.0.0.1", 3307)) #Associando Socket a uma porta e servidor
```

Para rodar localmente o programa, você deve alterar o IP para IPV4 da sua máquina. O IPV4 pode ser encontrado utilizando o comando `ipconfig` dentro do CMD ou dentro das informações de rede nas configurações de rede do seu computador. Com o seu IP em mãos, substitua dentro do local indicado tanto no arquivo `client.py` e `server.py`. A porta 3307 pode ser utilizada, mas caso já esteja em uso, tente trocar para a porta 3306. Com os IPs e portas configurados corretamente, você precisará de 3 CMDs abertos para conseguir realizar o teste local. Abra os 3 CMDs, entre na pasta utilizando o comando `cd C:\..` e coloque o caminho para sua pasta. Com essa etapa finalizada, você deverá digitar os seguinte comando em um dos prompts abertos:
```
python server.py
```
Com isso, deverá aparecer a mensagem "Servidor está funcionando e rodando...". Após checar que o servidor está funcionando, digite nos outros dois prompts o comando:
```
python client.py
```
Insira um nickname na caixa de texto que aparecerá na sua tela e o cheque se a janela do chat é aberta. Com todos os passos executados corretamente, você pode enviar suas mensagens e checar em ambas as janelas se elas aparecem. Caso queira testar a funcionalidade de enviar uma mensagem privada dentro do chat, repita o procedimento de abrir mais um prompt, entrar na pasta onde se encontram os arquivos, digitar o comando `python client.py` e abrir uma nova janela. Com essa janela aberta você pode enviar mensagens privadas digitando `@nickname` da pessoa que deseja enviar a mensagem privada.





## Apêndice

Observação: Se houver um firewall ativo, permita o uso da porta que será utilizada na execução do programa.

