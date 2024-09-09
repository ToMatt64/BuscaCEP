
# Busca CEP

## Descrição

Este projeto Java é uma aplicação desktop que realiza buscas de endereços a partir de um CEP informado. Utiliza uma API para consulta de CEP (através de uma requisição em formato XML) e exibe as informações do endereço, como logradouro, bairro, cidade e estado.

## Funcionalidades
- Busca de endereço a partir do CEP.

- Preenchimento automático dos campos: Endereço, Bairro, Cidade e UF.

- Indicação de sucesso ou erro na busca do CEP.

- Limpeza dos campos com um clique no botão "Limpar".

- Suporte para acionamento da busca através do botão "Buscar" ou pressionando a tecla Enter no campo de CEP.

- Validação do campo CEP para aceitar apenas números (máximo de 8 dígitos).

- Informações adicionais sobre o sistema através do botão "Sobre".

## Requisitos do Sistema

- Java SE 8 ou superior
- IDE compatível com projetos Java (Ex: Eclipse, IntelliJ IDEA) ou terminal com suporte a compilação e execução de programas Java.
### Biblioteca externa:
- Atxy2k CustomTextField para validação de campos: https://github.com/atxy2k/CustomTextField
- Dom4j para manipulação de XML: https://dom4j.github.io

## Instalação e Configuração

Clonar o repositório ou baixar os arquivos do projeto:

Se o projeto estiver em um repositório remoto, utilize:
- bash
- Copiar código
- git clone <URL_DO_REPOSITORIO>

Ou simplesmente baixe o código-fonte manualmente.

## Abrir o projeto em uma IDE:

Importar o projeto para sua IDE preferida (Eclipse, IntelliJ, NetBeans).
Certifique-se de que o JDK está corretamente configurado.

### Instalar as dependências:

- Baixe a biblioteca Atxy2k CustomTextField e adicione-a ao classpath ou como dependência do projeto.
- Baixe a biblioteca Dom4j e adicione-a ao classpath ou como dependência.

**Passos para adicionar dependências no Eclipse:**

- Clique com o botão direito no projeto.
- Selecione Build Path > Configure Build Path.
- Vá até a aba Libraries e clique em Add External JARs....
- Selecione o JAR da biblioteca Atxy2k CustomTextField e Dom4j e adicione ao projeto.

**Compilar e executar o programa:**

Na sua IDE, encontre a classe Cep que contém o método main.

Execute o programa pressionando Run.

Executar via terminal:

Navegue até a pasta onde o arquivo .java está localizado.
Compile o arquivo com o comando:
bash
Copiar código
javac -cp ".;path/to/libs/*" cep/Cep.java
(Substitua path/to/libs/* pelo caminho das bibliotecas necessárias.)
Execute o programa com o comando:
bash
Copiar código
java -cp ".;path/to/libs/*" cep.Cep
## Como Usar
### Inserir o CEP:

Na interface do programa, insira um CEP válido (somente números) no campo indicado.
O campo aceita até 8 dígitos.
### Buscar endereço:

- Pressione o botão Buscar ou simplesmente aperte Enter após digitar o CEP.
- Se o CEP for válido, os campos de Endereço, Bairro, Cidade e UF serão automaticamente preenchidos.
- Se o CEP não for encontrado, uma mensagem de erro será exibida.
### Limpar os campos:

Caso deseje limpar todos os campos, clique no botão Limpar.
## Informações sobre o programa:

- Clique no ícone de "Sobre" (um botão com ícone de informação) para visualizar informações adicionais do sistema.
## Tratamento de Erros

- Caso o campo de CEP esteja vazio e a busca seja realizada, uma mensagem de erro será exibida solicitando a inserção do CEP.
- Se o CEP inserido for inválido ou não encontrado na base de dados da API, uma notificação informando "CEP não encontrado" será mostrada.
- Conexões falhas à API ou problemas de rede também serão capturados e exibidos no console da aplicação.
## Modificações Futuras
- Implementar um histórico de consultas de CEP.
- Adicionar suporte para endereços com CEPs especiais ou fora da base da API usada.
- Melhorar a interface gráfica para uma experiência de usuário mais intuitiva.
## Considerações Finais
Este projeto é um exemplo simples de como integrar uma aplicação Java com APIs externas e manipular XML, além de demonstrar o uso de bibliotecas externas para validação de campos de texto. Sinta-se à vontade para modificar e melhorar conforme sua necessidade.

## Autor
Desenvolvido por Matheus Carvalho.
