<script src='https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.4/MathJax.js?config=default'></script>

<h1>Concreto Protendido: Atrito</h1>

<p align="justify">A calculadora Atrito do módulo Concreto Protendido efetua o cálculo das perdas de protensão por atrito, em uma única seção, segundo as prescrições da NBR 6118.<br>
<br>
Para utilizar a ferramenta acesse a plataforma <a href="https://www.coretectools.com.br/" target="_blank">Coretec Tools</a>. Dentro do menu <b>Painel</b> acesse as ferramentas do curso de <b>Engenhgaria Civil</b>.</p>

<h2>Procedimento de cálculo</h2>

<p align="justify">O procedimento de cálculo da perda de protensão por atrito segue a bibliografia de Carvalho [1] e também as prescrições do item 9.6.3.3.2.2 da NBR 6118 [2].<br>
<br>
Para efetuar o cálculo da perda de protensão basta a aplicação da equação (1):</p>

1:  $$\Delta P = P_i^t.(1-e^{-(\mu.\sum\alpha+k.x)})$$

<p align="justify">O valor da carga final de protensão ao final da perda (\(P_i^{t+1}\)), tensão de protensão após a aplicação da perda (\(sigma_i^{t+1}\)) e a perda de percentual são dadas pelas equações (2) a (4):</p>

2:  $$P_i^{t+1} = P_i^t.(e^{-(\mu.\sum\alpha+k.x)})$$
3:  $$\sigma_i^{t+1}=\frac{P_i^{t+1}}{A_p}$$
4:  $$\Delta%=\left(\Delta P/P_i^t\right).100$$

<p align="justify">A perda percentual de tensão é dada pela equação (5):</p>

$$\mathrm{\Delta\sigma}=\sigma_i^{t+1}-\sigma_i^t$$

<h2>Como utilizar a ferramenta</h2>

<p align="justify">O programa Concreto Protendido necessita do seguinte conjunto de dados:</p>

<table>
<thead>
  <tr>
    <th>Variável</th>
    <th>Descrição</th>
    <th>unidade</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>u</td>
    <td>Coeficiente de atrito aparente entre cabo e bainha</td>
    <td>1/rad</td>
  </tr>
  <tr>
    <td>k</td>
    <td>Coeficiente de perda provocado por curvaturas não intencionais do cabo</td>
    <td>1/m</td>
  </tr>
  <tr>
    <td>P_i</td>
    <td>Carga inicial de protensão sem perdas</td>
    <td>kN</td>
  </tr>
  <tr>
    <td>Sigma_i</td>
    <td>Tensão inicial de protensão sem perdas</td>
    <td>kPa</td>
  </tr>
  <tr>
    <td>x</td>
    <td>Abcissa do cabo que deseja-se calcular a perda</td>
    <td>m</td>
  </tr>
  <tr>
    <td>A_p</td>
    <td>Área de aço total das cordoalhas na seção x</td>
    <td>m²</td>
  </tr>
  <tr>
    <td>\alpha</td>
    <td>Soma dos ângulos de desvios previstos compreendido entre 0 e&nbsp;&nbsp;a abcissa&nbsp;&nbsp;de valor x</td>
    <td>rad</td>
  </tr>
</tbody>
</table>

<p align="justify">A saída do programa Concreto Protendido devolve os seguintes resultados:</p>

<table>
<thead>
  <tr>
    <th>Variável</th>
    <th>Descrição</th>
    <th>unidade</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>\Delta</td>
    <td>Perda de protensão</td>
    <td>%</td>
  </tr>
  <tr>
    <td>P_{t+i}</td>
    <td>Carga final de protensão após as perdas</td>
    <td>kN</td>
  </tr>
  <tr>
    <td>Sigma_{t+i}</td>
    <td>Tensão inicial de protensão após as perdas</td>
    <td>kPa</td>
  </tr>
</tbody>
</table>

<h3>Exemplo</h3>

<p align="justify">Considere a viga biapoiada apresenta por Thomaz[3] com vão de 30 metros e com tensão incial de protensão de 1.425.000 KPa. Deseja-se encontrar a perda de perda de protensão na seção de 15 m considerando que o perfil do cabo é parabólico e que as cordoalhas são protegidas por bainhas metálicas.</p>

* Dados de entrada do problema:
 * 1 Cabo de $\fi$ 12.7 mm
 * A_p 1 cabo = 1,002 cm²
 * \alpha = 0.173 rad
 * 
