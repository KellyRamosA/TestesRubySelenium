O que é o appium: O Appium é um framework, open source (de graça), capaz de automatizar testes funcionais para todos os aplicativos,
com essa ferrmanta você escreve/automatiza o teste uma única vez, ou seja, não precisa escrever um cenário para android e outro para o Ios.
Com ela, podemos executar os testes nos aparelhos de forma física ou em reguladores (simuladores de apps) e tablets. O Appium dá suporte a 
diversas linguagens de programação, como Java, php, C#, Python, etc, onde você poderá escolher a que tem mais afinidade.

Vantagens: Como dito a cima, não é necessário que você escreve/automatiza o teste uma única vez, ou seja, não precisa escrever um cenário 
para android e outro para o Ios, como por exemplo teria que com a ferramenta chamada Kotlin e Swift. É possível usar boa parte da lib do
Selenium, Cumcuber, etc.



Como instalar o Appium e suas dependências:

1️- Instalar o Java JDK (Temurin)

Download: https://www.oracle.com/br/java/technologies/downloads/#jdk24-windows

<img width="1720" height="943" alt="image" src="https://github.com/user-attachments/assets/0c7c426e-44fd-4e9e-909a-77064d3af7e1" />

Configurar variáveis de ambiente:

Vá em Painel de Controle > Sistema > Configurações avançadas do sistema > Variáveis de Ambiente.

Clique em Nova em Variáveis de Sistema:

Nome: JAVA_HOME

Valor: C:\Program Files\Eclipse Adoptium\jdk-17.0.x (ou onde estiver instalado)

Edite a variável Path e adicione:

%JAVA_HOME%\bin

Verifique no Prompt se o Java foi instalado corretamente:

java -version: Você verá a versão a qual foi instalda.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

2️- Instalar o Android Studio

Download: https://developer.android.com/studio?hl=pt-br

Instale Android Studio com SDK e AVD.

Abra o Android Studio e configure o SDK (consulte em File > Settings > Android SDK).

Configurar variáveis de ambiente:

ANDROID_HOME: C:\Users\SEU_USUARIO\AppData\Local\Android\Sdk

Adicionar ao Path:

%ANDROID_HOME%\platform-tools
%ANDROID_HOME%\tools
%ANDROID_HOME%\tools\bin

Verifique no Prompt se foi instalado corretamente digitando o seguinte comando(Lembrando que tem que verificar somente após configurar as variáveis de ambiente): 

adb devices

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

3️- Instalar Node.js e npm

Download: https://nodejs.org/en/download 

Irá abrir a tela do prompt pedindo para você apertar qualquer tecla e depois utilizar o powershell para continuar

<img width="1174" height="655" alt="image" src="https://github.com/user-attachments/assets/03563a37-f606-4558-a3a6-f78ae3ad6eb1" />


Verifique no Prompt se foi instalado corretamente digitando os seguintes comandos:

node -v

npm -v

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

4️- Instalar o Appium Doctor

Instalar via npm: Abra o prompt de comando e digite:

npm install -g appium-doctor

<img width="1120" height="630" alt="image" src="https://github.com/user-attachments/assets/c8853d34-578b-4664-b156-29c279fee1aa" />


Verifique no Prompt se foi instalado corretamente digitando o seguinte comando:

appium-doctor --android

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

ATENÇÃO: Caso ao instalar qualquer coisa via npm e receber um alerta de que tem uma versão superior a que está usando e pedir para atualizar, basta rodar o comando abaixo:

npm install -g npm@11.4.2    (claro que irá colocar a versão atual referente a data que está configurando sua máquina)

<img width="1134" height="624" alt="image" src="https://github.com/user-attachments/assets/e53df801-d990-4e2a-b5b2-c4d9d574f64f" />


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

5️- Instalar o Ruby

Download: RubyInstaller + Ruby+Devkit.

Abra o prompt de comando e digite/rode o seguinte comando, escolhendo após a opção 3: ridk install

<img width="1120" height="624" alt="image" src="https://github.com/user-attachments/assets/20646c4c-0913-44aa-b230-931e255043d0" />


Verifique no Prompt se foi instalado corretamente digitando os seguintes comandos:

ruby -v

gem -v

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

6️- Instalar o Appium

Instalação via npm, digite/rode no prompt:

npm install -g appium

Verifique no Prompt se foi instalado corretamente digitando o seguinte comando: 

appium -v


Rodar o Appium:

appium



