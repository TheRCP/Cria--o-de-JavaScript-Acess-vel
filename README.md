## Antevisão da criação de JavaScript acessível

### O que é JavaScript?

Talvez seja melhor, para responder a esta questão, começar por responder o que **NÃO** é JavaScript.

Primeiro, não é [HTML](#). O JavaScript não usa as *tags* do [HTML](#) nem se rege por nenhuma das regras gerais da linguagem [HTML](#). Pode, contudo, usar JavaScript com [HTML](#) numa página Web.

Segundo, o JavaScript não é Java. Embora o JavaScript seja muitas vezes chamado de Java, os dois não são a mesma coisa. O Java foi desenvolvido pela Sun Microsystems e é uma linguagem de programação autónoma. O JavaScript, por seu turno, foi desenvolvido pela Netscape Corporation. Embora seja similar ao Java em termos de sintaxe, o JavaScript não é uma linguagem autónoma; o JavaScript para funcionar precisa de ser parte integrante de uma página Web, a qual terá que ser vista num navegador Web que interprete a linguagem JavaScript.

A linguagem de programação Java da Sun pode ser implementada em páginas Web e funcionar, por si só, como programa, ao passo que os *scripts* feitos em JavaScript são dependentes do computador cliente (dos seus visitantes) para poderem funcionar.

Uma vez mais, JavaScript não é [HTML](#) ou uma versão de [HTML](#). É uma linguagem de programação à parte, completamente distinta. A linguagem [HTML](#) é lida e processada pelo navegador Web. Quando o navegador lê código JavaScript dentro dos seus documentos [HTML](#), ele processa o código, e depois mostra o resultado na página Web. Para ler JavaScript o computador tem de ter um interpretador de JavaScript, um programa que interpreta o código e o executa, e esse interpretador tem de estar ativo.

O [HTML](#), por si só, cria páginas bastante estáticas. Existe pouca interacção com o utilizador e pouca dinâmica de conteúdos dentro de uma página em particular. O [HTML](#) não consegue pensar; ele não tem a capacidade de efetuar cálculos matemáticos, de armazenar variáveis, ou de mostrar dinamicamente conteúdo. O JavaScript permite que a página Web 'pense'. Embora muitas linguagens de programação existentes do lado do servidor (tais como PHP, JPS, ASP, ou ColdFusion) tenham essa capacidade de executar todas essas funções, o JavaScript consegue executar estas funções dentro do navegador do cliente. Uma vez que o JavaScript é uma linguagem de programação, ela permite aos programadores implementar pequenas aplicações nas suas páginas. Estes programas podem fazer coisas tão simples como alterar um gráfico quando o rato é colocado sobre ele, ou coisas complexas como executar fórmulas matemáticas sofisticadas de acordo com os dados introduzidos pelo utilizador.

---

### Questões de acessibilidade do JavaScript

O JavaScript permite aos desenvolvedores adicionar interacção acrescida, processamento de informação, e controlo do conteúdo de base Web. Todavia, o JavaScript também pode levantar questões de acessibilidade. Estas questões incluem:

- **Navegação:** Inaptidão ou dificuldade de navegação ao usar um teclado ou uma tecnologia de apoio.
- **Esconder conteúdo:** Apreresentação de conteúdo ou funcionalidade não acessível às tecnologias de apoio.
- **Controlo pelo Utilizador:** Falta de controlo do utilizador perante as alterações automáticas do conteúdo.
- **Confusão/Desorientação:** Alterando ou modificando as funcionalidades normais do agente de utilizador (navegador) ou modificando as formas de accionar eventos por formas não familiares ao utilizador.

Tipicamente uma página Web que contenha JavaScript será totalmente acessível se a funcionalidade expressa pelo *script* for dispositivo-independente (que não requeira apenas o rato ou apenas o teclado) e a informação (conteúdo) esteja disponível às tecnologias de apoio. Infelizmente, não existem soluções fáceis que possam ser aplicadas para resolver todos os problemas de acessibilidade associados ao JavaScript. A única forma de assegurar a acessibilidade do JavaScript é através da avaliação de cada componente individual do *script* e desenvolver uma solução única para o problema de acessibilidade que ele coloca. Quem desenvolve precisa estar familiarizado com as questões que envolvem a acessibilidade do JavaScript e aplicar técnicas que façam uma ou ambas as coisas que se seguem acontecer:

1. Assegurar que as aplicações desenvolvidas em JavaScript são directamente acessíveis;
2. Fornecer uma alternativa, não-JavaScript, acessível.

---

### JavaScript não tem impacto na acessibilidade

Só porque é utilizado JavaScript numa página, isso não significa que a página é inacessível. Em muitos casos, o JavaScript pode ser usado para aumentar a acessibilidade. Informação adicional, avisos, ou instruções podem ser dadas aos utilizadores através de mensagens feitas em JavaScript. Por exemplo, as directrizes de acessibilidade em vigor nos Estados Unidos (Secção 508), determinam que um utilizador deve ser sempre notificado quando lhe é dado um determinado tempo para responder a uma solicitação e que, inclusivamente, lhe deve ser atribuído mais tempo para o fazer. Este tipo de funcionalidade será difícil de conseguir apenas com [HTML](#).

O JavaScript é, muitas vezes, utilizado para criar elementos de interfaces visuais que não afectam a acessibilidade. O JavaScript é comummente utilizado para fazer rolar imagens, em que uma imagem é substituída por outra sempre que se posiciona o rato em cima; por exemplo, quando um item do menu de navegação se altera para mostrar uma sombra, um recorte, ou ficar com uma impressão mais forte sempre que o rato é colocado sobre ele.

Coloque o rato sobre a imagem que se segue para ver um exemplo de JavaScript que não tem impacto sobre a acessibilidade.

[![Home](https://www.acessibilidade.gov.pt/wp-content/uploads/2020/03/off.gif)](https://www.acessibilidade.gov.pt/wp-content/uploads/2020/03/on.gif)

#### Problemas?

Nenhum. Neste exemplo, o JavaScript não introduz um conteúdo ou funcionalidade verdadeiramente importante. A troca de imagens é meramente cosmética.

#### Solução

Não são necessárias técnicas de acessibilidade adicionais. Não se esqueça, a imagem, ela própria, tem de ter um texto alternativo (i.e., `<img alt="home"... />`). Também pode desenvolver algo mais interessante. Veja [rolar imagens sem utilizar JavaScript - link](http://www.alistapart.com/stories/rollovers/).

Esta utilização de JavaScript não necessita de cuidados de acessibilidade porque o *script* não mostra conteúdo ou introduz uma funcionalidade importante.

Tornar o JavaScript acessível envolve olhar para os seguintes aspectos. Cada um deles será discutido nas próximas lições.

- Quando usar manipuladores de eventos (*event handlers*), use apenas aqueles que são dispositivo-independentes (e.g. que não requeiram o uso apenas do rato).
- Os conteúdos e as funcionalidades geradas e controladas pelo JavaScript devem ser tornadas acessíveis às tecnologias de apoio.
- As páginas Web que utilizam *script* devem ser integralmente navegáveis usando o teclado.
- O JavaScript não deverá modificar ou sobrepôr o normal funcionamento do navegador de uma forma que cause confusão.
- Quando o JavaScript não se puder tornar nativamente acessível, deverá ser elaborada uma alternativa acessível.

---

### Comparação das Directrizes relativamente ao JavaScript

Quer a Secção 508 do *Rehabilitation Act* (nos Estados Unidos) quer as Directrizes de Acessibilidade para o Conteúdo da Web (nos Estados Membros da União Europeia), do [W3C](#), se referem à acessibilidade dos elementos programáveis (*scripts*). Ambas as normas requerem que o conteúdo e a funcionalidade dos elementos programáveis sejam acessíveis a tecnologias de apoio tais como leitores de ecrã. Adicionalmente, os utilizadores devem ter controlo sobre o conteúdo de base-tempo, o qual se altera com frequência e repentinamente com o tempo. Existem, no entanto, diferenças entre os dois guias de directrizes de acessibilidade. As [WCAG](#) requerem que o conteúdo e a funcionalidade seja acessível com o *script* desactivado e que os utilizadores devem ser alertados se o JavaScript modificar a aparência ou funcionalidade da janela do navegador, enquanto que a Secção 508 apenas requer que o *script*, ele próprio, seja concebido de forma acessível ou que seja fornecida uma alternativa acessível.

---

### Testar a fiabilidade do JavaScript

Tal como foi referido acima, as páginas Web devem ser totalmente funcionais quando o JavaScript se encontra desactivado. É isto que é solicitado ao nível da Prioridade 1 das Directrizes de Acessibilidade para o Conteúdo da Web. A Secção 508 não solicita que a página funcione no caso do JavaScript se encontrar desactivado, mas requer que os *scripts*, eles próprios, sejam nativamente acessíveis. Este tutorial ensinar-lhe-á estratégias para tornar os *scripts* nativamente acessíveis e assume que você, como criador de páginas Web, pretende alcançar um alto nível de acessibilidade ou conformidade para com as Directrizes de Acessibilidade para o Conteúdo da Web, e que vai também testar o seu trabalho para que ele funcione mesmo quando se desactiva o JavaScript.

#### Desativar o JavaScript

No final deste parágrafo, se tiver o JavaScript ativado, lerá "JavaScript on", caso esteja desativado vai aparecer "JavaScript off". O que consegue ler a seguir? - **JavaScript on.**  
<noscript>**JavaScript off**</noscript>

Siga as indicações para desactivar ou activar o JavaScript no seu navegador.

Teste uma página Web com o JavaScript inactivo e veja se o conteúdo e a funcionalidade são acessíveis. Certifique-se de que reactiva o JavaScript quando terminar.

**Internet Explorer 6.X**

1. Abra o Internet Explorer.
2. Selecione **Tools > Internet Options**.
3. Na caixa de diálogo do **Internet Options** selecione o separador **Security**.
4. Pressione o botão **Custom Level** existente mais abaixo. Abrir-se-á, por cima, a caixa de diálogo **Security Settings**.
5. Na categoria **Scripting**, ative/desative **Active Scripting, Allow paste options via script** e **Scripting of Java applets**.
6. Pressione duas vezes **OK** para fechar e sair.
7. Pressione **Refresh (tecla F5)**.

**Netscape 7.X**

1. Abra o Netscape.
2. Selecione **Edit > Preferences**.
3. Pressione a seta **next** para **Advanced**.
4. Pressione **Scripts & Plugins**.
5. Selecione/deselecione a opção **"Enable Javascript for"** por debaixo de **Navigator**.
6. Pressione **OK**.
7. Pressione **Reload**.

**Opera 7.X**

1. Abra o Opera.
2. Selecione **File > Quick Preferences**.
3. Selecione/deselecione **Enable Javascript**.
4. Pressione **Reload**.