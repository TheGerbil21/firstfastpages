---
keywords: fastai
title: My API Experience
toc: true
categories: [TechTalk]
tags: [jupyter, python, tri1, concept]
nb_path: _notebooks/2022-10-07-my-API-experience.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-10-07-my-API-experience.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="The-Weather-API:-By-Zip-Code">The Weather API: By Zip Code<a class="anchor-link" href="#The-Weather-API:-By-Zip-Code"> </a></h2><p>I found an amazing API on the RapidAPI platform that houses data for weather details and conditions by ZIP code. By changing the inputs, I can display ZIP code specific data and change the city information displayed immediately, including up-to-date temperatures and weather description.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">requests</span>

<span class="n">url</span> <span class="o">=</span> <span class="s2">&quot;https://us-weather-by-zip-code.p.rapidapi.com/getweatherzipcode&quot;</span>

<span class="n">querystring</span> <span class="o">=</span> <span class="p">{</span><span class="s2">&quot;zip&quot;</span><span class="p">:</span><span class="s2">&quot;92127&quot;</span><span class="p">}</span>

<span class="n">headers</span> <span class="o">=</span> <span class="p">{</span>
	<span class="s2">&quot;X-RapidAPI-Key&quot;</span><span class="p">:</span> <span class="s2">&quot;24a738dc44msh1340883298de7f6p133977jsnb8399f963780&quot;</span><span class="p">,</span>
	<span class="s2">&quot;X-RapidAPI-Host&quot;</span><span class="p">:</span> <span class="s2">&quot;us-weather-by-zip-code.p.rapidapi.com&quot;</span>
<span class="p">}</span>

<span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">request</span><span class="p">(</span><span class="s2">&quot;GET&quot;</span><span class="p">,</span> <span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">headers</span><span class="p">,</span> <span class="n">params</span><span class="o">=</span><span class="n">querystring</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>{&#34;City&#34;:&#34;San Diego&#34;,&#34;State&#34;:&#34;CA&#34;,&#34;TempF&#34;:&#34;69.0&#34;,&#34;TempC&#34;:&#34;20.6&#34;,&#34;Weather&#34;:&#34;Overcast&#34;,&#34;WindMPH&#34;:&#34;4.6&#34;,&#34;WindDir&#34;:&#34;West&#34;,&#34;RelativeHumidity&#34;:&#34;68&#34;,&#34;VisibilityMiles&#34;:&#34;10.00&#34;,&#34;AirQualityIndex&#34;:&#34;84&#34;,&#34;AirQualityCode&#34;:&#34;2&#34;,&#34;AirQuality&#34;:&#34;Moderate&#34;,&#34;Sunrise&#34;:&#34;06:49&#34;,&#34;Sunset&#34;:&#34;18:20&#34;,&#34;DaylightHours&#34;:&#34;11&#34;,&#34;DaylightMinutes&#34;:&#34;31&#34;,&#34;Code&#34;:&#34;Success&#34;,&#34;Credits&#34;:&#34;499601737&#34;}

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
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">requests</span>

<span class="n">url</span> <span class="o">=</span> <span class="s2">&quot;https://us-weather-by-zip-code.p.rapidapi.com/getweatherzipcode&quot;</span>

<span class="n">querystring</span> <span class="o">=</span> <span class="p">{</span><span class="s2">&quot;zip&quot;</span><span class="p">:</span><span class="s2">&quot;94114&quot;</span><span class="p">}</span>

<span class="n">headers</span> <span class="o">=</span> <span class="p">{</span>
	<span class="s2">&quot;X-RapidAPI-Key&quot;</span><span class="p">:</span> <span class="s2">&quot;24a738dc44msh1340883298de7f6p133977jsnb8399f963780&quot;</span><span class="p">,</span>
	<span class="s2">&quot;X-RapidAPI-Host&quot;</span><span class="p">:</span> <span class="s2">&quot;us-weather-by-zip-code.p.rapidapi.com&quot;</span>
<span class="p">}</span>

<span class="n">response</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">request</span><span class="p">(</span><span class="s2">&quot;GET&quot;</span><span class="p">,</span> <span class="n">url</span><span class="p">,</span> <span class="n">headers</span><span class="o">=</span><span class="n">headers</span><span class="p">,</span> <span class="n">params</span><span class="o">=</span><span class="n">querystring</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="n">response</span><span class="o">.</span><span class="n">text</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>{&#34;City&#34;:&#34;San Francisco&#34;,&#34;State&#34;:&#34;CA&#34;,&#34;TempF&#34;:&#34;57.0&#34;,&#34;TempC&#34;:&#34;13.9&#34;,&#34;Weather&#34;:&#34;Overcast&#34;,&#34;WindMPH&#34;:&#34;0.0&#34;,&#34;WindDir&#34;:&#34;North&#34;,&#34;RelativeHumidity&#34;:&#34;87&#34;,&#34;VisibilityMiles&#34;:&#34;10.00&#34;,&#34;AirQualityIndex&#34;:&#34;84&#34;,&#34;AirQualityCode&#34;:&#34;2&#34;,&#34;AirQuality&#34;:&#34;Moderate&#34;,&#34;Sunrise&#34;:&#34;07:14&#34;,&#34;Sunset&#34;:&#34;18:38&#34;,&#34;DaylightHours&#34;:&#34;11&#34;,&#34;DaylightMinutes&#34;:&#34;24&#34;,&#34;Code&#34;:&#34;Success&#34;,&#34;Credits&#34;:&#34;499601736&#34;}

</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

