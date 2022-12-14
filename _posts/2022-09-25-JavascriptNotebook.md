---
keywords: fastai
description: Experimenting with Javascript
title: Javascript Notebook
toc: true
comments: true
permalink: /notebook/Java
tags: [Week5Hacks,Jupyter,Javascript]
nb_path: _notebooks/2022-09-25-JavascriptNotebook.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-09-25-JavascriptNotebook.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Expirementing-with-JavaScript">Expirementing with JavaScript<a class="anchor-link" href="#Expirementing-with-JavaScript"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-python"><pre><span></span><span class="n">function</span> <span class="nb">sum</span><span class="p">(</span><span class="n">a</span><span class="p">,</span> <span class="n">b</span><span class="p">)</span> <span class="p">{</span>
    <span class="k">return</span> <span class="n">a</span> <span class="o">+</span> <span class="n">b</span><span class="p">;</span>
<span class="p">}</span>

<span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="nb">sum</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="mi">11</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>13
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
<div class=" highlight hl-python"><pre><span></span><span class="n">var</span> <span class="n">x</span><span class="p">;</span>
<span class="n">x</span> <span class="o">=</span> <span class="mi">5</span><span class="p">;</span>

<span class="n">function</span> <span class="n">multiply</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">b</span><span class="p">)</span> <span class="p">{</span>
    <span class="k">return</span> <span class="n">x</span> <span class="o">*</span> <span class="n">b</span><span class="p">;</span>
<span class="p">}</span>

<span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="n">multiply</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="mi">10</span><span class="p">));</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>50
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Making-a-Table-and-experimenting-with-logIt">Making a Table and experimenting with logIt<a class="anchor-link" href="#Making-a-Table-and-experimenting-with-logIt"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-python"><pre><span></span><span class="n">function</span> <span class="n">logItType</span><span class="p">(</span><span class="n">output</span><span class="p">)</span> <span class="p">{</span>
    <span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="n">typeof</span> <span class="n">output</span><span class="p">,</span> <span class="s2">&quot;;&quot;</span><span class="p">,</span> <span class="n">output</span><span class="p">);</span>
<span class="p">}</span>
<span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
<span class="n">logItType</span><span class="p">(</span><span class="s2">&quot;hello&quot;</span><span class="p">);</span> 
<span class="n">logItType</span><span class="p">(</span><span class="mi">2022</span><span class="p">);</span>    
<span class="n">logItType</span><span class="p">([</span><span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">]);</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>
string ; hello
number ; 2022
object ; [ 1, 2, 3 ]
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
<div class=" highlight hl-python"><pre><span></span><span class="n">function</span> <span class="n">Person</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">ghID</span><span class="p">,</span> <span class="n">teamrole</span><span class="p">)</span> <span class="p">{</span>
    <span class="n">this</span><span class="o">.</span><span class="n">name</span> <span class="o">=</span> <span class="n">name</span><span class="p">;</span>
    <span class="n">this</span><span class="o">.</span><span class="n">ghID</span> <span class="o">=</span> <span class="n">ghID</span><span class="p">;</span>
    <span class="n">this</span><span class="o">.</span><span class="n">teamrole</span> <span class="o">=</span> <span class="n">teamrole</span><span class="p">;</span>
    <span class="n">this</span><span class="o">.</span><span class="n">role</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">;</span>
<span class="p">}</span>

<span class="o">//</span> <span class="n">define</span> <span class="n">a</span> <span class="n">setter</span> <span class="k">for</span> <span class="n">role</span> <span class="ow">in</span> <span class="n">Person</span> <span class="n">data</span>
<span class="n">Person</span><span class="o">.</span><span class="n">prototype</span><span class="o">.</span><span class="n">setRole</span> <span class="o">=</span> <span class="n">function</span><span class="p">(</span><span class="n">role</span><span class="p">)</span> <span class="p">{</span>
    <span class="n">this</span><span class="o">.</span><span class="n">role</span> <span class="o">=</span> <span class="n">role</span><span class="p">;</span>
<span class="p">}</span>

<span class="o">//</span> <span class="n">define</span> <span class="n">a</span> <span class="n">JSON</span> <span class="n">conversion</span> <span class="s2">&quot;method&quot;</span> <span class="n">associated</span> <span class="k">with</span> <span class="n">Person</span>
<span class="n">Person</span><span class="o">.</span><span class="n">prototype</span><span class="o">.</span><span class="n">toJSON</span> <span class="o">=</span> <span class="n">function</span><span class="p">()</span> <span class="p">{</span>
    <span class="n">const</span> <span class="n">obj</span> <span class="o">=</span> <span class="p">{</span><span class="n">name</span><span class="p">:</span> <span class="n">this</span><span class="o">.</span><span class="n">name</span><span class="p">,</span> <span class="n">ghID</span><span class="p">:</span> <span class="n">this</span><span class="o">.</span><span class="n">ghID</span><span class="p">,</span> <span class="n">teamrole</span><span class="p">:</span> <span class="n">this</span><span class="o">.</span><span class="n">teamrole</span><span class="p">,</span> <span class="n">role</span><span class="p">:</span> <span class="n">this</span><span class="o">.</span><span class="n">role</span><span class="p">};</span>
    <span class="n">const</span> <span class="n">json</span> <span class="o">=</span> <span class="n">JSON</span><span class="o">.</span><span class="n">stringify</span><span class="p">(</span><span class="n">obj</span><span class="p">);</span>
    <span class="k">return</span> <span class="n">json</span><span class="p">;</span>
<span class="p">}</span>

<span class="o">//</span> <span class="n">make</span> <span class="n">a</span> <span class="n">new</span> <span class="n">Person</span> <span class="ow">and</span> <span class="n">assign</span> <span class="n">to</span> <span class="n">variable</span> <span class="n">teacher</span>
<span class="n">var</span> <span class="n">teacher</span> <span class="o">=</span> <span class="n">new</span> <span class="n">Person</span><span class="p">(</span><span class="s2">&quot;Mr M&quot;</span><span class="p">,</span> <span class="s2">&quot;jm1021&quot;</span><span class="p">,</span> <span class="s2">&quot;Grader&quot;</span><span class="p">);</span>  <span class="o">//</span> <span class="nb">object</span> <span class="nb">type</span> <span class="ow">is</span> <span class="n">easy</span> <span class="n">to</span> <span class="n">work</span> <span class="k">with</span> <span class="ow">in</span> <span class="n">JavaScript</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">teacher</span><span class="p">);</span>  <span class="o">//</span> <span class="n">before</span> <span class="n">role</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">teacher</span><span class="o">.</span><span class="n">toJSON</span><span class="p">());</span>  <span class="o">//</span> <span class="n">ok</span> <span class="n">to</span> <span class="n">do</span> <span class="n">this</span> <span class="n">even</span> <span class="n">though</span> <span class="n">role</span> <span class="ow">is</span> <span class="ow">not</span> <span class="n">yet</span> <span class="n">defined</span>

<span class="o">//</span> <span class="n">output</span> <span class="n">of</span> <span class="n">Object</span> <span class="ow">and</span> <span class="n">JSON</span><span class="o">/</span><span class="n">string</span> <span class="n">associated</span> <span class="k">with</span> <span class="n">Teacher</span>
<span class="n">teacher</span><span class="o">.</span><span class="n">setRole</span><span class="p">(</span><span class="s2">&quot;Teacher&quot;</span><span class="p">);</span>   <span class="o">//</span> <span class="nb">set</span> <span class="n">the</span> <span class="n">role</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">teacher</span><span class="p">);</span> 
<span class="n">logItType</span><span class="p">(</span><span class="n">teacher</span><span class="o">.</span><span class="n">toJSON</span><span class="p">());</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>object ; Person { name: &#39;Mr M&#39;, ghID: &#39;jm1021&#39;, teamrole: &#39;Grader&#39;, role: &#39;&#39; }
string ; {&#34;name&#34;:&#34;Mr M&#34;,&#34;ghID&#34;:&#34;jm1021&#34;,&#34;teamrole&#34;:&#34;Grader&#34;,&#34;role&#34;:&#34;&#34;}
object ; Person {
  name: &#39;Mr M&#39;,
  ghID: &#39;jm1021&#39;,
  teamrole: &#39;Grader&#39;,
  role: &#39;Teacher&#39; }
string ; {&#34;name&#34;:&#34;Mr M&#34;,&#34;ghID&#34;:&#34;jm1021&#34;,&#34;teamrole&#34;:&#34;Grader&#34;,&#34;role&#34;:&#34;Teacher&#34;}
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
<div class=" highlight hl-python"><pre><span></span><span class="n">var</span> <span class="n">students</span> <span class="o">=</span> <span class="p">[</span> 
    <span class="n">new</span> <span class="n">Person</span><span class="p">(</span><span class="s2">&quot;Luka&quot;</span><span class="p">,</span> <span class="s2">&quot;LukaVDB&quot;</span><span class="p">,</span> <span class="s2">&quot;DevOps&quot;</span><span class="p">),</span>
    <span class="n">new</span> <span class="n">Person</span><span class="p">(</span><span class="s2">&quot;Jishnu&quot;</span><span class="p">,</span> <span class="s2">&quot;JishnuS420&quot;</span><span class="p">,</span> <span class="s2">&quot;Backend Developer&quot;</span><span class="p">),</span>
    <span class="n">new</span> <span class="n">Person</span><span class="p">(</span><span class="s2">&quot;Edwin&quot;</span><span class="p">,</span> <span class="s2">&quot;EdwinKuttappi&quot;</span><span class="p">,</span> <span class="s2">&quot;Frontend Developer&quot;</span><span class="p">),</span>
    <span class="n">new</span> <span class="n">Person</span><span class="p">(</span><span class="s2">&quot;Emaad&quot;</span><span class="p">,</span> <span class="s2">&quot;Emaad-Mir&quot;</span><span class="p">,</span> <span class="s2">&quot;Scrum Master&quot;</span><span class="p">),</span>
    
<span class="p">];</span>

<span class="o">//</span> <span class="n">define</span> <span class="n">a</span> <span class="n">classroom</span> <span class="ow">and</span> <span class="n">build</span> <span class="n">Classroom</span> <span class="n">objects</span> <span class="ow">and</span> <span class="n">json</span>
<span class="n">function</span> <span class="n">Classroom</span><span class="p">(</span><span class="n">teacher</span><span class="p">,</span> <span class="n">students</span><span class="p">){</span> <span class="o">//</span> <span class="mi">1</span> <span class="n">teacher</span><span class="p">,</span> <span class="n">many</span> <span class="n">student</span>
    <span class="o">//</span> <span class="n">start</span> <span class="n">Classroom</span> <span class="k">with</span> <span class="n">Teacher</span>
    <span class="n">teacher</span><span class="o">.</span><span class="n">setRole</span><span class="p">(</span><span class="s2">&quot;Teacher&quot;</span><span class="p">);</span>
    <span class="n">this</span><span class="o">.</span><span class="n">teacher</span> <span class="o">=</span> <span class="n">teacher</span><span class="p">;</span>
    <span class="n">this</span><span class="o">.</span><span class="n">classroom</span> <span class="o">=</span> <span class="p">[</span><span class="n">teacher</span><span class="p">];</span>
    <span class="o">//</span> <span class="n">add</span> <span class="n">each</span> <span class="n">Student</span> <span class="n">to</span> <span class="n">Classroom</span>
    <span class="n">this</span><span class="o">.</span><span class="n">students</span> <span class="o">=</span> <span class="n">students</span><span class="p">;</span>
    <span class="n">this</span><span class="o">.</span><span class="n">students</span><span class="o">.</span><span class="n">forEach</span><span class="p">(</span><span class="n">student</span> <span class="o">=&gt;</span> <span class="p">{</span> <span class="n">student</span><span class="o">.</span><span class="n">setRole</span><span class="p">(</span><span class="s2">&quot;Student&quot;</span><span class="p">);</span> <span class="n">this</span><span class="o">.</span><span class="n">classroom</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">student</span><span class="p">);</span> <span class="p">});</span>
    <span class="o">//</span> <span class="n">build</span> <span class="n">json</span><span class="o">/</span><span class="n">string</span> <span class="nb">format</span> <span class="n">of</span> <span class="n">Classroom</span>
    <span class="n">this</span><span class="o">.</span><span class="n">json</span> <span class="o">=</span> <span class="p">[];</span>
    <span class="n">this</span><span class="o">.</span><span class="n">classroom</span><span class="o">.</span><span class="n">forEach</span><span class="p">(</span><span class="n">person</span> <span class="o">=&gt;</span> <span class="n">this</span><span class="o">.</span><span class="n">json</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">person</span><span class="o">.</span><span class="n">toJSON</span><span class="p">()));</span>
<span class="p">}</span>

<span class="o">//</span> <span class="n">make</span> <span class="n">a</span> <span class="n">CompSci</span> <span class="n">classroom</span> <span class="kn">from</span> <span class="nn">formerly</span> <span class="n">defined</span> <span class="n">teacher</span> <span class="ow">and</span> <span class="n">students</span>
<span class="n">csp</span> <span class="o">=</span> <span class="n">new</span> <span class="n">Classroom</span><span class="p">(</span><span class="n">teacher</span><span class="p">,</span> <span class="n">students</span><span class="p">);</span>

<span class="o">//</span> <span class="n">output</span> <span class="n">of</span> <span class="n">Objects</span> <span class="ow">and</span> <span class="n">JSON</span> <span class="ow">in</span> <span class="n">CompSci</span> <span class="n">classroom</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">csp</span><span class="o">.</span><span class="n">classroom</span><span class="p">);</span>  <span class="o">//</span> <span class="n">constructed</span> <span class="n">classroom</span> <span class="nb">object</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">csp</span><span class="o">.</span><span class="n">classroom</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">name</span><span class="p">);</span>  <span class="o">//</span> <span class="n">abstract</span> <span class="mi">1</span><span class="n">st</span> <span class="n">objects</span> <span class="n">name</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">csp</span><span class="o">.</span><span class="n">json</span><span class="p">[</span><span class="mi">0</span><span class="p">]);</span>  <span class="o">//</span> <span class="n">show</span> <span class="n">json</span> <span class="n">conversion</span> <span class="n">of</span> <span class="mi">1</span><span class="n">st</span> <span class="nb">object</span> <span class="n">to</span> <span class="n">string</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">JSON</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">csp</span><span class="o">.</span><span class="n">json</span><span class="p">[</span><span class="mi">0</span><span class="p">]));</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>object ; [ Person {
    name: &#39;Mr M&#39;,
    ghID: &#39;jm1021&#39;,
    teamrole: &#39;Grader&#39;,
    role: &#39;Teacher&#39; },
  Person {
    name: &#39;Luka&#39;,
    ghID: &#39;LukaVDB&#39;,
    teamrole: &#39;DevOps&#39;,
    role: &#39;Student&#39; },
  Person {
    name: &#39;Jishnu&#39;,
    ghID: &#39;JishnuS420&#39;,
    teamrole: &#39;Backend Developer&#39;,
    role: &#39;Student&#39; },
  Person {
    name: &#39;Edwin&#39;,
    ghID: &#39;EdwinKuttappi&#39;,
    teamrole: &#39;Frontend Developer&#39;,
    role: &#39;Student&#39; },
  Person {
    name: &#39;Emaad&#39;,
    ghID: &#39;Emaad-Mir&#39;,
    teamrole: &#39;Scrum Master&#39;,
    role: &#39;Student&#39; } ]
string ; Mr M
string ; {&#34;name&#34;:&#34;Mr M&#34;,&#34;ghID&#34;:&#34;jm1021&#34;,&#34;teamrole&#34;:&#34;Grader&#34;,&#34;role&#34;:&#34;Teacher&#34;}
object ; { name: &#39;Mr M&#39;,
  ghID: &#39;jm1021&#39;,
  teamrole: &#39;Grader&#39;,
  role: &#39;Teacher&#39; }
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
<div class=" highlight hl-python"><pre><span></span><span class="n">Classroom</span><span class="o">.</span><span class="n">prototype</span><span class="o">.</span><span class="n">_toHtml</span> <span class="o">=</span> <span class="n">function</span><span class="p">()</span> <span class="p">{</span>
    <span class="o">//</span> <span class="n">HTML</span> <span class="n">Style</span> <span class="ow">is</span> <span class="n">build</span> <span class="n">using</span> <span class="n">inline</span> <span class="n">structure</span>
    <span class="n">var</span> <span class="n">style</span> <span class="o">=</span> <span class="p">(</span>
      <span class="s2">&quot;display:inline-block;&quot;</span> <span class="o">+</span>
      <span class="s2">&quot;border: 2px solid blue;&quot;</span>
    <span class="p">);</span>
  
    <span class="o">//</span> <span class="n">HTML</span> <span class="n">Body</span> <span class="n">of</span> <span class="n">Table</span> <span class="ow">is</span> <span class="n">build</span> <span class="k">as</span> <span class="n">a</span> <span class="n">series</span> <span class="n">of</span> <span class="n">concatenations</span> <span class="p">(</span><span class="o">+=</span><span class="p">)</span>
    <span class="n">var</span> <span class="n">body</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">;</span>
    <span class="o">//</span> <span class="n">Heading</span> <span class="k">for</span> <span class="n">Array</span> <span class="n">Columns</span>
    <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;tr&gt;&quot;</span><span class="p">;</span>
    <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;th&gt;&quot;</span> <span class="o">+</span> <span class="s2">&quot;Name&quot;</span> <span class="o">+</span> <span class="s2">&quot;&lt;/th&gt;&quot;</span><span class="p">;</span>
    <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;th&gt;&quot;</span> <span class="o">+</span> <span class="s2">&quot;GitHub ID&quot;</span> <span class="o">+</span> <span class="s2">&quot;&lt;/th&gt;&quot;</span><span class="p">;</span>
    <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;th&gt;&quot;</span> <span class="o">+</span> <span class="s2">&quot;Team Role&quot;</span> <span class="o">+</span> <span class="s2">&quot;&lt;/th&gt;&quot;</span><span class="p">;</span>
    <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;th&gt;&quot;</span> <span class="o">+</span> <span class="s2">&quot;Class Role&quot;</span> <span class="o">+</span> <span class="s2">&quot;&lt;/th&gt;&quot;</span><span class="p">;</span>
    <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;/tr&gt;&quot;</span><span class="p">;</span>
    <span class="o">//</span> <span class="n">Data</span> <span class="n">of</span> <span class="n">Array</span><span class="p">,</span> <span class="n">iterate</span> <span class="n">through</span> <span class="n">each</span> <span class="n">row</span> <span class="n">of</span> <span class="n">compsci</span><span class="o">.</span><span class="n">classroom</span> 
    <span class="k">for</span> <span class="p">(</span><span class="n">var</span> <span class="n">row</span> <span class="n">of</span> <span class="n">csp</span><span class="o">.</span><span class="n">classroom</span><span class="p">)</span> <span class="p">{</span>
      <span class="o">//</span> <span class="n">tr</span> <span class="k">for</span> <span class="n">each</span> <span class="n">row</span><span class="p">,</span> <span class="n">a</span> <span class="n">new</span> <span class="n">line</span>
      <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;tr&gt;&quot;</span><span class="p">;</span>
      <span class="o">//</span> <span class="n">td</span> <span class="k">for</span> <span class="n">each</span> <span class="n">column</span> <span class="n">of</span> <span class="n">data</span>
      <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;td&gt;&quot;</span> <span class="o">+</span> <span class="n">row</span><span class="o">.</span><span class="n">name</span> <span class="o">+</span> <span class="s2">&quot;&lt;/td&gt;&quot;</span><span class="p">;</span>
      <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;td&gt;&quot;</span> <span class="o">+</span> <span class="n">row</span><span class="o">.</span><span class="n">ghID</span> <span class="o">+</span> <span class="s2">&quot;&lt;/td&gt;&quot;</span><span class="p">;</span>
      <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;td&gt;&quot;</span> <span class="o">+</span> <span class="n">row</span><span class="o">.</span><span class="n">teamrole</span> <span class="o">+</span> <span class="s2">&quot;&lt;/td&gt;&quot;</span><span class="p">;</span>
      <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;td&gt;&quot;</span> <span class="o">+</span> <span class="n">row</span><span class="o">.</span><span class="n">role</span> <span class="o">+</span> <span class="s2">&quot;&lt;/td&gt;&quot;</span><span class="p">;</span>
      <span class="o">//</span> <span class="n">tr</span> <span class="n">to</span> <span class="n">end</span> <span class="n">line</span>
      <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;tr&gt;&quot;</span><span class="p">;</span>
    <span class="p">}</span>
  
     <span class="o">//</span> <span class="n">Build</span> <span class="ow">and</span> <span class="n">HTML</span> <span class="n">fragment</span> <span class="n">of</span> <span class="n">div</span><span class="p">,</span> <span class="n">table</span><span class="p">,</span> <span class="n">table</span> <span class="n">body</span>
    <span class="k">return</span> <span class="p">(</span>
      <span class="s2">&quot;&lt;div style=&#39;&quot;</span> <span class="o">+</span> <span class="n">style</span> <span class="o">+</span> <span class="s2">&quot;&#39;&gt;&quot;</span> <span class="o">+</span>
        <span class="s2">&quot;&lt;table&gt;&quot;</span> <span class="o">+</span>
          <span class="n">body</span> <span class="o">+</span>
        <span class="s2">&quot;&lt;/table&gt;&quot;</span> <span class="o">+</span>
      <span class="s2">&quot;&lt;/div&gt;&quot;</span>
    <span class="p">);</span>
  
  <span class="p">};</span>
  
  <span class="o">//</span> <span class="n">IJavaScript</span> <span class="n">HTML</span> <span class="n">processor</span> <span class="n">receive</span> <span class="n">parameter</span> <span class="n">of</span> <span class="n">defined</span> <span class="n">HTML</span> <span class="n">fragment</span>
  <span class="err">$$</span><span class="o">.</span><span class="n">html</span><span class="p">(</span><span class="n">csp</span><span class="o">.</span><span class="n">_toHtml</span><span class="p">());</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">


<div class="output_html rendered_html output_subarea output_execute_result">
<div style='display:inline-block;border: 2px solid blue;'><table><tr><th>Name</th><th>GitHub ID</th><th>Team Role</th><th>Class Role</th></tr><tr><td>Mr M</td><td>jm1021</td><td>Grader</td><td>Teacher</td><tr><tr><td>Luka</td><td>LukaVDB</td><td>DevOps</td><td>Student</td><tr><tr><td>Jishnu</td><td>JishnuS420</td><td>Backend Developer</td><td>Student</td><tr><tr><td>Edwin</td><td>EdwinKuttappi</td><td>Frontend Developer</td><td>Student</td><tr><tr><td>Emaad</td><td>Emaad-Mir</td><td>Scrum Master</td><td>Student</td><tr></table></div>
</div>

</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Final-Result">Final Result<a class="anchor-link" href="#Final-Result"> </a></h1>
</div>
</div>
</div>
</div>
 

