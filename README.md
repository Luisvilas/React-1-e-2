# Exercício React

* Baixar o arquivo de imagens
* Colocar esse arquivo na pasta public/assets
* Criar pasta components na pasta scr, e criar na pasta components um arquivo MenuComponent.js

Já no visual Code:
* Inserir todo o código nesse arquivo

1. As importações:
   * usestates- gerencia componentes dentro de outros componentes
   * media- exibe listas de imagens e textos juntos
     
2. Define a constante Menu para chamar os pratos:
   * dentro dessa constante ele chama outra constante chamada pratos ou dishes,
     essa que utiliza o import usestate, para utilizar listas de imagens e textos.
   * Dentro dessa mesma constante ele cria a lista de Menu em "dishes.map"
  
3. Na próxima linha de código ele renderiza a linha de código para a página.
  
4. E por último exporta o componente Menu.

-Esse código chama as imagens que estão na pasta public, e coloca na pagina.

-O código imita um cardápio de restaurante com descrições e imagens.

* Apagar tudo do arquivo App.css

No terminal da pasta confusion:
* git init para criar um repositorio
* git add .
* git commit -m "nome do arquivo"
* git remote add origin <url do git hub>
* git push -u origin master
Para subir os arquivos para o github

# Exercício parte 2 - Aula 10

## MenuComponent.js

### 1. Imports utilizados
* Card- componente para inserir um cartão com imagem e conteúdo.
* CardImg- componente que serve para atribuir uma imagem ao Card.
* CardImgOverlay- serve para colocar elementos sobre a imagem do Card.
* CardText- atribuir um texto a essa imagem.
* CardBody- nesse está inserido alguns outros componentes, serve para organizar o cartão.
* CardTitle- utilizado para dar um título ao cartão selecionado.

### 2. Pra que serve o OnDishSelect
* Essa função é chamada quando um prato é selecionado.

### 3. Pra que serve o renderDish
* Para exibir os detalhes do prato selecionado

### 4. Pra que serve props.dishes.map
* Serve para mapear o menu de pratos a serem selecionados
* Para cada prato selecionado ele vincula uma imagem, um texto e um título

## Dishes.js

### 1. Quais são as propriedades
* Essa array possui propriedades como, id, name, image, category, label, price e description.

### 2. Que tipo de date é utilizado
* Ele utiliza o formato de data, apresentando dia, hora, minutos e segundos.

## App.js

### 1. Pra que serve o const[dishes] 
* O dishes é criado para armazenar uma array com os pratos.
* O useState(dishes) ele inicializa a lista de pratos importados do outro arquivo.

### 2. Explicar como funciona o Menu(dishes)
* O componente Menu é renderizado e recebe a propriedade dishes. Sendo dishes a lista dos pratos importados do app.js.
* o menu ele exibe os pratos na interface.
