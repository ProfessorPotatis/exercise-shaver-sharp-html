<h1 id="knivskarp-html"><i class="fa fa-laptop"></i> Knivskarp HTML</h1>
<ul class="fa-ul fa-border exercise-info">
  <li><i class="fa-li fa fa-signal level-a"></i>A-niv&#xE5;</li>
  <li><i class="fa-li fa fa-github"></i><a href="https://github.com/1dv021/exercise-shaver-sharp-html.git" target="_blank">https://github.com/1dv021/exercise-shaver-sharp-html.git</a></li>
</ul>

<blockquote>
<p><i class="fa fa-warning"></i> <strong>VIKTIGT!</strong> Innan du b&#xF6;rjar arbeta med &#xF6;vningsuppgiften &#xE4;r det viktigt att du f&#xF6;ljer guiden <a href="../../guider/att-komma-igang-med-en-ovningsuppgift/README.md">Att komma ig&#xE5;ng med en &#xF6;vningsuppgift</a> f&#xF6;r att l&#xE4;gga till &#xF6;vningsuppgiftens repo till ditt repo f&#xF6;r &#xF6;vningsuppgifter.</p>
</blockquote>
<p>Denna uppgift ska resultera i en applikation som skapar HTML. Det &#xE4;r dock en enklare variant som
bara klarar av att skapa starttag, sluttag och textinneh&#xE5;ll d&#xE4;remellan. Den klarar allts&#xE5;
inte av t.ex. tomma element eller attribut. Tanken &#xE4;r att du i slut&#xE4;ndan ska kunna skicka in
en array med objekt som instruerar applikationen att skapa HTML-kod i form av en textstr&#xE4;ng.
Du beh&#xF6;ver inte ta h&#xE4;nsyn till s&#xE5; kallade &quot;whitespaces&quot;, s&#xE5; som radbrytningar s&#xE5; HTML-str&#xE4;ngen blir
i ett stycke.</p>
<h2 id="funktioner">Funktioner</h2>
<p>Uppgiften &#xE4;r t&#xE4;nkt att l&#xF6;sas via fyra olika funktioner f&#xF6;r att enklare bryta ner problemet.</p>
<h3 id="createbegintag">createBeginTag</h3>
<p>Tar en textstr&#xE4;ng som parameter och returnerar en textstr&#xE4;ng i form av en starttagg.</p>
<pre><code>let html = ShaverSharp.createBeginTag(&quot;h1&quot;); // html contains &quot;&lt;h1&gt;&quot;
</code></pre><h3 id="createendtag">createEndTag</h3>
<p>Tar en textstr&#xE4;ng som parameter och returnerar parametern formaterad som en sluttagg.</p>
<pre><code>let html = ShaverSharp.createEndTag(&quot;h1&quot;); // html contains &quot;&lt;/h1&gt;&quot;
</code></pre><h3 id="createelement">createElement</h3>
<p>Tar tv&#xE5; textstr&#xE4;ngar som parameter och returnerar en textstr&#xE4;ng av ett helt element.
H&#xE4;r b&#xF6;r man anropa de tv&#xE5; tidigare funktionerna f&#xF6;r att skapa slutresultatet</p>
<pre><code>let html = ShaverSharp.createElement(&quot;h1&quot;, &quot;This is a headline&quot;); // html contains &quot;&lt;h1&gt;This is a headline&lt;/h1&gt;&quot;
</code></pre><h3 id="createelements">createElements</h3>
<p>Tar en array med objekt som parameter och returnerar en textstr&#xE4;ng i form av HTML.</p>
<pre><code>let arr = [{element: &apos;h1&apos;, innerHTML: &apos;This is a headline&apos;}, {elment: &apos;p&apos;, innerHTML: &apos;...and this is a paragraph.&apos;}]
let html = ShaverSharp.createElements(arr); // html contains &apos;&lt;h1&gt;This is a headline&lt;/h1&gt;&lt;p&gt;...and this is a paragraph.&lt;/p&gt;&apos;
</code></pre><h2 id="tips"><i class="fa fa-lightbulb-o"></i> Tips</h2>
<p>Genom att k&#xF6;ra testerna som kommer med &#xF6;vningsuppgiften kan du unders&#xF6;ka om koden du skrivit l&#xF6;st uppgiften (i alla fall enligt testerna...).</p>
<p>Funktioner, metoder, etc. som <em>kan</em> komma till anv&#xE4;ndning beroende hur du v&#xE4;ljer att l&#xF6;sa uppgiften.</p>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions" target="_blank">funktioner</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let" target="_blank">let</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof" target="_blank">typeof</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else" target="_blank">if...else</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/return" target="_blank">return</a></li>
<li><a href="https://nodejs.org/api/console.html#console_console_log_data" target="_blank">console.log</a></li>
</ul>
<h2 id="l&#xF6;sningsf&#xF6;rslag"><i class="fa fa-flask"></i> L&#xF6;sningsf&#xF6;rslag</h2>
<ul class="fa-ul fa-border exercise-info">
  <li><i class="fa-li fa fa-github"></i><a href="https://github.com/1dv021/exercise-solution-proposals/tree/master/part-1/shaver-sharp-html" target="_blank">https://github.com/1dv021/exercise-solution-proposals/tree/master/part-1/shaver-sharp-html</a></li>
</ul>
