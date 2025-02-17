# Processo Seletivo

Este é um projeto Java que utiliza Servlets e Maven para implementar um sistema de processo seletivo.

## Requisitos

- [Visual Studio Code](https://code.visualstudio.com/Download) (Editor de código)
- [XAMPP](https://www.apachefriends.org/pt_br/index.html) (Servidor local Apache + MySQL)
- [Java SE Development Kit](https://www.oracle.com/java/technologies/downloads/) (JDK 23 ou superior)
- [Apache Maven](https://maven.apache.org/download.cgi) (Gerenciador de dependências)

## Passos para Instalação

### 1. Instalar o Java JDK

Baixe e instale o JDK 23 ou superior a partir do link oficial da Oracle.

- Após a instalação, adicione o `JAVA_HOME` nas variáveis de ambiente:
  - **Variável**: `JAVA_HOME`
  - **Valor**: Caminho onde o JDK foi instalado, por exemplo: `C:\Program Files\Java\jdk-23`

### 2. Instalar o Maven

Baixe o Maven a partir do link oficial e descompacte o arquivo em um diretório de sua escolha, por exemplo:

- **Caminho de instalação**: `C:\apache-maven-3.x.x`

Adicione o Maven ao seu `PATH`:
- **Variável**: `MAVEN_HOME`
- **Valor**: Caminho onde o Maven foi instalado, por exemplo: `C:\apache-maven-3.x.x`

E adicione o diretório `bin` do Maven ao seu `PATH`:
- **Valor**: `C:\apache-maven-3.x.x\bin`

### 3. Baixar o Projeto

Clone o repositório do projeto para o seu diretório de trabalho local:

```bash
git clone https://github.com/pedroleandro/processoseletivo.git
```

## Passos para Execução

### 1. Construir o projeto

Navegue até o diretório do projeto:

```bash
cd processoseletivo
```

Em seguida, execute o Maven para compilar o projeto e gerar o arquivo .war:

```bash
mvn clean package
```

### 2. Colocar o WAR no Tomcat

Copie o arquivo .war gerado na pasta target e cole na pasta webapps do Tomcat em `C:\xampp\tomcat\webapps`

### 3. Inicie o Tomcat no painel de controle do xampp

### 4. Acessar a aplicação em:
```bash
http://localhost:8080/processoseletivo
```

ou 

```bash
http://localhost:8080/processoseletivo/hello
```

### Estrutura Base do Projeto

```bash
processoseletivo/
 ├── src/
 │    ├── main/
 │    │    └── java/
 │    │         └── br/
 │    │              └── com/
 │    │                   └── processoseletivo/
 │    │                        └── servlets/
 │    │                             └── HelloWorldServlet.java
 │    ├── WEB-INF/
 │    │    └── web.xml
 │    └── index.html
 └── pom.xml
```
