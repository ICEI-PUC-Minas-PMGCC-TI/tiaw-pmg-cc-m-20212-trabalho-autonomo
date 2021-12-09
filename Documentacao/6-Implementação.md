# Projeto da Solução

## Tecnologias Utilizadas
As tecnologias utilizadas para implementação do projeto foram:
  * Front-End: Arquivos HTML, CSS e JavaScript que em conjunto formam a página WEB.
    * Para o desenvolvimento da página HTML foi utilizado o framework "bootstrap" que permite maior facilidade no desenvolvimento da responsividade.
    * A biblioteca "Font-Awesome" foi utilizada para incluir todos os ícones da aplicação de forma integrada
    * Os ambientes de desenvolvimento escolhidos foram o "Visual Studio Code" e a ferramenta "replit" de acordo com a preferência do desenvolvedor.
    * Os artefatos específicos foram publicados na WEB por meio das  plataformas do "Github Pages" e "replit".
    
      > A plataforma do GitHub pages foi escolhida para hospedagem da aplicação final por possuir integração direta com o repositório utilizado ao longo do desenvolvimento  
      
  * API'S: Foram utilizadas duas API's no desenvolvimento da funcionalidade do mapa na aplicação
    * Google Maps Api: API do google maps que permite interagir com o mapa diretamente da página WEB
    * Places API: Extensão do API do google maps que permite a sugestão e sugestão de lugares de acordo com o endereço fornecido pelo usuário
 

## Arquitetura da solução

# Funcionalidades da Aplicação
  Nesta sessão encontra-se a descrição das funcionalidades presentes na aplicação 
  
  * As funcionalidades apresentam-se com imagens de suas respectivas telas, estruturas de dados, desenvolvedor responsável e link disponível na WEB

## Mapa Integrado
A funcionalidade de Mapa permite que o usuário busque o endereço desejado
  * Ao digitar o endereço uma sugestão surge como lista embaixo da barra de busca 
  * API's Utilizadas: Google maps API e Places API
  
Desenvolvedor responsável: Ricardo Henrique Guedes Furiati

  > Documentação disponível em: https://developers.google.com/maps/documentation <br>
  > Funcionalidade disponível em: https://rickfuriati.github.io/Collegare/index.html <br>


<img src="https://github.com/ICEI-PUC-Minas-PMGCC-TI/tiaw-pmg-cc-m-20212-trabalho-autonomo/blob/015e27c3d7d2dc35a116b15d88d11972d43658b9/Documentacao/images/Funcionalidades/Mapa.png" width="400">

## Cadastro de Serviços

Página do cadastro do site com dois botões, um para salvar o novo cadastro do
localstorage e outro para mostrar todos os cadastros já salvos no local storage. O botão de
salvar já mostra automaticamente o que estava no localstorage sem a necessidade de
apertar o botão de mostrar, além de uma função para mostrar que os espaços não podem
ficar em branco sinalizando em vermelho as caixas de texto.

Desenvolvedor Responsável: Victor Lopes Azevedo Araujo

> Funcionalidade disponível em: https://vlopinhos.github.io/Cadastro-Collegare/

<img src="https://github.com/ICEI-PUC-Minas-PMGCC-TI/tiaw-pmg-cc-m-20212-trabalho-autonomo/blob/aba9d75c159752e1cc4169613ba271a92c80b0ec/Documentacao/images/Funcionalidades/Cadastro.png" width="400">

### Estrutura de Dados:
``` javascript
function incluirCadastro() {
 
 let objDados = leDados();
 
 let strNome = document.getElementById("inputNome").value;
 let strEmpresa = document.getElementById("inputEmpresa").value;
 let strCategoria = document.getElementById("inputCategoria").value;
 let strEndereco = document.getElementById("inputEndereco").value;
 let strTelefone = document.getElementById("inputTelefone").value;
 let strEmail = document.getElementById("inputEmail").value;
 let strDescricao = document.getElementById("inputDescricao").value;
 
 let novoCadastro = {
 
   nome: strNome,
   empresa: strEmpresa,
   categoria: strCategoria,
   endereco: strEndereco,
   telefone: strTelefone,
   email: strEmail,
   descricao: strDescricao
 };
 
 objDados.cadastros.push(novoCadastro);
 
 salvaDados(objDados);
 
 imprimeDados();
 
}

```




