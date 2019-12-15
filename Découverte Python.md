---


---

<h1 id="atelier-découverte-python">Atelier découverte Python</h1>
<p>L’objectif de cet atelier est de découvrir le langage <strong>Python</strong> à travers la programmation d’une carte <strong>BBC Micro:bit</strong>.</p>
<ul>
<li>Vous trouverez d’abord un <strong>mémo</strong> récapitulant les principales fonctionnalités du langage Python.</li>
<li>Vous devrez ensuite relever une liste de <strong>défis</strong> en programmant la carte micro:bit. A vous de jouer!</li>
</ul>
<h2 id="mémo-python">Mémo Python</h2>
<h3 id="généralités">Généralités</h3>
<ul>
<li>Un programme  Python est un texte qui permet de “commander” un ordinateur. Il est <strong>exécuté</strong> par un <strong>interpréteur</strong> situé dans la carte micro:bit. Le texte ne doit comporter <strong>aucune erreur</strong>, sinon l’interpréteur signale un problème lors de l’execution.</li>
<li>Les lignes commençant par <code>#</code> ne sont pas prises en compte par l’interpréteur, elles permettent de faire des <strong>commentaires</strong>, de donner des explications.<br>
<em>Exemple:</em></li>
</ul>
<pre class=" language-python"><code class="prism  language-python"><span class="token comment">#Cette ligne ne sera pas prise en compte </span>
</code></pre>
<ul>
<li><code>print()</code> permet d’écrire dans la <strong>console</strong>. C’est une sorte de journal dans lequel l’interpréteur peut écrire pendant l’exécution du programme. Ce journal peut être utile au programmateur pour voir ce qu’il s’est passé lors de l’exécution.<br>
<em>Exemple:</em></li>
</ul>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Bonjour!"</span><span class="token punctuation">)</span>
</code></pre>
<h3 id="variables">Variables</h3>
<p>Permet de garder en mémoire des valeurs au cours de l’exécution</p>
<p><em>Exemple:</em></p>
<pre class=" language-python"><code class="prism  language-python"><span class="token comment">#Donne la valeur 2 à la variable var1</span>
var1 <span class="token operator">=</span> <span class="token number">2</span>
<span class="token comment">#Donne la valeur 3 à la variable var2</span>
var2 <span class="token operator">=</span> <span class="token number">3</span>
<span class="token comment">#Ajoute 1 à la variable var2</span>
var2 <span class="token operator">=</span> var2 <span class="token operator">+</span><span class="token number">1</span>
<span class="token comment">#Calcul une somme puis l'affecte à la variable var3</span>
var3 <span class="token operator">=</span> var1<span class="token operator">+</span>var2
<span class="token comment">#Calcul un produit puis l'affecte à la variable var4</span>
var4 <span class="token operator">=</span> var3<span class="token operator">*</span>var1
<span class="token comment">#Ecrit dans la console la valeur de la variable var4</span>
<span class="token keyword">print</span><span class="token punctuation">(</span>var4<span class="token punctuation">)</span>
</code></pre>
<p><em>Dans la console:</em></p>
<pre><code>12
</code></pre>
<h3 id="conditionnelle">Conditionnelle</h3>
<p>Permet d’exécuter différentes instructions selon des conditions</p>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">if</span> <span class="token operator">&lt;</span>condition1<span class="token operator">&gt;</span><span class="token punctuation">:</span>
	<span class="token comment">#Si la condition 1 est vérifiée, execute le bloc d'instruction 1</span>
	<span class="token operator">&lt;</span>bloc_instruction1<span class="token operator">&gt;</span>
<span class="token keyword">elif</span> <span class="token operator">&lt;</span>condition2<span class="token operator">&gt;</span><span class="token punctuation">:</span>
	<span class="token comment">#Sinon, si la condition 2 est vérifiée, execute le bloc d'instruction 2</span>
	<span class="token operator">&lt;</span>bloc_instruction2<span class="token operator">&gt;</span>
<span class="token keyword">else</span> <span class="token punctuation">:</span>
	<span class="token comment">#Sinon, execute le bloc d'instruction 3</span>
	<span class="token operator">&lt;</span>bloc_instruction3<span class="token operator">&gt;</span>
</code></pre>
<p><em>Exemple:</em></p>
<pre class=" language-python"><code class="prism  language-python">var1 <span class="token operator">=</span> <span class="token number">7</span>
<span class="token keyword">if</span> var1 <span class="token operator">&lt;</span> <span class="token number">0</span> <span class="token punctuation">:</span>
	<span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Plus petit que 0"</span><span class="token punctuation">)</span>
<span class="token keyword">elif</span> var1 <span class="token operator">&lt;</span> <span class="token number">10</span> <span class="token punctuation">:</span>
	<span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Entre 0 et 10"</span><span class="token punctuation">)</span>
<span class="token keyword">else</span> <span class="token punctuation">:</span>
	<span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Plus grand que 10"</span><span class="token punctuation">)</span>
</code></pre>
<p>Dans la console:</p>
<pre><code>Entre 0 et 10
</code></pre>
<p><em>Remarque :</em><br>
Le nombre de  “cas” est variable. On peut utiliser  un <code>if</code> seul, le couple <code>if</code>/<code>else</code>  ou autant de <code>elif</code> que l’on souhaite :  <code>if</code>/<code>elif</code>/…/<code>elif</code>/<code>else</code></p>
<h3 id="boucle-bornée">Boucle bornée</h3>
<p>Répète un bloc d’instruction un certain nombre de fois</p>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">for</span> <span class="token operator">&lt;</span>variable<span class="token operator">&gt;</span> <span class="token keyword">in</span> <span class="token builtin">range</span><span class="token punctuation">(</span><span class="token operator">&lt;</span>nombre<span class="token operator">&gt;</span><span class="token punctuation">)</span><span class="token punctuation">:</span>
	<span class="token comment">#Répète un bloc d'instruction &lt;nombre&gt; de fois</span>
	<span class="token comment">#La variable &lt;variable&gt; peut être utilisée dans la boucle, elle commence à 0 et est automatiquement </span>
	<span class="token comment">#augmentée de 1 à chaque tour</span>
	<span class="token operator">&lt;</span>bloc_instruction<span class="token operator">&gt;</span>
</code></pre>
<p><em>Exemple:</em></p>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">for</span> var1 <span class="token keyword">in</span> <span class="token builtin">range</span><span class="token punctuation">(</span><span class="token number">5</span><span class="token punctuation">)</span><span class="token punctuation">:</span>
	<span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Dans la boucle, valeur de var1: "</span><span class="token punctuation">)</span>
	<span class="token keyword">print</span><span class="token punctuation">(</span>var1<span class="token punctuation">)</span>
<span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Plus dans la boucle"</span><span class="token punctuation">)</span>
</code></pre>
<p><em>Dans la console:</em></p>
<pre><code>Dans la boucle, valeur de var1: 0
Dans la boucle, valeur de var1: 1
Dans la boucle, valeur de var1: 2
Dans la boucle, valeur de var1: 3
Dans la boucle, valeur de var1: 4
Plus dans la boucle
</code></pre>
<h3 id="boucle-non-bornée">Boucle non bornée</h3>
<p>Répète un bloc d’instruction tant qu’une condition est vraie</p>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">while</span> <span class="token operator">&lt;</span>condition<span class="token operator">&gt;</span><span class="token punctuation">:</span>
	<span class="token comment">#Répète le bloc d'instruction tant que la condition est vraie</span>
	<span class="token operator">&lt;</span>bloc_instruction<span class="token operator">&gt;</span>
</code></pre>
<p><em>Exemple:</em></p>
<pre class=" language-python"><code class="prism  language-python">var1 <span class="token operator">=</span> <span class="token number">6</span>
<span class="token keyword">while</span> var1 <span class="token operator">&gt;</span> <span class="token number">0</span><span class="token punctuation">:</span> 
	var1 <span class="token operator">=</span> var1<span class="token number">-1</span>
	<span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Dans la boucle, valeur de var1: "</span><span class="token punctuation">)</span>
	<span class="token keyword">print</span><span class="token punctuation">(</span>var1<span class="token punctuation">)</span>
<span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Plus dans la boucle"</span><span class="token punctuation">)</span>
</code></pre>
<p><em>Dans la console</em>:</p>
<pre><code>Dans la boucle, valeur de var1: 5
Dans la boucle, valeur de var1: 4
Dans la boucle, valeur de var1: 3
Dans la boucle, valeur de var1: 2
Dans la boucle, valeur de var1: 1
Dans la boucle, valeur de var1: 0
Plus dans la boucle
</code></pre>
<h3 id="fonction">Fonction</h3>
<p>Une fonction permet d’isoler un ensemble d’instruction qui réalisent la même tâche mais avec des paramètres différents.</p>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">def</span> <span class="token operator">&lt;</span>nom_fonction<span class="token operator">&gt;</span> <span class="token punctuation">(</span><span class="token operator">&lt;</span>liste_paramètres<span class="token operator">&gt;</span><span class="token punctuation">)</span><span class="token punctuation">:</span>
	<span class="token operator">&lt;</span>bloc_instruction<span class="token operator">&gt;</span>
</code></pre>
<p><em>Exemple:</em></p>
<pre class=" language-python"><code class="prism  language-python"><span class="token comment">#La définition de la fonction se fait avant son utilisation</span>
<span class="token keyword">def</span> <span class="token function">puissance</span><span class="token punctuation">(</span>base<span class="token punctuation">,</span>exposant<span class="token punctuation">)</span><span class="token punctuation">:</span>
	resultat <span class="token operator">=</span> base
	<span class="token keyword">for</span> i <span class="token keyword">in</span> <span class="token builtin">range</span><span class="token punctuation">(</span>exposant<span class="token number">-1</span><span class="token punctuation">)</span><span class="token punctuation">:</span>
		resultat <span class="token operator">=</span> resultat <span class="token operator">*</span> base
	<span class="token keyword">print</span><span class="token punctuation">(</span>resultat<span class="token punctuation">)</span>
<span class="token comment">#On peut ensuite utiliser la fonction plus loin dans le programme</span>
puissance<span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">,</span><span class="token number">3</span><span class="token punctuation">)</span>
puissance<span class="token punctuation">(</span><span class="token number">10</span><span class="token punctuation">,</span><span class="token number">4</span><span class="token punctuation">)</span>
</code></pre>
<p><em>Dans la console</em>:</p>
<pre><code>8
10000
</code></pre>
<h2 id="défis-1-le-smiley">Défis 1: Le smiley</h2>
<p>|</p>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">for</span> i <span class="token keyword">in</span> <span class="token builtin">range</span><span class="token punctuation">(</span><span class="token number">4</span><span class="token punctuation">)</span>
</code></pre>
<p><img src="https://docs.google.com/uc?id=1qLTLoWg2SzmAfVda-EX8U4G9FzQW1TFz" alt="enter image description here"></p>

