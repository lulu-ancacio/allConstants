<div align="center">
<img width=360px height=370px src="https://user-images.githubusercontent.com/110111018/215011072-ce2f4508-2962-4078-961b-0289cf9b73b0.png"/>
<br>
<img src="https://img.shields.io/github/license/lulu-ancacio/REPOSITORIO?style=plastic">
<img src="http://img.shields.io/static/v1?label=language&message=lua&color=rgb(138,43,226)&style=plastic">
</div>

<h2>Módulo</h2>
<p>
O horizonte da matemática é tão vasto e incógnito, que casualmente nos deparamos com valores inenarráveis à olho leigo. Estas são as constantes matemáticas. Números de utilidade ampla, porém específica, e que muitas vezes são definidas por operações abstratas do Cálculo! Utiliza-se <strong>allConstants</strong> para ter acessível todas estas variáveis extensas, com o máximo de precisão possível. Crie novas experiências e veja a matemática pura agir em sua mais computável forma!
<br>
Quais constantes este módulo contempla?
<ul>
<li>Número de ouro: φ</li>
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
</ul>
</p>
<h2>Fidedignidade</h2>
<p>
Embora seja impossível repoduzir a irracionalidade das constantes supracitas, podemos solucioná-las com a maior precisão possível dentro da linguagem Lua, usando 16 casas decimais de seus valores. Abaixo está destacado demonstrações da veracidade que o uso deste módulo fornece à expressões:
</p>
<br>
<h3>Constante de Glaisher–Kinkelin</h3>
<img src="https://user-images.githubusercontent.com/110111018/215250119-ba38afc4-a50f-43d8-b7e0-789fdb61ec5a.png">&nbsp; com &nbsp;
<img src="https://user-images.githubusercontent.com/110111018/215250118-db63f415-0706-444a-b8ec-ddaf8ded7557.png">
<br>
<p>
Estabelecendo <i>exp = ζ'(2)</i>, <i>A</i> como a Constante de Glaisher–Kinkelin definida no módulo e N como a expressão que define A na imagem a cima, temos: 
</p>

```lua
local exp = ((math.pi^2)/6)*(allConstants.eulerMascheroni+math.log(2*math.pi, math.exp(1))-12*math.log(allConstants.glaisherKinkelin, math.exp(1)))
local A = allConstants.glaisherKinkelin
local N = ((2*math.pi)^(1/12)) * (math.exp(((allConstants.eulerMascheroni*math.pi^2)/6)-exp))^(1/(2*math.pi^2))

print(A)
print(N)

>> 1.2824271291006
>> 1.2824271291006
```

<p>
Ou seja, foi possível transcrever a definição da Constante de Glaisher–Kinkelin  com a máxima precisão, logrando de resultados satisfatórios tanto no valor predefinido da constante quanto na expressão computada.
</p>
<br>
<h3>Constante Omega</h3>
<img src="https://user-images.githubusercontent.com/110111018/215250892-679b4028-5f21-4a7b-b67e-4aa22152d16f.png">
<h3>Constante de Plástico</h3>
<img src="https://user-images.githubusercontent.com/110111018/215251257-9eeb0f41-1f95-4c14-a457-4dd2e9d6d06f.png">
<h3>Constante de Sierpiński</h3>
<img src="https://user-images.githubusercontent.com/110111018/215251254-3e8860b6-53c0-4d83-922f-5bcee9a3c6d5.png">
