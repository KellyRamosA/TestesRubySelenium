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

Download: Baixar Android Studio

Instale Android Studio com SDK e AVD.

Abra o Android Studio e configure o SDK (consulte em File > Settings > Android SDK).

Configurar variáveis de ambiente:

ANDROID_HOME: C:\Users\SEU_USUARIO\AppData\Local\Android\Sdk

Adicionar ao Path:

%ANDROID_HOME%\platform-tools
%ANDROID_HOME%\tools
%ANDROID_HOME%\tools\bin

Verifique no Prompt se foi instalado corretamente digitando o seguinte comando: adb devices
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

3️- Instalar Node.js e npm

Download: Baixar Node.js

Passos:

Baixe a versão LTS.

Instale normalmente.

Verifique no Prompt se foi instalado corretamente digitando os seguintes comandos:

node -v
npm -v

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

4️- Instalar o Appium Doctor

Instalar via npm:

npm install -g appium-doctor

Verifique no Prompt se foi instalado corretamente digitando o seguinte comando: appium-doctor --android

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

5️- Instalar o Ruby

Download: Baixar RubyInstaller

Passos:

Baixe o Ruby+Devkit.

Execute o instalador.

Rode ridk install e escolha a opção 3.

Verifique no Prompt se foi instalado corretamente digitando os seguintes comandos:

ruby -v
gem -v
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

6️- Instalar o Appium

Instalação via npm:

npm install -g appium

Verifique no Prompt se foi instalado corretamente digitando o seguinte comando: appium -v


Rodar o Appium:

appium



