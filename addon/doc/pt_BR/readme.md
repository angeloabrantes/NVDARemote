# Acesso Remoto do NVDA
Versão 2.3

Bem-vindo ao complemento Acesso Remoto do NVDA \[NVDA Remote Access\], que permite a conexão com outro computador que esteja executando o leitor de tela livre NVDA. Não faz diferença se você está do outro lado da sala ou do outro lado do mundo. A conexão é simples e há muito poucos comandos para memorizar. Você pode se conectar ao computador de outra pessoa ou permitir que uma pessoa confiável se conecte ao seu computador para realizar manutenção de rotina, diagnosticar um problema ou fornecer treinamento.

## Antes de começar

Você precisará ter instalado o NVDA nos dois computadores e obter o complemento de Acesso Remoto do NVDA.
A instalação do NVDA e do complemento de Acesso Remoto é padrão. Se você precisar de mais informações, isso pode ser encontrado no Guia do Usuário do NVDA.

## Atualizando

Ao atualizar o complemento, se você instalou o acesso remoto do NVDA na área de trabalho segura, é recomendável atualizar também a cópia na área de trabalho segura.
Para fazer isso, primeiro atualize o complemento existente. Em seguida, abra o menu do NVDA, preferências, Configurações Gerais e pressione o botão rotulado "Usar configurações salvas atualmente no logon e em outras telas seguras (requer privilégios administrativos)".

## Iniciando uma sessão remota através de um servidor de retransmissão

### No computador a ser controlado
1. Abra o menu NVDA, Ferramentas, Acesso Remoto, Conectar.
2. Escolha cliente no primeiro botão de opção.
3. Selecione Permitir que esta máquina seja controlada no segundo conjunto de botões de opção.
4. No campo host, digite o host \[nome ou endereço\] do servidor ao qual você está se conectando, por exemplo, nvdaremote.com. Quando o servidor específico usa uma porta alternativa, você pode inserir o host no formato &lt;host&gt;:&lt;porta&gt;, por exemplo nvdaremote.com:1234.
5. Digite um código \[senha ou chave\] no campo código ou pressione o botão gerar código.
O código é o que os outros utilizarão para controlar seu computador.
A máquina a ser controlada e todos os seus clientes precisam usar o mesmo código.
6. Pressione ok. Depois de concluído, você ouvirá um tom e será conectado.

### Na máquina que deve ser o computador controlador
1. Abra o menu NVDA, Ferramentas, Acesso Remoto, Conectar.
2. Escolha cliente no primeiro botão de opção.
3. Selecione Controlar outra máquina no segundo conjunto de botões de opção.
4. No campo host, digite o host \[nome ou endereço\] do servidor ao qual você está se conectando, por exemplo, nvdaremote.com. Quando o servidor específico usa uma porta alternativa, você pode inserir o host no formato &lt;host&gt;:&lt;porta&gt;, por exemplo nvdaremote.com:1234.
5. Digite um código \[senha ou chave\] no campo código ou pressione o botão gerar código.
A máquina a ser controlada e todos os seus clientes precisam usar o mesmo código.
6. Pressione ok. Depois de concluído, você ouvirá um tom e será conectado.

## Conexões diretas

A opção servidor, no diálogo de conexão, permite configurar uma conexão direta.
Depois de selecionar essa opção, selecione em qual modo o final da conexão estará.
A outra pessoa se conectará a você usando o oposto.

Depois que o modo é selecionado, você pode usar o botão Obter IP externo para obter seu endereço IP externo e
verificar se a porta inserida no campo da porta está encaminhada corretamente.
Se o portcheck \[verificação de porta\] detectar que sua porta (6837 por padrão) não está acessível, um aviso será exibido.
Encaminhe sua porta e tente novamente.
Nota: O processo para encaminhamento de portas está fora do escopo deste documento. Consulte as informações fornecidas com o seu roteador para obter mais instruções.

Digite um código \[senha ou chave\] no campo código ou pressione gerar código. A outra pessoa precisará do seu IP externo junto com o código para se conectar. Se você inseriu uma porta diferente da padrão (6837) no campo porta, verifique se a outra pessoa anexa a porta alternativa ao endereço do host no formato &lt;ip externo&gt;:&lt;porta&gt;.

Ao pressionar OK, você será conectado.
Quando a outra pessoa se conectar, você poderá usar o acesso Remoto do NVDA normalmente.

## Controlando a máquina remota

Depois que a sessão é conectada, o usuário da máquina controladora pode pressionar f11 para começar a controlar a máquina remota (por exemplo, enviando comandos de teclado ou entrada braille).
Quando o NVDA diz como controlar a máquina remota, as teclas do teclado e da linha braille pressionadas irão para a máquina remota. Além disso, quando a máquina controladora estiver usando uma linha braille, as informações da máquina remota serão exibidas nela. Pressione f11 novamente para parar de enviar as teclas e voltar para a máquina controladora.
Para uma melhor compatibilidade, verifique se os esquemas \[leiautes\] de teclado das duas máquinas correspondem.

## Compartilhando sua sessão

Para compartilhar um link para que outra pessoa possa ingressar facilmente na sua sessão de acesso Remoto do NVDA, selecione Copiar link no menu Acesso Remoto.
Se você estiver conectado como o computador de controle, esse link permitirá que outra pessoa se conecte e seja controlada.
Se, em vez disso, você configurou seu computador para ser controlado, o link permitirá que as pessoas com quem você o compartilha controlem sua máquina.
Muitos aplicativos permitem que os usuários ativem esse link automaticamente, mas se ele não for executado a partir de um aplicativo específico, ele poderá ser copiado para a área de transferência e executado no diálogo executar.

## Enviar Control+Alt+Del

Ao enviar teclas, não é possível enviar a combinação Control+Alt+del normalmente.
Se você precisar enviar Control+Alt+Del e o sistema remoto estiver na área de trabalho segura, use esse comando.

## Controlando remotamente um computador autônomo

Às vezes, você pode querer controlar um dos seus computadores remotamente. Isso é especialmente útil se você estiver viajando e desejar controlar o seu PC doméstico a partir do seu laptop. Ou então, você pode controlar um computador em um cômodo da sua casa enquanto está sentado do lado de fora com outro PC. Um pouco de preparação avançada torna isso conveniente e possível. Vejamos:
1. Acesse o menu do NVDA, escolha Ferramentas e, em seguida, Acesso Remoto. Por fim, pressione Enter em Opções.
2. Marque a caixa que diz "Conectar automaticamente ao servidor de controle ao iniciar o NVDA".
3. Selecione se deseja usar um servidor de retransmissão remota ou hospedar localmente a conexão.
4. Selecione Permitir que esta máquina seja controlada no segundo conjunto de botões de opção.
5. Se você hospedar a conexão, precisará garantir que a porta inserida no campo da porta (6837 por padrão) na máquina controlada possa ser acessada pelas máquinas controladoras.
6. Se você deseja usar um servidor de retransmissão, preencha os campos Host e Código, tecle tab até OK e pressione Enter. A opção Gerar código não está disponível nessa situação. É melhor criar um código do qual você se lembre para poder usá-lo facilmente em qualquer local remoto.

Para uso avançado, você também pode configurar o Acesso Remoto do NVDA para conectar-se automaticamente a um servidor de retransmissão local ou remoto no modo de controle. Se desejar, selecione Controlar outra máquina no segundo conjunto de botões de opção.

Nota: A conexão automática nas opções relacionadas à inicialização no diálogo Opções não se aplica até que o NVDA seja reiniciado.

## Silenciando a fala no computador remoto
Se você não deseja ouvir a fala do computador remoto ou sons específicos do NVDA, basta acessar o menu NVDA, Ferramentas e Acesso Remoto. Seta para baixo até Silenciar computador remoto e pressione Enter. Observe que esta opção não desativará a saída braille remota para a tela de controle quando a máquina controladora estiver enviando teclas.

## Terminando uma sessão remota

Para encerrar uma sessão remota, faça o seguinte:
1. No computador de controle, pressione F11 para parar de controlar a máquina remota. Você deve ouvir ou ler a mensagem: "Controlando a máquina local". Se você ouvir ou ler uma mensagem de que está controlando a máquina remota, pressione F11 mais uma vez.
2. Acesse o menu do NVDA, depois Ferramentas, Acesso Remoto e pressione Enter em desconectar.

## Enviar texto da área de transferência

A opção Enviar texto da área de transferência no menu Acesso remoto permite enviar o texto da área de transferência de uma máquina para outra.
quando esta opção estiver ativada, qualquer texto da área de transferência poderá ser enviado da máquina controladora para a máquina controlada e vice-versa.
Isso pode ser feito pressionando o atalho NVDA+Control+Shift+C.

## Configurando o Acesso Remoto do NVDA para funcionar na Área de Trabalho Segura

Para que o Acesso Remoto do NVDA funcione na área de trabalho segura, o complemento deve ser instalado no NVDA em execução na área de trabalho segura.
1. No menu do NVDA, selecione Preferências e Configurações.
2. Na categoria Geral, tecle Tab até o botão Usar configurações salvas atualmente no Logon e outras telas seguras (requer privilégios administrativos) e pressione Enter.
3. Responda Sim às solicitações sobre cópia de suas configurações e sobre a cópia de plug-ins e responda à solicitação de Controle de Conta de Usuário que possa aparecer.
4. Quando as configurações forem copiadas, pressione Enter no botão OK para fechar. Tecle tab até OK e pressione Enter mais uma vez para sair da caixa de diálogo.
Depois que o Acesso Remoto do NVDA estiver instalado na área de trabalho segura, se você estiver sendo controlado em uma sessão remota,
você terá acesso de voz e braille à área de trabalho segura quando alternar.

## Contribuições
Gostaríamos de agradecer aos seguintes colaboradores, entre outros, que ajudaram a tornar o projeto Acesso Remoto do NVDA uma realidade.

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

## Registro de Alterações \[Change Log\]

### Versão 2.3
* Migrado para Python 3
* Suporte ao Python 2 descartado
* Atualização para atender à API alterada no NVDA 2019.3, incluindo:
  - Refatorador de fala
  - Alterações para linhas braille

### Versão 2.2

* Suporte IPv6
* Suporte para o novo NVDA 2018.3 e versões anteriores
* Suporte para comandos \[gestos\] específicos de modelo de linha braille

### Versão 2.1

* Corrigida conexão não é salva ao permitir que esta máquina seja controlada
* Adicionado um script para enviar conteúdo da área de transferência com NVDA+Control+Shift+C
* A entrada Braille agora funciona no modo de navegação
* Suporte a comandos \[gestos\] específicos de modelo de linha braille
* Os bipes gerados pelo Remoto NVDA não bloqueiam mais o NVDA

### Versão 2.0

* Suporte para Braille remoto
* Suporte para links nvdaremote://
* Diálogos centralizados para estar em conformidade com o restante do NVDA
* Corrigido portcheck \[verificação de porta\] para apontar para um domínio que controlamos, portcheck.nvdaremote.com
* Suporte para conectar automaticamente a um servidor de controle no modo mestre \[master \]
* Corrigido erro de renderização na documentação
* Atualiza à versão 2 do protocolo, que inclui um campo de origem em todas as mensagens remotas
* Limpeza de código significativa, permitindo modificações mais fáceis no futuro

## Alterando o Acesso Remoto do NVDA

Você pode clonar este repositório para fazer alterações no NVDA Remote.

### Dependências de terceiros
Podem ser instalados com o pip:
- Markdown
- scons
- python-gettext

### Empacotar o complemento para distribuição:

1. Abra uma linha de comando, mude para a raiz deste repositório
1. Execute o comando **scons**. O complemento criado, se não houver erros, é colocado no diretório atual.
