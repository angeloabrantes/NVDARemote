# Acesso Remoto do NVDA
Versão 2.3

Bem-vindo ao extra Acesso Remoto do NVDA \[NVDA Remote Access\], que permite a ligação com outro computador que esteja a executar o leitor de ecrã livre NVDA. Não faz diferença se  estiver do outro lado da sala ou do outro lado do mundo. A ligação é simples e há muito poucos comandos para memorizar.  pode ligar-se ao computador de outra pessoa ou permitir que uma pessoa confiável se conecte ao seu computador para realizar manutenção de rotina, diagnosticar um problema ou fornecer-lhe elementos de aprendizagem.

## Antes de começar

 precisará ter instalado o NVDA nos dois computadores e obter o extra de Acesso Remoto do NVDA.
A instalação do NVDA e do extra de Acesso Remoto é realizada de modo padrão. Se  precisar de mais informações, podem ser encontradas no Guia do Usuário do NVDA.

## Actualizar

Ao actualizar o extra, se  instalou o acesso remoto do NVDA na área de trabalho segura, é recomendável actualizar também a cópia na área de trabalho segura.
Para fazer isso, primeiro, actualize o extra existente. Em seguida, abra o menu do NVDA, preferências, Configurações Gerais e pressione o botão rotulado "Usar configurações guardadas actualmente no logon e noutros ecrãs seguros (requer privilégios administrativos)".

## Iniciar uma sessão remota através de um servidor de retransmissão

### No computador a ser controlado
1. Abra o menu NVDA, Ferramentas, Remoto, ligar.
2. Escolha cliente, no primeiro botão de opção.
3. Seleccione Permitir que esta máquina seja controlada, no segundo conjunto de botões de opção.
4. No campo servidor, escreva o nome do servidor \[nome ou endereço\] do servidor ao qual  se está  a ligar, por exemplo, nvdaremote.com. Quando o servidor específico usa uma porta alternativa,  pode inserir o host no formato &lt;host&gt;:&lt;porta&gt;, por exemplo nvdaremote.com:1234.
5. Escreva um código \[senha ou chave\] no campo código ou pressione o botão gerar código.
O código é o que os outros utilizarão para controlar o seu computador.
A máquina a ser controlada e todos os seus clientes precisam de usar o mesmo código.
6. Pressione ok. Depois de concluído,  ouvirá um tom e será ligado.

### Na máquina que deve ser o computador controlador
1. Abra o menu NVDA, Ferramentas, Remoto, ligar.
2. Escolha cliente, no primeiro botão de opção.
3. Seleccione Controlar outra máquina, no segundo conjunto de botões de opção.
4. No campo servidor, escreva o nome do servidor \[nome ou endereço\] do servidor ao qual  se está  a ligar, por exemplo, nvdaremote.com. Quando o servidor específico usa uma porta alternativa,  pode inserir o servidor no formato &lt;servidor&gt;:&lt;porta&gt;, por exemplo nvdaremote.com:1234.
5. Escreva um código \[senha ou chave\] no campo código ou pressione o botão gerar código.
A máquina a ser controlada e todos os seus clientes precisam de usar o mesmo código.
6. Pressione ok. Depois de concluído,  ouvirá um tom e será ligado.

## Ligações directas

A opção servidor, no diálogo de ligação, permite configurar uma ligação directa.
Depois de seleccionar essa opção, seleccione em que situação entra na ligação: computador controlado ou controlador
A outra pessoa  liga-se   usando o oposto.

Depois que o posicionamento dos computadores for seleccionado,  pode usar o botão Obter IP externo para obter seu endereço IP externo e
verificar se a porta inserida no campo da porta está encaminhada corretamente.
Se o portcheck \[verificação de porta\] detectar que a sua porta (6837 por padrão) não está acessível, um aviso será mostrado.
Reencaminhe a sua porta e tente novamente.
Nota: O processo para encaminhamento de portas está fora do escopo deste documento. Consulte as informações fornecidas com o seu roteador, para obter mais instruções.

Escreva um código \[senha ou chave\] no campo código ou pressione gerar código. A outra pessoa precisará do seu IP externo, junto com o código, para se ligar. Se  inseriu uma porta diferente da padrão (6837) no campo porta, verifique se a outra pessoa anexa a porta alternativa ao endereço do servidor no formato &lt;ip externo&gt;:&lt;porta&gt;.

Ao pressionar OK,  será ligado.
Quando a outra pessoa se ligar,  poderá usar o acesso Remoto do NVDA normalmente.

## Controlar a máquina remota

Depois da  sessão ser iniciada, o utilizador da máquina controladora pode pressionar f11 para começar a controlar a máquina remota (por exemplo, enviando comandos de teclado ou entrada braille).
Quando o NVDA diz "a controlar a máquina remota", as teclas do teclado e da linha braille pressionadas irão para a máquina remota. Além disso, quando a máquina controladora estiver a usar uma linha braille, as informações da máquina remota serão mostradas no display da linha. Pressione f11 novamente para parar de enviar as teclas e voltar para a máquina controladora.
Para uma melhor compatibilidade, verifique se os esquemas \[leiautes\] de teclado das duas máquinas correspondem.

## Compartilhar a sua sessão

Para compartilhar um link, para que outra pessoa possa ingressar facilmente na sua sessão de acesso Remoto do NVDA, selecione Copiar link no menu do Acesso Remoto.
Se  estiver ligado como o computador de controlo, esse link permitirá que outra pessoa se ligue e seja também controlada.
Se, em vez disso,  configurou o seu computador para ser controlado, o link permitirá que as pessoas com quem  o compartilha controlem sua máquina.
Muitos aplicativos permitem que os utilizadores activem esse link automaticamente, mas se ele não for executado a partir de um aplicativo específico, ele poderá ser copiado para a área de transferência e executado no diálogo executar.

## Enviar Control+Alt+Del

Ao enviar teclas, não é possível enviar a combinação Control+Alt+del normalmente.
Se  precisar enviar Control+Alt+Del e o sistema remoto estiver na área de trabalho segura, use esse comando.

## Controlar remotamente um computador autónomo

Às vezes,  pode querer controlar um dos seus computadores remotamente. Isto é especialmente útil se  estiver a viajar e desejar controlar o seu PC doméstico a partir do seu laptop. Ou então,  pode controlar um computador numa divisão da sua casa enquanto está sentado do lado de fora com outro PC. Um pouco de preparação avançada torna isso conveniente e possível. Vejamos:
1. Aceda ao menu do NVDA, escolha Ferramentas e, em seguida, Acesso Remoto. Por fim, pressione Enter em Opções.
2. Marque a caixa que diz "ligar automaticamente ao servidor de controlo, ao iniciar o NVDA".
3. Seleccione se deseja usar um servidor de retransmissão remota ou hospedar localmente a ligação.
4. Seleccione Permitir que esta máquina seja controlada, no segundo conjunto de botões de opção.
5. Se  hospedar a ligação, precisará garantir que a porta inserida no campo da porta (6837 por padrão) na máquina controlada possa ser acedida pelas máquinas controladoras.
6. Se  deseja usar um servidor de retransmissão, preencha os campos servidor e Código, tecle tab até OK e pressione Enter. A opção Gerar código não está disponível nessa situação. É melhor criar um código do qual  se lembre para poder usá-lo facilmente em qualquer local remoto.

Para uso avançado,  também pode configurar o Acesso Remoto do NVDA para se ligar automaticamente a um servidor de retransmissão local ou remoto no modo de controlo. Se desejar, selecione Controlar outra máquina no segundo conjunto de botões de opção.

Nota: A ligação automática nas opções relacionadas à inicialização no diálogo Opções não se aplica até que o NVDA seja reiniciado.

## Silenciar a fala no computador remoto
Se  não deseja ouvir a voz do computador remoto ou sons específicos do NVDA, basta aceder ao menu NVDA, Ferramentas e Acesso Remoto. Seta para baixo até Silenciar computador remoto e pressione Enter. Observe que esta opção não desactivará a saída braille remota para o ecrã de controlo quando a máquina controladora estiver a enviar teclas.

## Terminar uma sessão remota

Para encerrar uma sessão remota, faça o seguinte:
1. No computador de controlo, pressione F11 para parar de controlar a máquina remota.  deve ouvir ou ler a mensagem: "a Controlar a máquina local". Se  ouvir ou ler uma mensagem de que está a controlar a máquina remota, pressione F11 mais uma vez.
2. Aceda ao menu do NVDA, depois Ferramentas, Acesso Remoto e pressione Enter, em desligar.

## Enviar texto da área de transferência

A opção Enviar texto da área de transferência no menu Acesso remoto permite enviar o texto da área de transferência de uma máquina para outra.
quando esta opção estiver activada, qualquer texto da área de transferência poderá ser enviado da máquina controladora para a máquina controlada e vice-versa.
Isso pode ser feito pressionando o atalho NVDA+Control+Shift+C.

## Configurar o Acesso Remoto do NVDA para funcionar na Área de Trabalho Segura

Para que o Acesso Remoto do NVDA funcione na área de trabalho segura, o extra deve ser instalado no NVDA em execução na área de trabalho segura.
1. No menu do NVDA, seleccione Preferências e Configurações.
2. Na categoria Geral, tecle Tab até o botão Usar configurações guardadas actualmente no Logon e outros ecrãs seguros (requer privilégios administrativos) e pressione Enter.
3. Responda Sim às solicitações sobre a cópia das suas configurações e sobre a cópia de plug-ins e responda à solicitação de Controle de Conta de Usuário que possa aparecer.
4. Quando as configurações forem copiadas, pressione Enter no botão OK para fechar. Tecle tab até OK e pressione Enter mais uma vez para sair da caixa de diálogo.
Depois do Acesso Remoto do NVDA estar instalado na área de trabalho segura, se  estiver a ser controlado numa sessão remota,
 terá acesso de voz e braille à área de trabalho segura quando alternar.

## Contribuições
Gostaríamos de agradecer aos seguintes colaboradores, entre outros, que ajudaram a tornar o projecto Acesso Remoto do NVDA uma realidade.

* Hai Nguyen Ly
* Chris Westbrook
* Thomas Huebner
* John F Crosotn III
* Darrell Shandrow
* D Williams
* Matthew McCubbin
* Jason Meddaugh
* ABDULAZIZ ALSHMASI.
* Tyler W Kavanaugh
* Casey Mathews
* Babbage B.V.
* Leonard de Ruijter
* NV Access
* Reef Turner

## Registo de Alterações \[Change Log\]

### Versão 2.3
* Migrado para Python 3
* Suporte ao Python 2 abandonado
* Actualização para atender à API alterada no NVDA 2019.3, incluindo:
  - Refactorador de voz
  - Alterações para linhas braille

### Versão 2.2

* Suporte IPv6
* Suporte para o novo NVDA 2018.3 e versões anteriores
* Suporte para comandos \[gestos\] específicos de modelos de linhas braille

### Versão 2.1

* Corrigido o problema da ligação não ser guardada, ao permitir que esta máquina seja controlada
* Adicionado um script para enviar conteúdo da área de transferência com NVDA+Control+Shift+C
* A entrada Braille agora funciona no modo de navegação
* Suporte a comandos \[gestos\] específicos de modelos de linhas braille
* Os bipes gerados pelo Remoto NVDA não bloqueiam mais o NVDA

### Versão 2.0

* Suporte para Braille remoto
* Suporte para links nvdaremote://
* Diálogos modificados para estarem em conformidade com o restante do NVDA
* Corrigido portcheck \[verificação de porta\] para apontar para um domínio que controlamos, portcheck.nvdaremote.com
* Suporte para ligar automaticamente a um servidor de controlo no modo mestre \[master \]
* Corrigido erro de renderização na documentação
* Actualiza à versão 2 do protocolo, que inclui um campo de origem em todas as mensagens remotas
* Limpeza significativa de código, permitindo modificações mais fáceis, no futuro

## Alterando o Acesso Remoto do NVDA

 pode clonar este repositório para fazer alterações no NVDA Remote.

### Dependências de terceiros
Podem ser instalados com o pip:
- Markdown
- scons
- python-gettext

### Empacotar o extra para distribuição:

1. Abra uma linha de comando, mude para a raíz deste repositório
1. Execute o comando **scons**. O extra criado, se não houver erros, é colocado no directório actual.
