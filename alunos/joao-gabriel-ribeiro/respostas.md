5. Aprendendo a simular com o simuladores SPICE.

a) Faça um resumo em forma de tutorial sobre o como funciona o SPICE e responda: 
1. O que é o NETLIST?
Forma que o SPICE utiliza pra chamar uma simulação, transcrevendo para modo texto.

2. Como descrever o NETLIST de um circuito?
O NETLIST é transcrito em uma linha, as conexões são descritas por nós, normalmente são escritos em números

3. Como é representado cada um dos componentes? Explique com um exemplo.
Representando uma fonte de tensão: V1 (fonte 1)  N001 (primeiro 0 é o nó de referência GROUND) (01 é o nó 1) 5V (valor de V1).

4. O que é o “LABEL” de um nó e qual a vantagem de usar o mesmo?
Quando você da nome as terminações/nós, eu não preciso sempre ficar puxando um fio, posso colocar um nome que o programa entende que o meu  circuito continua a partir de lá.

5. Quais os componentes básicos implementados no SPICE? (resistor, capacitor etc)
Resistores, capacitores, indutores, diodos, fontes de tensão, transistores,terminal terra, amplificador operacional,e outros.

6. O que é um “SUBCKT”? Faça um exemplo.
É um subcircuito, feito a partir de um outro circuito que já existe, pode ser utilizá-lo mais vezes no mesmo circuito ou nos próximos circuitos

7. Como incluir novos modelos de componentes em um simulador SPICE?
Basta ir em file e open, selecionar o arquivo que quer adicionar. É possível fazer download de arquivos de terceiros na internet.

 b) Faça um resumo em forma de tutorial sobre o como funciona os parâmetros de simulação do SPICE, respondendo: 

1. O que é simulação transiente (.trans)? Quando usar? Faça um exemplo.
Quando quero simular algo em função do tempo, usado em circuitos que dependem de carga, corrente ou tensão. .TRAN 1NS 100NS

2. O que é simulação “ DC operating point” (.op)? Quando usar? Faça um exemplo
Esta declaração instrui  a calcular os pontos operacionais DC:tensão nos nós, corrente em cada fonte de tensão e ponto operacional para cada elemento

3. Quando usar .trans ou .op no SPICE?

4. O que faz a diretiva “.step”? Forneça exemplos de utilização
Este comando é usado para varredura de parâmetro. Isso faz com que uma análise seja realizada repetidamente durante a etapa do parâmetro específico. .step param X list .1u .2u .3u

5. O que faz a diretiva “.means”? Forneça exemplos de utilização.
É utilizado para calcular certas condições do circuito como a média da tensão de saída

6. O que é a simulação “DC sweep” (.dc)? Quando usar? Faça um exemplo.
Esta instrução permite incrementar (varrer) uma fonte independente em um determinado intervalo com uma etapa especificada, pode ser útil para obter características de saída de dispositivos semicondutores. .DC VIN 0.25 5.0 0.25

7. Como simular um circuito em diferentes temperaturas de funcionamento?
 Com o comando .temp e os parâmetros de temperatura que desejo medir
















