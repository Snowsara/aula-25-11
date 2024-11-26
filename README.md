# Aula 25-11 - App Conversão de moeda

## Avaliação

* Implemente para que o usuário possa fazer conversão de outras moedas (mínimo + 3 moedas);
* Descreva abaixo o seu entendimento acerca desta atividade, explorando as funcionalidades das classes que contruímos e os principais pontos da aplicação;

## Entrega

* Clone este repositório e faça o que se pede;
* Realize um commit das suas alterações no seu repositório;
* Envie o link do repositório na avaliação gerada no classroom;

## Descritivo do Aluno:

Formulário de conversão de moeda pelo angular. 
Usando a vinculação primordial do angular foi possível o usuário mais de uma opção com o [(ngModel)]="opcaoEscolhida",
essa variavel armazena assim o valor da moeda selecionada. Na linha 16, o usuário podera o valor que deseja converter 
com um botão para usuário apertar e calcular a conversão. 
"<input [(ngModel)]="valor" type="number">" campo de entrada onde o coloca um valor. sendo assim, o [(ngModel)] vincula 
esse campo à variável valor no componente Angular, o que significa que o valor digitado será armazenado na variável valor. 
<button (click)="calcularConversao()">Calcular</button>: o botão chamando a função calcularConversao(). Quando o usuário
clica no botão, essa função será executada para calcular a conversão, usando o valor inserido e a opção de moeda escolhida.
<input [(ngModel)]="resultado" type="number" disabled>, campo de entrada exibirá o valor convertido. Por fim, o [(ngModel)]
vincula esse campo à variável resultado no componente Angular, o que significa que o valor da conversão será armazenado na 
variável resultado. O atributo disabled é usado para impedir que o usuário edite esse campo. O valor exibido será apenas o
resultado calculado pela função calcularConversao().
Por ultimo, o código que esta no converter-moeda.component.ts, permite ao usuário escolher uma moeda, inserir um valor e 
calcular o valor convertido usando as taxas de câmbio fornecidas por uma API através do ConversorService. Essa taxa de conversão
é extraída da resposta da API e usada para calcular o valor final, que é armazenado em resultado.

