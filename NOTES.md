* Componentes
- São elementos independentes, substituiveis e modulares que ajudam na escalabilidade manutenção e performance.
EX: um navBar, carrosel

* Ciclo de vida do componente
- São os estagios do componente ngInit, ngOnDestroy etc.
- O Ciclo de vida do componente deve ser bem pre-estabelecido e controlado pois ele pode influencia na performance da aplicação.

* Dica - Use o contrutor para instanciar ou injetar dependencia de serviço a ser utilizado e o ngInit para setar ou chamar metodos ou iniciar um componente

* Data Binding 
- É a forma como associamos a informação que esta no componente para o template e vice-versa.
- String Interpolação: {{ valor }} - associa info do componente para o template.
- Property Binding: [propiedade]="valor" - associa info do componente para a propiedade do template HTML
- Event Binding - (click, onMouseHover, etc)="hanler()" - associa info do template HTML para o componente
- Two-Way Data Binding: [(ngModel)]="propiedade" - associa info entre ambos ou seja mantem ambos atualizados (componente e template HTML)
OBS: Caso queira fazer este metodo utilizando inputs será necessário importar o FormsModule no app.module.ts e inserir ele nos imports.

* Dica - Nos seletores dos componente é possível pasar um arquivo referenciando o componente ou pode ser passado pelo mesmo seletor geralmente isto é usado quando o componente é pequeno. O mesmo vale para o css utilizando css inline.

* Conceito compartilhamento de dados
- @input > propiedades que podem ser passado de uma classe pai para uma classe filho veja a imagem "input.png" nos prints

- @output > retornando dados para a classe pai utilizando eventEmitter veja a imagem "ouput-eventEmitter.png" nos prints

* Componente inteligente / apresentacionais
* Apresentacional - parecido com funcoes puras, se procupa apenas com a interface, nao fica responsavel ou lidar com logica de negocio, nao causa efeito colateral na aplicação, recebem dados via @input e emite eventos via @output.

* Inteligente - parecido com funções impuras, contem toda a logica do negocio, são internamente compostos por componentes apresentacionais, ficam responsaveis por repassar os dados para os componente apresentacionais que por vez apresentaram para o usuario final.

- veja o exemplo na imagem "componentes-tipos.png" nos prints

* Desenvolvimento em modulos com design Modular
- veja definicao na imagem "design-modular.png" nos prints

* Arquiteturas 
* SMACSS - Arquitetura modular para organizar o css 
- veja algumas definições na imagem "arquitetura-smacss.png" nos prints

* BEM(CSS) - Bloco, Elemento Modificador 
- veja a definicao na imagem "arquitetura-bem(css).png" nos prints.

* OOCSS - CSS orientado a objeto, o intuito é a reutilização de código atraves de classes
- veja a imagem "arquitetura-oocss.png" nos prints.

* Instalando o bootstrap
- npm install bootstrap, no seu projeto 
    - verifique no diretorio node_modules se foi criado um diretorio com o nome do bootstrap.

    * Definindo o bootstrap de forma global
    - Vá para o arquivo styles.css ou styles.scss dentro da pasta src do seu projeto
    - Insira o endereço do arquivo 
    - @import '~bootstrap/dist/css/bootstrap.min.css'
    - OU
    - @import '../node_modules/bootstrap/dist/css/bootstrap.min.css'
    - Reinicie o serve
    - Faça um teste inserindo algum elemento do bootstrap




