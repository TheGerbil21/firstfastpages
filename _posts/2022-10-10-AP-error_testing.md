---
keywords: fastai
description: Practice with identifying and correcting code blocks
title: Big Idea 1 'Identifying and Correcting Errors'
layout: default
badges: false
permalink: /collegeboard/error
categories: [jupyter, python, tri1, concept]
nb_path: _notebooks/2022-10-10-AP-error_testing.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-10-10-AP-error_testing.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><a href="https://apclassroom.collegeboard.org/103/home?unit=1">College Board Big Idea 1</a></p>
<h2 id="Identifying-and-Correcting-Errors-(Unit-1.4)">Identifying and Correcting Errors (Unit 1.4)<a class="anchor-link" href="#Identifying-and-Correcting-Errors-(Unit-1.4)"> </a></h2><blockquote><p>Become familiar with types of errors and strategies to fixing them</p>
<ul>
<li>Lightly Review Videos and take notes on topics with Blog</li>
<li>Complete assigned MCQ questions</li>
</ul>
</blockquote>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Here-are-some-code-segments-you-can-practice-fixing:">Here are some code segments you can practice fixing:<a class="anchor-link" href="#Here-are-some-code-segments-you-can-practice-fixing:"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">alphabet</span> <span class="o">=</span> <span class="s2">&quot;abcdefghijklmnopqrstuvwxyz&quot;</span>

<span class="n">alphabetList</span> <span class="o">=</span> <span class="p">[]</span>

<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">alphabet</span><span class="p">:</span>
    <span class="n">alphabetList</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="n">alphabetList</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[&#39;a&#39;, &#39;b&#39;, &#39;c&#39;, &#39;d&#39;, &#39;e&#39;, &#39;f&#39;, &#39;g&#39;, &#39;h&#39;, &#39;i&#39;, &#39;j&#39;, &#39;k&#39;, &#39;l&#39;, &#39;m&#39;, &#39;n&#39;, &#39;o&#39;, &#39;p&#39;, &#39;q&#39;, &#39;r&#39;, &#39;s&#39;, &#39;t&#39;, &#39;u&#39;, &#39;v&#39;, &#39;w&#39;, &#39;x&#39;, &#39;y&#39;, &#39;z&#39;]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>The intended outcome is to determine where the letter is in the alphabet using a while loop</p>
<ul>
<li>What is a good test case to check the current outcome? Why?</li>
<li>Make changes to get the intended outcome.</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">letter</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;What letter would you like to check?&quot;</span><span class="p">)</span>

<span class="n">i</span> <span class="o">=</span> <span class="mi">0</span>

<span class="k">while</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="mi">26</span><span class="p">:</span>
    <span class="k">if</span> <span class="n">alphabetList</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">==</span> <span class="n">letter</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The letter &quot;</span> <span class="o">+</span> <span class="n">letter</span> <span class="o">+</span> <span class="s2">&quot; is the &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; letter in the alphabet&quot;</span><span class="p">)</span>
    <span class="n">i</span> <span class="o">+=</span> <span class="mi">1</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>The letter a is the 0 letter in the alphabet
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>The intended outcome is to determine where the letter is in the alphabet using a for loop</p>
<ul>
<li>What is a good test case to check the current outcome? Why?</li>
<li>Make changes to get the intended outcome.</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">letter</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;What letter would you like to check?&quot;</span><span class="p">)</span>

<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">alphabetList</span><span class="p">:</span>
    <span class="n">count</span> <span class="o">=</span> <span class="mi">1</span>
    <span class="k">if</span> <span class="n">i</span> <span class="o">==</span> <span class="n">letter</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The letter &quot;</span> <span class="o">+</span> <span class="n">letter</span> <span class="o">+</span> <span class="s2">&quot; is the &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">count</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; letter in the alphabet&quot;</span><span class="p">)</span>
    <span class="n">count</span> <span class="o">+=</span> <span class="mi">1</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>The letter a is the 1 letter in the alphabet
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This code outputs the even numbers from 0 - 10 using a while loop.</p>
<ul>
<li>Analyze this code to determine what can be changed to get the outcome to be odd numbers. (Code block below)</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">evens</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">i</span> <span class="o">=</span> <span class="mi">0</span>

<span class="k">while</span> <span class="n">i</span> <span class="o">&lt;=</span> <span class="mi">10</span><span class="p">:</span>
    <span class="n">evens</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
    <span class="n">i</span> <span class="o">+=</span> <span class="mi">2</span>

<span class="nb">print</span><span class="p">(</span><span class="n">evens</span><span class="p">)</span>    
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[0, 2, 4, 6, 8, 10]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This code should output the odd numbers from 0 - 10 using a while loop.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">odds</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">i</span> <span class="o">=</span> <span class="mi">1</span>

<span class="k">while</span> <span class="n">i</span> <span class="o">&lt;=</span> <span class="mi">10</span><span class="p">:</span>
    <span class="n">odds</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
    <span class="n">i</span> <span class="o">+=</span> <span class="mi">2</span>

<span class="nb">print</span><span class="p">(</span><span class="n">odds</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[1, 3, 5, 7, 9]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This code outputs the even numbers from 0 - 10 using a for loop.</p>
<ul>
<li>Analyze this code to determine what can be changed to get the outcome to be odd numbers. (Code block below)</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">numbers</span> <span class="o">=</span> <span class="p">[</span><span class="mi">0</span><span class="p">,</span><span class="mi">1</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">4</span><span class="p">,</span><span class="mi">5</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">7</span><span class="p">,</span><span class="mi">8</span><span class="p">,</span><span class="mi">9</span><span class="p">,</span><span class="mi">10</span><span class="p">]</span>
<span class="n">evens</span> <span class="o">=</span> <span class="p">[]</span>

<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">numbers</span><span class="p">:</span>
    <span class="k">if</span> <span class="p">(</span><span class="n">numbers</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">%</span> <span class="mi">2</span> <span class="o">==</span> <span class="mi">0</span><span class="p">):</span>
        <span class="n">evens</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">numbers</span><span class="p">[</span><span class="n">i</span><span class="p">])</span>

<span class="nb">print</span><span class="p">(</span><span class="n">evens</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[0, 2, 4, 6, 8, 10]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This code should output the odd numbers from 0 - 10 using a for loop.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">numbers</span> <span class="o">=</span> <span class="p">[</span><span class="mi">0</span><span class="p">,</span><span class="mi">1</span><span class="p">,</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">4</span><span class="p">,</span><span class="mi">5</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">7</span><span class="p">,</span><span class="mi">8</span><span class="p">,</span><span class="mi">9</span><span class="p">,</span><span class="mi">10</span><span class="p">]</span>
<span class="n">odds</span> <span class="o">=</span> <span class="p">[]</span>

<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">numbers</span><span class="p">:</span>
    <span class="k">if</span> <span class="p">(</span><span class="n">numbers</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">%</span> <span class="mi">3</span> <span class="o">==</span> <span class="mi">0</span><span class="p">):</span>
        <span class="n">odds</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">numbers</span><span class="p">[</span><span class="n">i</span><span class="p">])</span>

<span class="nb">print</span><span class="p">(</span><span class="n">odds</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[0, 3, 6, 9]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>The intended outcome is printing a number between 1 and 100 once, if it is a multiple of 2 or 5</p>
<ul>
<li>What values are outputted incorrectly. Why?</li>
<li>Make changes to get the intended outcome.</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">numbers</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">newNumbers</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">i</span> <span class="o">=</span> <span class="mi">0</span>


<span class="k">while</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="mi">100</span><span class="p">:</span>
    <span class="n">numbers</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
    <span class="n">i</span> <span class="o">+=</span> <span class="mi">1</span>

<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">numbers</span><span class="p">:</span>
    <span class="k">if</span> <span class="n">numbers</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">%</span> <span class="mi">5</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
        <span class="n">newNumbers</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">numbers</span><span class="p">[</span><span class="n">i</span><span class="p">])</span>
    <span class="k">if</span> <span class="n">numbers</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">%</span> <span class="mi">2</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
        <span class="n">newNumbers</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">numbers</span><span class="p">[</span><span class="n">i</span><span class="p">])</span>

<span class="nb">print</span><span class="p">(</span><span class="n">newNumbers</span><span class="p">)</span> 
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[0, 0, 2, 4, 5, 6, 8, 10, 10, 12, 14, 15, 16, 18, 20, 20, 22, 24, 25, 26, 28, 30, 30, 32, 34, 35, 36, 38, 40, 40, 42, 44, 45, 46, 48, 50, 50, 52, 54, 55, 56, 58, 60, 60, 62, 64, 65, 66, 68, 70, 70, 72, 74, 75, 76, 78, 80, 80, 82, 84, 85, 86, 88, 90, 90, 92, 94, 95, 96, 98]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Challenge">Challenge<a class="anchor-link" href="#Challenge"> </a></h1><p>This code segment is at a very early stage of implementation.</p>
<ul>
<li>What are some ways to (user) error proof this code?</li>
<li>The code should be able to calculate the cost of the meal of the user</li>
</ul>
<p>Hint:</p>
<ul>
<li>write a “single” test describing an expectation of the program of the program</li>
<li>test - input burger, expect output of burger price</li>
<li>run the test, which should fail because the program lacks that feature</li>
<li>write “just enough” code, the simplest possible, to make the test pass</li>
</ul>
<p>Then repeat this process until you get program working like you want it to work.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">menu</span> <span class="o">=</span>  <span class="p">{</span><span class="s2">&quot;burger&quot;</span><span class="p">:</span> <span class="mf">3.99</span><span class="p">,</span>    <span class="c1"># creates the menu, its components, and each component&#39;s price.</span>
         <span class="s2">&quot;fries&quot;</span><span class="p">:</span> <span class="mf">1.99</span><span class="p">,</span>
         <span class="s2">&quot;drink&quot;</span><span class="p">:</span> <span class="mf">0.99</span><span class="p">,</span>
         <span class="s2">&quot;checkout&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">}</span>     <span class="c1"># &#39;checkout&#39; is created in the table in order for it to be an interactive input.</span>
<span class="n">total</span> <span class="o">=</span> <span class="mi">0</span>                   <span class="c1"># creates the variable &#39;total&#39; and sets it to 0.</span>

<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Menu&quot;</span><span class="p">)</span>               <span class="c1"># prints menu&#39;s components.</span>
<span class="k">for</span> <span class="n">k</span><span class="p">,</span><span class="n">v</span> <span class="ow">in</span> <span class="n">menu</span><span class="o">.</span><span class="n">items</span><span class="p">():</span>    <span class="c1"># &#39;k&#39; = item&#39;s name. &#39;v&#39; = item&#39;s price(numeric value).</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">k</span> <span class="o">+</span> <span class="s2">&quot;  $&quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">v</span><span class="p">))</span> <span class="c1">#str changes a numeric value (v) into a character that can be printed.</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Please select an item. Type &#39;checkout&#39; to finish your order.&quot;</span><span class="p">)</span> <span class="c1">#tells users what they can do.</span>

<span class="n">checkout</span> <span class="o">=</span> <span class="mi">0</span>                <span class="c1"># checkout created and set to 0.</span>
<span class="k">while</span> <span class="n">checkout</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>        <span class="c1"># while loop connected to checkout.</span>
    <span class="n">item</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Please select an item from the menu Type &#39;checkout&#39; to finish.&quot;</span><span class="p">)</span> <span class="c1">#tells users what they can do.</span>
    <span class="n">item</span> <span class="o">=</span> <span class="n">item</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span>     <span class="c1">#changes input to lowercase to be user friendly.</span>
    <span class="k">if</span> <span class="n">item</span> <span class="o">==</span> <span class="s2">&quot;burger&quot;</span> <span class="ow">or</span> <span class="n">item</span> <span class="o">==</span> <span class="s2">&quot;fries&quot;</span> <span class="ow">or</span> <span class="n">item</span> <span class="o">==</span> <span class="s2">&quot;drink&quot;</span><span class="p">:</span> <span class="c1">#this if statement allows for muiltple inputs to have the same output.</span>
        <span class="nb">print</span><span class="p">(</span> <span class="n">item</span><span class="p">,</span> <span class="s2">&quot;will be $&quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">menu</span><span class="p">[</span><span class="n">item</span><span class="p">]))</span> <span class="c1">#prints item info.</span>
        <span class="n">total</span> <span class="o">+=</span> <span class="n">menu</span><span class="p">[</span><span class="n">item</span><span class="p">]</span>  <span class="c1"># adds the price of the item to total price.</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="k">if</span> <span class="n">item</span> <span class="o">==</span> <span class="s2">&quot;checkout&quot;</span><span class="p">:</span>
            <span class="n">checkout</span> <span class="o">=</span> <span class="mi">1</span>    <span class="c1">#Changes value of checkout that ends while loop.</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Try again, that item is not on the menu&quot;</span><span class="p">)</span> <span class="c1">#In case user makes a typo or tpyes an unknown item.</span>
<span class="k">else</span><span class="p">:</span>
    <span class="n">myorder</span> <span class="o">=</span> <span class="s2">&quot;Your total is $</span><span class="si">{:.2f}</span><span class="s2">! Enjoy!&quot;</span>                <span class="c1">#source: w3shools.com Python String Formatting</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">myorder</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">total</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Menu
burger  $3.99
fries  $1.99
drink  $0.99
checkout  $0
Please select an item. Type &#39;checkout&#39; to finish your order.
burger will be $3.99
burger will be $3.99
drink will be $0.99
fries will be $1.99
Your total is $10.96! Enjoy!
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 
