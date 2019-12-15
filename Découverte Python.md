---


---

<h1 id="atelier-découverte-python">Atelier découverte Python</h1>
<p>Lors de cet atelier, tu vas apprendre à programmer la carte <strong>BBC Micro:bit</strong> à l’aide du langage de programmation <strong>Python</strong>.<br>
Tu vas devoir surmonter un maximum de <strong>défis</strong> pour gagner tes <strong>badges</strong> de développeur Python :</p>

<table>
<thead>
<tr>
<th><img src="https://docs.google.com/uc?id=1mxdm7U4UIaIGgUOoun9pMSYMnB011HcJ" alt=""></th>
<th><img src="https://docs.google.com/uc?id=18HiRKTA-m0i2rHz9fLgW6anVe9DVhEzr" alt=""></th>
<th><img src="https://docs.google.com/uc?id=16c0XypJpKssvt1ibHtbL_xHa2j8DCevA" alt=""></th>
</tr>
</thead>
<tbody>
<tr>
<td>3 défis relevés</td>
<td>6 défis relevés</td>
<td>9 défis relevés</td>
</tr>
</tbody>
</table><p>Pour y arriver, tu disposes:</p>
<ul>
<li>d’une <strong>carte</strong> micro:bit et de son câble USB</li>
</ul>
<p><img src="https://docs.google.com/uc?id=11Me-Sfi0Nzcr3sPgfg-4r9cN6gqxOoeF" alt=""><img src="https://docs.google.com/uc?id=1q_2OtzdZw47tGmzcM8U0k4qPHO-tWVAO" alt=""></p>
<ul>
<li>de l’<strong>environnement de développement</strong> Mu</li>
</ul>
<p><img src="https://docs.google.com/uc?id=1rBgO5Vv6Ipov51FQncRIIMywJ_fyWY6I" alt=""></p>
<ul>
<li>d’un <strong>guide de démarrage</strong>, te permettant de prendre en main l’environnement</li>
<li>d’un <strong>mémo</strong> récapitulant les <strong>principales fonctionnalités</strong>  du langage Python</li>
<li>d’une <strong>liste de défis</strong> à relever</li>
</ul>
<p>A toi de jouer! Bonne chance!</p>
<h2 id="guide-de-démarrage">Guide de démarrage</h2>
<ul>
<li>Un programme  Python est un texte qui permet de “commander” un ordinateur (la carte micro:bit est un petit ordinateur). Dans notre cas, ce programme est <strong>exécuté</strong> par un <strong>interpréteur</strong> situé dans la carte. Le texte ne doit comporter <strong>aucune erreur</strong>, sinon l’interpréteur signale un problème et l’exécution s’arrête.</li>
<li>Les lignes commençant par <code>#</code> ne sont pas prises en compte par l’interpréteur, elles permettent de faire des <strong>commentaires</strong>, de donner des explications.<br>
<em>Exemple:</em></li>
</ul>
<pre class=" language-python"><code class="prism  language-python"><span class="token comment">#Cette ligne ne sera pas prise en compte </span>
</code></pre>
<ul>
<li><code>print()</code> permet d’écrire dans la <strong>console</strong>. C’est une sorte de journal dans lequel l’interpréteur peut écrire pendant l’exécution du programme. Ce journal peut être utile au programmeur pour voir ce qu’il s’est passé lors de l’exécution. Dans l’environnement de développement Mu,  il est possible d’accéder à ce qui a été écrit dans la console en cliquant sur le bouton “REPL”<br>
<img src="https://docs.google.com/uc?id=1aGNmo8mjkL7Cv1RSey_7gwB4jtTMNTKP" alt=""></li>
</ul>
<p><em>Exemple:</em><br>
dans le programme:</p>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">print</span><span class="token punctuation">(</span><span class="token string">"Bonjour!"</span><span class="token punctuation">)</span>
</code></pre>
<p>dans la console:<br>
<mark>Photo à ajouter</mark></p>
<ul>
<li>Les programmes qui utilisent la carte micro:bit doivent <strong>absolument commencer par</strong>:</li>
</ul>
<pre class=" language-python"><code class="prism  language-python"><span class="token keyword">from</span> microbit <span class="token keyword">import</span> <span class="token operator">*</span>
</code></pre>
<ul>
<li>Pour <strong>téléverser</strong> un programme que tu as écrit dans Mu vers la carte micro:bit, il faut cliquer sur le bouton “Flasher”<br>
<img src="https://docs.google.com/uc?id=16K_p-_F61BJJDsDU0nlLp0raK51ba5K9" alt=""></li>
</ul>
<h2 id="mémo-python">Mémo Python</h2>
<h3 id="variables">Variables</h3>
<p>Permet de garder en mémoire des valeurs au cours de l’exécution</p>
<p><em>Exemple:</em></p>
<pre class=" language-python"><code class="prism  language-python"><span class="token comment">#Donne la valeur 2 à la variable var1</span>
var1 <span class="token operator">=</span> <span class="token number">2</span>
<span class="token comment">#Donne la valeur 3 à la variable var2</span>
var2 <span class="token operator">=</span> <span class="token number">3</span>
<span class="token comment">#Ajoute 1 à la variable var2</span>
var2 <span class="token operator">=</span> var2 <span class="token operator">+</span><span class="token number">1</span>
<span class="token comment">#Calcul un produit puis l'affecte à la variable var3</span>
var3 <span class="token operator">=</span> var2<span class="token operator">*</span>var1
<span class="token comment">#Ecrit dans la console la valeur de la variable var3</span>
<span class="token keyword">print</span><span class="token punctuation">(</span>var3<span class="token punctuation">)</span>
</code></pre>
<p><em>Dans la console:</em></p>
<pre><code>8
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
<span class="token comment">#Ici, on définie une fonction que calcul une puissance connaissant la base et l'exposant</span>
<span class="token keyword">def</span> <span class="token function">puissance</span><span class="token punctuation">(</span>base<span class="token punctuation">,</span>exposant<span class="token punctuation">)</span><span class="token punctuation">:</span>
	resultat <span class="token operator">=</span> base
	<span class="token keyword">for</span> i <span class="token keyword">in</span> <span class="token builtin">range</span><span class="token punctuation">(</span>exposant<span class="token number">-1</span><span class="token punctuation">)</span><span class="token punctuation">:</span>
		resultat <span class="token operator">=</span> resultat <span class="token operator">*</span> base
	<span class="token keyword">print</span><span class="token punctuation">(</span>resultat<span class="token punctuation">)</span>
<span class="token comment">#On peut ensuite utiliser la fonction plus loin dans le programme</span>
puissance<span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">,</span><span class="token number">3</span><span class="token punctuation">)</span> <span class="token comment">#Calcul 2 exposant 3</span>
puissance<span class="token punctuation">(</span><span class="token number">10</span><span class="token punctuation">,</span><span class="token number">4</span><span class="token punctuation">)</span> <span class="token comment">#Calcul 10 exposant 4</span>
</code></pre>
<p><em>Dans la console</em>:</p>
<pre><code>8
10000
</code></pre>
<h2 id="défis-1-le-smiley">Défis 1: Le smiley</h2>
<h3 id="défis">Défis</h3>
<blockquote>
<p>Afficher un smiley sur l’écran de la carte micro:bit</p>
</blockquote>
<p><img src="https://docs.google.com/uc?id=1JFzH6CJBEGwXW3QAYFm8C5e7aFfX_3HA" alt=""></p>
<h3 id="aide">Aide:</h3>
<p>Tu disposes de la fonction:</p>
<pre class=" language-python"><code class="prism  language-python">display<span class="token punctuation">.</span>set_pixel<span class="token punctuation">(</span><span class="token operator">&lt;</span>num_colonne<span class="token operator">&gt;</span><span class="token punctuation">,</span><span class="token operator">&lt;</span>num_ligne<span class="token operator">&gt;</span><span class="token punctuation">,</span><span class="token operator">&lt;</span>intentisité<span class="token operator">&gt;</span><span class="token punctuation">)</span>
</code></pre>
<p>pour allumer la LED de la colonne <code>&lt;num_colonne&gt;</code> (nombre entre 0 et 4) et de la ligne <code>&lt;num_ligne&gt;</code> (nombre entre 0 et 4) avec une intensité <code>&lt;intensité&gt;</code> (nombre entre 0 et 9)</p>
<h2 id="défis-2-la-pluie">Défis 2: La pluie</h2>
<blockquote>
<p>Présenter une goute d’eau</p>
</blockquote>

