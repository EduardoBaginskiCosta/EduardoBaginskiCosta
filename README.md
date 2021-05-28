# Quem Sou Eu:

Olá ! Sou Eduardo Baginski Costa, sou um desenvolvedor web, e Desktop brasileiro.  
  
Eu desenvolvo bibliotecas JavaScript, PHP e CSharp, para desenvolvedores, que desejam tornar seu websites e aplicativos mais seguros. Como a ***encriptação*** e ***decriptação*** de dados, ***proteção de mídia digital (imagens, vídeos, documentos)***, entre outros.  
Já criei diversas bibliotecas (Web e Desktop), voltadas para o segurança, e para a dinâmica dos mesmos. Nos próximos tópicos, será mostrado todas as bibliotecas desenvolvidas até o presente momento, tanto as de desenvolvimento web, como as para desenvolvimento Desktop.

[comment]: --------------------------------------------------------------------------

# Sobre a Sway Cloud SDK:

A ***Sway Cloud SDK*** é um conjunto de bibliotecas, tanto para o desenvolvimento web, quanto para o desenvolvimento Desktop, que ajudam aos desenvolvedores tornarem seus websites, e softwares mais seguros e dinâmicos para os usuários/clientes.  
O SDK é regido por um plano mensal de ***50 reais***, ao qual o usuário tem acesso a todas as bibliotecas (Web e Desktop), incluindo as futuras bibliotecas, que serão adicionadas. Ao criar uma conta o usuário recebe uma ***SDK-KEY*** única, ao qual se mantem válida enquanto a conta estiver ativa.  
A ***SDK-KEY*** serve para ativar os recursos disponíveis nas bibliotecas (Web e Desktop); Sem a mesma, nenhum recurso presente nas bibliotecas estará disponível para a utilização do usuário.  

[comment]: --------------------------------------------------------------------------

# Como Abrir Uma Conta Oficial:

Para poder ter acesso a ***Sway Cloud SDK***, e a todas as bibliotecas (Web e Desktop), basta entar em ***[contato comigo](mailto:eduardobcosta1234@gmail.com)*** pelo ***Google GMail***. Lhe será dito todas as informações, como: ***pagamento***, ***incrementação (Web e Desktop)***, ***obrigações e deveres***, ***ativação***, etc.  
**!!! AVISO IMPORTANTE !!!:** Somente aceite pagamentos, e informações disponibilizadas pelo meu GMail oficial: ***eduardobcosta1234@gmail.com***.

[comment]: --------------------------------------------------------------------------

# Bibliotecas Web (JavaScript e PHP):  
Essas bibliotecas são destinadas e deixar os websites mais seguros e dinâmicos, geralmente sendo escritas em JavaScript e PHP, por serem justamente as línguagens mais comuns, tanto para iniciantes, quanto para profissionais, integrando ferramentas de fácil utilização, sendo elas:  

* Encriptação e Decriptação [PHP].  
  * Esta biblioteca realiza a ***encriptação*** e ***decriptação*** de variáveis PHP, utilizando uma ***Senha-Mestra***, definida pelo desenvolvedor.
  * Encriptação e Decriptação rápidas, fáceis, dinâmicas e seguras.

* Proteção de Midia Digital [JavaScript].  
  * Esta biblioteca protege seus arquivos de serem baixados, e incorporados em outros websites.
  * Pode proteger arquivos de ***Vídeo*** e ***Áudio***, de qualquer dimensão.

* Rastreador Web (Web Crawler) [PHP].
  * Esta biblioteca permite você capturar dados, atributos, elementos, meta tags, códigos-dontes de websites, etc.  
  * Biblioteca ideal para construir ***motores de busca***.

* Bibliotecas Hospedadas [PHP e JavaScript].
  * Hospedamos todos os tipos de bibliotecas, que podem ser incluídas rápidamente, tais como: ***jQuery***, ***D3.js***, ***jQuery Mobile***, ***Ext Core***, dentre outras.  
  * Nos oferescemos também um plano mensal de hospedagem, para você hospedar suas bibliotecas, e incluí-las quando desejar.

* DOM Inspector [JavaScript].  
  * Esta biblioteca disponibiliza a "criação" de um ***"DOM Inspector"***, que pode alterar attributos, estilos e o código-fonte do elemento selecionado.

[comment]: --------------------------------------------------------------------------

# Bibliotecas CSharp (C#):  
Essas bibliotecas são destinadas a segurança de dados, e a integração de recursos extras ao ***WinForms***, tais como:   

* ### Leitor de Arquivos INI:  
  * Esta classe permite que o software consiga interpretar arquivos INI, com facilidade, podendo retornar valores, em diferentes tipos, de acordo com a necessidade, e o tipo de chave que está sendo trabalhado, sendo eles: ***string***, ***int***, ***boolean (bool)***, ***double***, e também em uma ***array*** tipo ***string***. Veja uma exemplo de utilização:  
  
  ```csharp
  IniFile INIDoc = new IniFile("IniFile.ini");  // --- Aqui Carregamos o Conteúdo do Arquivo INI  
    
  string UserName = INIDoc.GetValue("UserData", "Name", ""); // --- Aqui requisitamos que seja retornado o valor da chave "Name"  
  int UserAge = INIDoc.GetInteger("UserData", "Age", 0); // --- Aqui requisitamos que seja retornado a o valor da chave "Age", no formato "Int"  
  bool ApplyConfig = INIDoc.GetBoolean("UserData", "Apply", false); // --- Aqui requisitamos que seja retonado o valor da chave "Apply", no formato "bool"  
  double UserHeight = INIDoc.GetDouble("UserData", "Height", 0); // --- Aqui requisitamos que seja retornado o valor da chave "Height", no formato "double"  
  string[] UserParents = INIDoc.GetAllValues("Parents", "Name", ""); // --- Aqui requisitamos que sejam passado o valor de todas as chaves "Name", que estão dentro da seção "Parents"
  ```  
  
  * Possui suporte a múltiplas leituras de chaves em uma mesma seção, sendo retornados em uma ***array*** tipo ***string***.

* ### TabControl Sem As Bordas Laterais:  
  * Este controle como o nome diz, é um ***TabControl*** normal, porém suas bordas padrões foram removidas, aumentando o ***ClientRectangle***, proporcionando mais espaço.

* ### Extensão Para o Controle RichTextBox:  
  * Adicionar a Função: ***"SetInnerMargins"***. Ao qual é utilizada para setar as margens internas do controle. Veja um exemplo de utilização:  
  
  ```csharp
  RichTextBox MyRichTextBox = new RichTextBox(); // --- Aqui capturamos o RichTextBox que desejamos aplicar, as margens internas  
    
  // !!! --- ATENÇÃO: as variáveis (LEFT, TOP, RIGHT e BOTTOM), devem ser valores inteiros (int) --- !!!  
  MyRichTextBox.SetInnerMargins(20, 20, 20, 20); // --- Aqui setamos a dimensão das bordas internas: LEFT, TOP, RIGHT e BOTTOM
  ```  
  
  * Podendo ser utilizado juntamente a um **TextRuler**.  

* ### Cifra de String (Segurança):
  * Esta classe realiza a ***encriptação*** e ***decriptação*** de ***"strings"***, utilizando uma ***"Chave-Mestra"***. Veja um exemplo de utilização:  
  
  ```csharp
  private static readonly string MASTER_KEY = "master_key_here"; // --- Aqui definimos a Chave-Mestra que será utilizada
  ```  
  
  ```csharp
  string UserPass = MyTextBox.Text; // --- Aqui capturamos o contéudo do TextBox
    
  string EncryptedString = StringCipher.Encrypt(MASTER_KEY, UserPass); // --- Aqui será retornado a senha já encriptada  
  string Decryptedstring = StringCipher.Decrypt(MASTER_KEY, EncryptedString); // --- Aqui será retornado a senha decriptada
  ```  
  
  * Sendo uma classe perfeita para ocultar e proteger dados, dos usuários.
  
* ### Interface de usuário:
  * Esta classe adiciona ferramentas para manipular ***Formulários (Form)***, apartir de outros controles, sendo recomandada na utilização de ***Formulários (Form)*** que não possuem bordas. As ferramentas disponíveis para a utilização, são:
    * A função: ***DraggableWindow***, esta função permite que você consiga mover o ***Formulário (Form)*** apartir de outro controle interno. Veja um exemplo de utilização:  
	
	```csharp
	Button DragControl = MyButton as Button; // --- Aqui capturamos o controle que será responsável, pela movimentação do Formulário (Form) (OBS: pode ser qualquer controle)  
	new UserInterface().DraggableWindow(DragControl, this); // --- Aqui definimos que o controle será responsável por mover o Formulário (Form), sendo "this" o Formulário local
	```  
	
	* A função ***MaximizationControl***, serve para que você possa maximizar/normalizar um ***Formulário (Form)***, apartir de um controle interno. Esta possui alguns argumentos extras como: ***doubleClick*** ao qual define se o controle deve ser ativado com um clique duplo, para maximizar/normalizar um ***Formulário (Form)***, e o  ***moveToCenter*** ao qual define se o ***Formulário (Form)*** ao ser normalizado, deve ser "movido" para o centro da janela. Veja um exemplo de utilização:  
	
	```csharp
	Button MaxControl = MyButton as Button; // --- Aqui capturamos o controle que será responsável, pela maximização/normalização do Formulário (Form) (OBS: pode ser qualquer controle)  
	new UserInterface().MaximizationControl(MaxControl, this, false, false); // --- Aqui definimos que o controle será responsável por maximizar/normalizar o Formulário (Form)
	```  
	
	* A função ***MinimizeControl***, server para que você possa minimizar um ***Formulário (Form)***, apartir de um controle interno. Este possui o argumento ***doubleClick***, ao qual define se o controle deve ser ativada com um clique duplo. Veja um exemplo de utilização:  
	
	```csharp
	Button MinControl = MyButton as Button;// --- Aqui capturamos o controle que será responsável, pela minimização da Formulário (Form) (OBS: pode ser qualquer controle)  
	new UserInterface().MinimizeControl(MinControl, this, false); // --- Aqui definimos que o controle será responsável por minimizar o Formulário (Form)
	```  
	
	* A função ***CloseControl*** (1º Variante), serve para que você possa fechar o ***Formulário (Form)***, apartir de um controle interno. Esta possui alguns argumentos extras como: ***doubleClick*** que define se o controle deve ser ativo com um clique duplo, e o ***confirmBox*** que define o ***Formulário (Form)*** que deve ser mostrado como um diálogo ***"ShowDialog()"***, antes da execução da função, ao qual deve possuir dois retornos de diálogo (***DialogResult.Yes***, e ***DialogResult.No***). Veja um exemplo de utilização:  
	
	```csharp
	MyFormDialog ConfFialog = new MyFormDialog(); // --- Aqui invocamos um Formulário (Form), que possua os retornos de diálogo ("DialogResult.Yes" e "DialogResult.No")  
	Button CloseButton = MyButton as Button; // --- Aqui capturamos o controle que será responsável, pelo fechamento do Formulário (Form) (OBS: pode ser qualquer controle)  
	new UserInterface().CloseControl(CloseButton, this, false, ConfFialog); // --- Aqui definimos que o controle será responsável por "fechar" o Formulário (Form), e a "caixa de diálogo", que deve ser mostrada
	```  
	
	* A função ***CloseControl*** (2º Variante), serve para que você possa fechar o ***Formulário (Form)***, apartir de um controle interno. Esta possui o argumento ***doubleClick***, ao qual define so o controle deve ser ativado com um clique duplo.  
	Seu funcionamento é igual a "1º Variante", porém não possue o argumento ***confirmBox***, sendo assim, o fechamento do ***Formulário (Form)*** será instantâneo. Veja um exemplo de utilização:  
	
	```csharp
	Button CloseButton = MyButton as Button; // --- Aqui capturamos o controle que será responsável, pelo fechamento do Formulário (Form) (OBS: pode ser qualquer controle)  
	new UserInterface().CloseControl(CloseButton, this, false); // --- Aqui definimos que o controle será responsável por "fechar" o Formulário (Form)
	```  
	
	* A função ***SetTip***, como o nome diz, define o ***ToolTip*** que será exibido ao passar o mouse sobre um controle, sendo um atalho mais prático para setar um ***ToolTip***. Veja um exemplo de utilização:  
	
	```csharp
	Button TipButton = MyButton as Button; // --- Aqui capturamos o controle que desejamos atribuir o "ToolTip" (OBS: pode ser qualquer controle)  
	new UserInterface().SetTip(TipButton, "Testando o ToolTip"); // --- Aqui aplicamos o ToolTip ao controle definido
	```  
	
* ### Retângulo do Usuário (Graphics):
  * Esta classe adiciona criar um ***UserRect***, que pode ser utilizado um ***PictureBox*** (caso seja utilizado como um "Canvas", para desenhar gráficos), para auxiliar o usuário a posicionar e redimensionar alguma imagem e/ou desenho. Veja um exemplo de utilização:  
  
  ```csharp
  Rectangle Area = new Rectangle(5, 5, 20, 20); // --- Aqui definimos a posição ("X: 5" e "Y: 5"), e a dimensão ("Width: 20" e "Height: 20") inicial do "UserRect"  
    
  UserRect URect = new UserRect(Area); // --- Aqui invocamos a classe "UserRect"  
  PictureBox Target = MyPictureBox as PictureBox; // --- Aqui capturamos o "PictureBox", que será o nosso alvo  
  URect.SetPictureBox(Target); // --- Aqui definimos em qual "PictureBox" ele deve ser injetado
  ```  

[comment]: --------------------------------------------------------------------------

# Bibliotecas Encomendadas (Web e Desktop):

Você pode entrar em contato pelo GMail oficial ***eduardobcosta1234@gmail.com***, e encomendar uma biblioteca com funções e classes customizadas, de acordo com a sua necessidade.  
Após o envio, seu pedido será analisado, e respondido dentro do período de ***uma semana***. Se a mesma for aceita, o preço será definido de acordo com a dificuldade, e complexidade da mesma. Se for recusada, lhe será enviado um e-mail, notificando tal ocorrência.  
  
Para a sua segurança, não aceite informações de terceiros de qualquer tipo que seja. Somente utilize, e siga instruções e informações do GMail oficial ***eduardobcosta1234@gmail.com***.

[comment]: --------------------------------------------------------------------------

# Considerações Finais e Informações Extras:

* ### Considerações Finais:
  * Os códigos exibidos são exemplos/demonstrações básicas de algumas bibliotecas, não se referindo ao produto como um todo.
  * As bibliotecas (Desktop) funcionam com o **NET Framework 4.5.1** ou superior.
  * Algumas bibliotecas (Desktop) podem depender de ***DLL's*** externas, em caso de recursos não instalados no computador.
  * Todas as bibliotecas (Dektop) funcionam em computadores (***32 e 64 Bits***), sendo o sistema operacional ***Windows 7 (indefinido)***, ou superior.
  * As bibliotecas (Web), requesitam navegadores com suporte a tecnologia ***HTML 5***, ***CSS 3*** e ***PHP (ultimas versões)***.

* ### Informações Extras:
  * Todas as informações sobre: ***pagamento***, ***incrementação***, ***ativação***, etc. Só devem ser seguidas, se vindas do GMail oficial ***eduardobcosta1234@gmail.com***.
  * Não aceite instruções externas/terceiros, com exceção de tutoriais, desde que estes não contenham ações relacionadas a: ***ativação***, ***pagamento***, ou até mesmo a ***manutenção*** e/ou ***configuração*** da conta.
  * Toda e qualquer dúvida deve ser enviada ao GMail oficial ***eduardobcosta1234@gmail.com***, ao qual lhe será devolvida uma resposta e/ou a indexação de um ***vídeo confiável*** e verificado.

[comment]: --------------------------------------------------------------------------
  
# Créditos e Direitos Autorais:

* Copyright © 2021 - Eduardo Baginski Costa. Todos os Direitos Reservados.  
* Todas as bibliotecas estão protegidas por ***Direitos Autorais***, assim como seus ícones, e seu código-fonte. Todos os Direitos Reservados a *Eduardo Baginski Costa*.  
* Os nomes ***Sway Cloud SDK***, ***Sway Cloud***, ***Sway Cloud Developers*** e variantes, assim como seus ícones, e código-fonte estão protegidos por ***Direitos Autorais***. Todos os Direitos Reservados a *Eduardo Baginski Costa*.

















