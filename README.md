<div align="center">
<img width=360px height=370px src="https://user-images.githubusercontent.com/110111018/215011072-ce2f4508-2962-4078-961b-0289cf9b73b0.png"/>
<br>
<img src="https://img.shields.io/github/license/lulu-ancacio/lulu-ancacio?style=plastic">
<img src="http://img.shields.io/static/v1?label=language&message=lua&color=rgb(138,43,226)&style=plastic">
</div>

<h2>Módulo</h2>
<p>
O horizonte da matemática é tão vasto e incógnito, que casualmente nos deparamos com valores inenarráveis à olho leigo. Estas são as constantes matemáticas. Números de utilidade ampla, porém específica, e que muitas vezes são definidas por operações abstratas do Cálculo! Utiliza-se <strong>allConstants</strong> para ter acessível todas estas variáveis extensas, com o máximo de precisão possível. Crie novas experiências e veja a matemática pura agir em sua mais computável forma!
<br>
Quais constantes este módulo contempla?
<ul>
<li>Número de ouro: φ</li>
<li>Constante de Ramanujan</li>
<li>Constante Apéry: ζ(3)</li>
<li>Tau: τ</li>
<li>Constante Euler-Mascheroni: γ</li>
<li>Constante omega: Ω</li>
<li>Constante de Landau–Ramanujan: Κ</li>
<li>Constante de Catalan: K ou G</li>
<li>Constante de Plástico: Ρ ou ρ</li>
<li>Constante de Meissel-Mertens: M</li>
<li>Número de "Super Ouro": ψ</li>
<li>Constante de Kepler–Bouwkamp</li>
<li>Constante de Wallis</li>
<li>Constante de Lemniscata: ϖ</li>
<li>Constante de Erdős–Borwein: E</li>
<li>Constante de Ramanujan-Soldner: μ</li>
<li>Constante de Gauss: G</li>
<li>Primeira Constante de Fração Continua: C₁</li>
<li>Constante de Glaisher-Kinkelin: A</li>
<li>Número de Dottie</li>
<li>Constante de Cahen: C</li>
<li>Constante Parabólica Universal: P₂</li>
<li>Constante de Gelfond</li>
<li>Constante de Gelfond–Schneider</li>
<li>Ângulo de Ouro: g ou GA</li>
<li>Constante de Sierpiński</li>
<li>Constante de Gieseking: G</li>
<li>Constante de Bernstein: β</li>
<li>Constante dos Primos Gêmeos "Twin Primes": Π₂</li>
<li>Constante de Prouhet–Thue–Morse</li>
<li>Constante de Golomb-Dickman: λ</li>
<li>Constante de Feller-Tornier</li>
<li>Constante de khinchin: K</li>
<li>Constante de Lévy: β</li>
<li>Constante de Copeland–Erdős</li>
<li>Constante de Mills: θ</li>
<li>Constante de Gompertz: G</li>
<li>Constante de Van der Pauw</li>
<li>Ângulo Mágico: θₘ</li>
<li>Constante de Artin</li>
<li>Constante de Porter: C</li>
<li>Constante de Lochs: L</li>
<li>Constante do tesserato de DeVicci</li>
<li>Constante de Niven</li>
<li>Constante de Stephens: Cₛ</li>
<li>Constante de Feigenbaum Alfa: α</li>
<li>Constante de Feigenbaum Delta: δ</li>
<li>Constante de Robbins: Δ(3)</li>
<li>Constante de Erdõs-Tenenbaum-Ford: δ</li>
<li>Constante de Conway: λ</li>
<li>Constante de Hafner-Sarnak-McCurley: D(n) n→∞</li>
<li>Constante de Backhouse: B</li>
<li>Constante de Komornik-Loreti: q</li>
<li>Constante de Heath-Brown-Moroz</li>
<li>Constante MRB: S</li>
<li>Constante Foias: α</li>
<li>Constante de Taniguchi</li>
<li>Constante de Varga: V</li>
<li>Constante de Pell: P</li>
<li>Constante de Wyler</li>
<li>Constante de Lehmer</li>
<li>Constante Coelho "Rabbit Constant": R</li>
<li>Constante de Tribonacci</li>
<li>Constante de Tetranacci</li>
<li>Constante de Pentanacci</li>
<li>Constante de Hexanacci</li>
<li>Constante de Heptanacci</li>
<li>Constante de Freiman: F</li>
<li>Constante de Silver: S</li>
<li>Constante de Gauss-Kuzmin-Wirsing: λ</li>
<li>Constante de Alladi-Grinstead</li>
<li>Constante de Gelo Quadrado de Lieb "Lieb's Square Ice Constant"</li>
</ul>
</p>
<h2>Fidedignidade</h2>
<p>
Embora seja impossível repoduzir a irracionalidade das constantes supracitas, podemos solucioná-las com a maior precisão possível dentro da linguagem Lua, usando 16 casas decimais de seus valores. Abaixo está destacado demonstrações da veracidade que o uso deste módulo fornece à expressões:
</p>

<h3>Constante de Ramanujan</h3>
<img src="https://user-images.githubusercontent.com/110111018/215370950-d79810ec-51ea-4eb0-83a0-c9676abf12c9.png">
<br>
<p>
Vamos calcular o valor de pi usando a Constante de Ramanujan (definida aqui pelo valor de 262537412640768743.99999999999925). Para isso, é preciso somente uma operação logarítmica.
</p>

```lua
local ramanujan = allConstants.ramanujan
local piForRamanujan = math.log(ramanujan, math.exp(1))/math.sqrt(163)

print(piForRamanujan)
print(math.pi)

>>3.1415926535898
>>3.1415926535898
```

<p>
A variável <i>piForRamanujan</i> recebe as operações inversas necessárias para chegar ao valor de pi e, como podemos ver, converge à definição de pi da própria biblioteca Lua.
</p>

<h3>Constante de Glaisher–Kinkelin</h3>
<img src="https://user-images.githubusercontent.com/110111018/215250119-ba38afc4-a50f-43d8-b7e0-789fdb61ec5a.png">&nbsp; com &nbsp;
<img src="https://user-images.githubusercontent.com/110111018/215250118-db63f415-0706-444a-b8ec-ddaf8ded7557.png">
<br>
<p>
Vamos agora comparar o valor da Constante de Glaisher–Kinkelin dada no módulo com a construção de sua definição.
<br>
Estabelecendo <i>A</i> como o valor decimal da Constante de Glaisher–Kinkelin, <i>def</i> como sua definição mostrada a cima, <i>exp</i> como <i>ζ ' (2)</i> e <i>y</i> como a Constante Euler-Mascheroni, calculamos: 
</p>

```lua
local A = allConstants.glaisherKinkelin
local y = allConstants.eulerMascheroni
local exp = ((math.pi^2)/6)*(y+math.log(2*math.pi, math.exp(1))-12*math.log(A, math.exp(1)))
local definicao = ((2*math.pi)^(1/12)) * (math.exp(((Y*math.pi^2)/6)-exp))^(1/(2*math.pi^2))

print(A)
print(definicao)

>> 1.2824271291006
>> 1.2824271291006
```

<p>
Observa-se que a orquestra de constantes da definição da constante <i>A</i> convergem para seu valor decimal programado.
</p>

<h3>Constante de Sierpiński</h3>
<img src="https://user-images.githubusercontent.com/110111018/215251254-3e8860b6-53c0-4d83-922f-5bcee9a3c6d5.png">
<br>
<p>
Fazendo agora outra comparação, usando o valor decimal da Constante de Sierpiński e sua definição explicitada a cima. Temos aqui <i>K</i> representando a váriavel mormente no tópico, <i>y</i> a Constante Euler-Mascheroni, <i>G</i> a Constante de Gauss e <i>def</i> a definição da constante <i>K</i>.
</p>

```lua
local K = allConstants.sierpinski
local y = allConstants.eulerMascheroni
local G = allConstants.gauss
local definicao = math.pi*math.log(((math.exp(2*y))/(2*G^2)), math.exp(1))

print(K)
print(definicao)

>>2.5849817595793
>>2.5849817595793
```

<p>
Computando a definição da constante <i>K</i> chegamos ao mesmo resultado do valor introduzido no módulo.
</p>

<h3>Constante de Plástico</h3>
<img src="https://user-images.githubusercontent.com/110111018/215251257-9eeb0f41-1f95-4c14-a457-4dd2e9d6d06f.png">
<br>
<p>
A conhecida Constante de Plástico é o valor que satisfaz a igualdade apresentada. Pode-se computá-la facilmente da seguinte forma:
</p>

```lua
local p = allConstants.plastic

print(p^3)
print(p+1)

>>2.3247179572447
>>2.3247179572447
```

<p>
A igualdade transpare-se utilizando o decimal decimal estabelecido para a Constante de Plástico.
</p>

<h3>Conclusão</h3>
<p>
Fazendo uso do módulo <strong>allConstants</strong> foi possível realizar operações normalmente privilegiadas à papel e caneta ou calculadoras científicas, logrando de exelentes resultados com o máximo de precisão concebível.
</p>

<h2>Fontes</h2>
<p>
Todas as constantes deste módulos são oriundas das enciclopédias <a href="https://wikipedia.org">Wikipédia</a> e <a href="https://oeis.org">OEIS</a>, do acervo matemático da <a href="https://mathworld.wolfram.com/">MathWorld</a> e da lista de constantes matemáticas da <a href="https://play.google.com/store/apps/details?id=cz.hipercalc">HiPER Calc</a>.
</p>
