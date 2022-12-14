---
keywords: fastai
title: APCSP Final Reflection and Growth
toc: false 
badges: true
comments: true
categories: [jupyter]
nb_path: _notebooks/2022-11-10-Personal-Trimester-Growth.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-11-10-Personal-Trimester-Growth.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Reflection:">Reflection:<a class="anchor-link" href="#Reflection:"> </a></h2><p>I have learned many things over the trimester, and I made a quick list project out of python to show my learning. It's not perfect and has a few errors, but I think it captured the nature of APCSP, which is realizing errors and working to eventually fix and prevent them in the future.</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Code-Segment:">Code Segment:<a class="anchor-link" href="#Code-Segment:"> </a></h2>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">InfoDb</span> <span class="o">=</span> <span class="p">[]</span>

<span class="c1"># Append to List a Dictionary of key/values related to a person and preferences</span>
<span class="n">InfoDb</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;#1&quot;</span><span class="p">:</span> <span class="s2">&quot;Set up a personal blog, updating it regularly with weekly knowledge and work&quot;</span><span class="p">,</span>
    <span class="s2">&quot;#2&quot;</span><span class="p">:</span> <span class="s2">&quot;Explored many APCSP topics including lists, Javascript, HTML, API&#39;s, and Deployment&quot;</span><span class="p">,</span>
    <span class="s2">&quot;#3&quot;</span><span class="p">:</span> <span class="s2">&quot;Deployed Flask Web Servers on official Amazon Web Services&quot;</span><span class="p">,</span>
    <span class="s2">&quot;#4&quot;</span><span class="p">:</span> <span class="s2">&quot;Created API&#39;s to store and display data on servers&quot;</span><span class="p">,</span>
    <span class="s2">&quot;#5&quot;</span><span class="p">:</span> <span class="s2">&quot;Managed both Frontend and Backend Elements to create a fufilling project&quot;</span><span class="p">,</span>
    <span class="s2">&quot;#6&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;Became a better group leader&quot;</span><span class="p">]</span>
<span class="p">})</span>

<span class="c1"># Append to List a 2nd Dictionary of key/values</span>
<span class="n">InfoDb</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;#1&quot;</span><span class="p">:</span> <span class="s2">&quot;Jeffrey Lee (Scrum Master)&quot;</span><span class="p">,</span>
    <span class="s2">&quot;#2&quot;</span><span class="p">:</span> <span class="s2">&quot;Luke Riggins (DevOps)&quot;</span><span class="p">,</span>
    <span class="s2">&quot;#3&quot;</span><span class="p">:</span> <span class="s2">&quot;Ethan Truong (Frontend)&quot;</span><span class="p">,</span>
    <span class="s2">&quot;#4&quot;</span><span class="p">:</span> <span class="s2">&quot;James Armstrong (Backend)&quot;</span><span class="p">,</span>
<span class="p">})</span>

<span class="c1"># Print the data structure</span>
<span class="nb">print</span><span class="p">(</span><span class="n">InfoDb</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[{&#39;#1&#39;: &#39;Set up a personal blog, updating it regularly with weekly knowledge and work&#39;, &#39;#2&#39;: &#34;Explored many APCSP topics including lists, Javascript, HTML, API&#39;s, and Deployment&#34;, &#39;#3&#39;: &#39;Deployed Flask Web Servers on official Amazon Web Services&#39;, &#39;#4&#39;: &#34;Created API&#39;s to store and display data on servers&#34;, &#39;#5&#39;: &#39;Managed both Frontend and Backend Elements to create a fufilling project&#39;, &#39;#6&#39;: [&#39;Became a better group leader&#39;]}, {&#39;#1&#39;: &#39;Jeffrey Lee (Scrum Master)&#39;, &#39;#2&#39;: &#39;Luke Riggins (DevOps)&#39;, &#39;#3&#39;: &#39;Ethan Truong (Frontend)&#39;, &#39;#4&#39;: &#39;James Armstrong (Backend)&#39;}]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">print_data</span><span class="p">(</span><span class="n">d_rec</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Major Areas of Growth This Trimester&quot;</span><span class="p">)</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\t</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;#1&quot;</span><span class="p">,</span> <span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;#1&quot;</span><span class="p">])</span> <span class="c1"># \t is a tab indent</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\t</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;#2&quot;</span><span class="p">,</span> <span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;#2&quot;</span><span class="p">])</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\t</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;#3&quot;</span><span class="p">,</span> <span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;#3&quot;</span><span class="p">])</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\t</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;#4&quot;</span><span class="p">,</span> <span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;#4&quot;</span><span class="p">])</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\t</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;#5&quot;</span><span class="p">,</span> <span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;#5&quot;</span><span class="p">])</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\t</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;#6: &quot;</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>  <span class="c1"># end=&quot;&quot; make sure no return occurs</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">d_rec</span><span class="p">[</span><span class="s2">&quot;#6&quot;</span><span class="p">]))</span>
    <span class="nb">print</span><span class="p">()</span>

<span class="c1"># for loop iterates on length of InfoDb</span>
<span class="k">def</span> <span class="nf">for_loop</span><span class="p">():</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;For loop output</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
    <span class="k">for</span> <span class="n">record</span> <span class="ow">in</span> <span class="n">InfoDb</span><span class="p">:</span>
        <span class="n">print_data</span><span class="p">(</span><span class="n">record</span><span class="p">)</span>

<span class="n">for_loop</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>For loop output

Major Areas of Growth This Trimester
	 #1 Set up a personal blog, updating it regularly with weekly knowledge and work
	 #2 Explored many APCSP topics including lists, Javascript, HTML, API&#39;s, and Deployment
	 #3 Deployed Flask Web Servers on official Amazon Web Services
	 #4 Created API&#39;s to store and display data on servers
	 #5 Managed both Frontend and Backend Elements to create a fufilling project
	 #6: Became a better group leader

Major Areas of Growth This Trimester
	 #1 Jeffrey Lee (Scrum Master)
	 #2 Luke Riggins (DevOps)
	 #3 Ethan Truong (Frontend)
	 #4 James Armstrong (Backend)
</pre>
</div>
</div>

<div class="output_area">

<div class="output_subarea output_text output_error">
<pre>
<span class="ansi-red-fg">---------------------------------------------------------------------------</span>
<span class="ansi-red-fg">KeyError</span>                                  Traceback (most recent call last)
<span class="ansi-green-intense-fg ansi-bold">/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb Cell 5</span> in <span class="ansi-cyan-fg">&lt;cell line: 19&gt;</span><span class="ansi-blue-fg">()</span>
<span class="ansi-green-intense-fg ansi-bold">     &lt;a href=&#39;vscode-notebook-cell://wsl%2Bubuntu/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb#W1sdnNjb2RlLXJlbW90ZQ%3D%3D?line=15&#39;&gt;16&lt;/a&gt;</span>     for record in InfoDb:
<span class="ansi-green-intense-fg ansi-bold">     &lt;a href=&#39;vscode-notebook-cell://wsl%2Bubuntu/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb#W1sdnNjb2RlLXJlbW90ZQ%3D%3D?line=16&#39;&gt;17&lt;/a&gt;</span>         print_data(record)
<span class="ansi-green-fg">---&gt; &lt;a href=&#39;vscode-notebook-cell://wsl%2Bubuntu/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb#W1sdnNjb2RlLXJlbW90ZQ%3D%3D?line=18&#39;&gt;19&lt;/a&gt;</span> for_loop()

<span class="ansi-green-intense-fg ansi-bold">/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb Cell 5</span> in <span class="ansi-cyan-fg">for_loop</span><span class="ansi-blue-fg">()</span>
<span class="ansi-green-intense-fg ansi-bold">     &lt;a href=&#39;vscode-notebook-cell://wsl%2Bubuntu/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb#W1sdnNjb2RlLXJlbW90ZQ%3D%3D?line=14&#39;&gt;15&lt;/a&gt;</span> print(&#34;For loop output\n&#34;)
<span class="ansi-green-intense-fg ansi-bold">     &lt;a href=&#39;vscode-notebook-cell://wsl%2Bubuntu/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb#W1sdnNjb2RlLXJlbW90ZQ%3D%3D?line=15&#39;&gt;16&lt;/a&gt;</span> for record in InfoDb:
<span class="ansi-green-fg">---&gt; &lt;a href=&#39;vscode-notebook-cell://wsl%2Bubuntu/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb#W1sdnNjb2RlLXJlbW90ZQ%3D%3D?line=16&#39;&gt;17&lt;/a&gt;</span>     print_data(record)

<span class="ansi-green-intense-fg ansi-bold">/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb Cell 5</span> in <span class="ansi-cyan-fg">print_data</span><span class="ansi-blue-fg">(d_rec)</span>
<span class="ansi-green-intense-fg ansi-bold">      &lt;a href=&#39;vscode-notebook-cell://wsl%2Bubuntu/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb#W1sdnNjb2RlLXJlbW90ZQ%3D%3D?line=5&#39;&gt;6&lt;/a&gt;</span> print(&#34;\t&#34;, &#34;#3&#34;, d_rec[&#34;#3&#34;])
<span class="ansi-green-intense-fg ansi-bold">      &lt;a href=&#39;vscode-notebook-cell://wsl%2Bubuntu/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb#W1sdnNjb2RlLXJlbW90ZQ%3D%3D?line=6&#39;&gt;7&lt;/a&gt;</span> print(&#34;\t&#34;, &#34;#4&#34;, d_rec[&#34;#4&#34;])
<span class="ansi-green-fg">----&gt; &lt;a href=&#39;vscode-notebook-cell://wsl%2Bubuntu/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb#W1sdnNjb2RlLXJlbW90ZQ%3D%3D?line=7&#39;&gt;8&lt;/a&gt;</span> print(&#34;\t&#34;, &#34;#5&#34;, d_rec[&#34;#5&#34;])
<span class="ansi-green-intense-fg ansi-bold">      &lt;a href=&#39;vscode-notebook-cell://wsl%2Bubuntu/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb#W1sdnNjb2RlLXJlbW90ZQ%3D%3D?line=8&#39;&gt;9&lt;/a&gt;</span> print(&#34;\t&#34;, &#34;#6: &#34;, end=&#34;&#34;)  # end=&#34;&#34; make sure no return occurs
<span class="ansi-green-intense-fg ansi-bold">     &lt;a href=&#39;vscode-notebook-cell://wsl%2Bubuntu/home/jeffrey/vscode/firstfastpages/_notebooks/2022-11-10-Personal-Trimester-Growth.ipynb#W1sdnNjb2RlLXJlbW90ZQ%3D%3D?line=9&#39;&gt;10&lt;/a&gt;</span> print(&#34;, &#34;.join(d_rec[&#34;#6&#34;]))

<span class="ansi-red-fg">KeyError</span>: &#39;#5&#39;</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

