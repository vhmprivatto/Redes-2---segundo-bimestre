# Atividade-redes2-segundo-bimestre

Trabalho de REDES 2 baseado no tutorial do canal de YouTube 'Tech With Tim'

Intergrantes:
	
		Daiane Maria de Freitas       RA 77232
		Everton Eduardo do Nascimento RA 82555
		Vitor Hugo Monteiro Privatto  RA 93453
		Caio Eduardo Chiari           RA 93308


As partes explicadas nesse documento de texto são as relacionadas a conectividade.

Para o funcionamento desse programa é necessário atribuir o ip da máquina em 'server.py' e 'network.py'.

--------------------------------------------------------------------------------------------------------------------------------                          
                                                        SERVER
                                                        
linha 5 - é definido IP.

linha 6 - é definido a porta.

linha 8 - criação do socket ( tipo AF_INET = conexão e SOCK_STREAM = tipo de fluxo de String através do server.

linha 11 - BIND no server e porta, há um except para verificar se é possível.

linha 16 - ouve as conexões e abre a porta para multiplas conexões, o valor entre parenteses indica a quantidade, se não for passado valor então é ilimitado.

linha 19 - médoto def responsável por dividir um String (ex 85 ,98) em duas Strings (String 85) e (String 98) para que seja possível a conversão em INT em uma TUPLA.

linha 24 - método converte TUPLA em STRING.

linha 27 - inicia uma lista que salva as informações de jogador na memória do server.
linha 

29 - método que converte em String e envia ao jogador 
que lê a String e converte em posição e a atualiza.

linha 35 - toda vez que o jogado receber algum dado (no caso, no máximo 2048 bits) de outro jogador, esse também envia os dados da posição e transforma em TUPLA.

linha 36 - atualiza a posição do jogador atual.

linha 51 - codifica a String para envio

linha 60 - incrementa quando uma nova conexão é recebida.

linha 62 - loot que procura continuamente por conexões e as pega e inicia uma nova thread.

linha 63 - aceita qualquer conexão e guarda a conexão e endereço.

linha 66 - começa unma nova thread com a conexão.

--------------------------------------------------------------------------------------------------------------------------------
                                                     NETWORK


linha 
3 - classe Network - retorna o ID como se estivesse guardado nesse objeto, é necessário enviar um ID para cada cliente para identiticação.

linha 18 - fará a conexão.

linha 19 - realiza o handshake e decodifica a String.

linha 23 - envia informações para o server e mantem o loop de envio-recebimento


-------------------------------------------------------------------------------------------------------------------------------- 
                                                      CLIENT

linha 45 - este método divide(split) uma string (ex 85,98) em duas (String 85) e (string 98) e então retorna a converção para int em uma TUPLA.

linha 50 - transforma e retorna a TUPLA em String.

linha 64 - importa a classe Network.

linha 65 - recebe uma posição do server em String.

linha 71 - envia a posição atual para o server e recebe a posição toda a vez que o 
frame é atualizado.








  
