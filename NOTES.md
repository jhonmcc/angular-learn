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



