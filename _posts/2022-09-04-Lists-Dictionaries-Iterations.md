---
keywords: fastai
description: Code for holding key information using keys and values
title: Lists, Dictionaries, and Iterations 
toc: true
comments: true
image: /images/LDI.png
permalink: /notebook/ldi
tags: [collegeboard]
nb_path: _notebooks/2022-09-04-Lists-Dictionaries-Iterations.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-09-04-Lists-Dictionaries-Iterations.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">random</span>

<span class="c1"># variable of type string</span>
<span class="n">name</span> <span class="o">=</span> <span class="s2">&quot;Jishnu&quot;</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Name:&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="nb">type</span><span class="p">(</span><span class="n">name</span><span class="p">))</span>

<span class="c1"># variable of type integer</span>
<span class="n">age</span> <span class="o">=</span> <span class="mi">16</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Age:&quot;</span><span class="p">,</span> <span class="n">age</span><span class="p">,</span> <span class="nb">type</span><span class="p">(</span><span class="n">age</span><span class="p">))</span>

<span class="c1"># variable of type float</span>
<span class="n">grade</span> <span class="o">=</span> <span class="mi">11</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Grade:&quot;</span><span class="p">,</span> <span class="n">grade</span><span class="p">,</span> <span class="nb">type</span><span class="p">(</span><span class="n">grade</span><span class="p">))</span>

<span class="c1"># another variable of type string</span>
<span class="n">favorite_color</span> <span class="o">=</span> <span class="s2">&quot; Blue&quot;</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Favorite Color:&quot;</span><span class="p">,</span> <span class="n">favorite_color</span><span class="p">,</span> <span class="nb">type</span><span class="p">(</span><span class="n">favorite_color</span><span class="p">))</span>



<span class="nb">print</span><span class="p">()</span>

<span class="c1"># variable of type list (many values in one variable)</span>

<span class="n">langs</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;Python&quot;</span><span class="p">,</span> <span class="s2">&quot;HTML&quot;</span><span class="p">,</span> <span class="s2">&quot;CSS&quot;</span><span class="p">,</span> <span class="s2">&quot;C&quot;</span><span class="p">,</span> <span class="s2">&quot;Java&quot;</span><span class="p">,</span> <span class="s2">&quot;JavaScript&quot;</span><span class="p">,</span> <span class="s2">&quot;C&quot;</span><span class="p">,</span> <span class="s2">&quot;R&quot;</span><span class="p">,</span> <span class="s2">&quot;C++&quot;</span><span class="p">,</span> <span class="s2">&quot;Bash&quot;</span><span class="p">]</span>
<span class="n">random_lang</span> <span class="o">=</span> <span class="n">random</span><span class="o">.</span><span class="n">choice</span><span class="p">(</span><span class="n">langs</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Random Language:&quot;</span><span class="p">,</span> <span class="n">random_lang</span><span class="p">)</span>

<span class="n">dream_cars</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;Toyota Supra&quot;</span><span class="p">,</span> <span class="s2">&quot;McLaren 750&quot;</span><span class="p">,</span> <span class="s2">&quot;Buggati Chiron&quot;</span><span class="p">,</span> <span class="s2">&quot;Tesla Roadster&quot;</span><span class="p">]</span>
<span class="n">random_car</span> <span class="o">=</span> <span class="n">random</span><span class="o">.</span><span class="n">choice</span><span class="p">(</span><span class="n">dream_cars</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Random Dream Car:&quot;</span><span class="p">,</span> <span class="n">random_car</span><span class="p">)</span>

<span class="nb">print</span><span class="p">()</span>

<span class="c1"># variable of type dictionary (a group of keys and values)</span>
<span class="n">person</span> <span class="o">=</span> <span class="p">{</span>
    <span class="s2">&quot;Name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span>
    <span class="s2">&quot;Age&quot;</span><span class="p">:</span> <span class="n">age</span><span class="p">,</span>
    <span class="s2">&quot;Grade&quot;</span><span class="p">:</span> <span class="n">grade</span><span class="p">,</span>
    <span class="s2">&quot;Languages&quot;</span><span class="p">:</span> <span class="n">langs</span><span class="p">,</span>
    <span class="s2">&quot;Favorite Color&quot;</span><span class="p">:</span> <span class="n">favorite_color</span>
<span class="p">}</span>

<span class="c1"># prints what is in the person dictionary without brackets</span>
<span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">k</span><span class="p">)</span> <span class="o">+</span> <span class="s1">&#39;:&#39;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">v</span><span class="p">)</span> <span class="k">for</span> <span class="n">k</span><span class="p">,</span><span class="n">v</span> <span class="ow">in</span> <span class="n">person</span><span class="o">.</span><span class="n">items</span><span class="p">()])</span>


<span class="n">games</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;Valorant&quot;</span><span class="p">,</span> <span class="s2">&quot;Apex Legends&quot;</span><span class="p">,</span> <span class="s2">&quot;League of Legends&quot;</span><span class="p">,</span> <span class="s2">&quot;Fortnite&quot;</span><span class="p">,</span> <span class="s2">&quot;Minecraft&quot;</span><span class="p">,</span> <span class="s2">&quot;Pokemon&quot;</span><span class="p">,</span> <span class="s2">&quot;Zelda:BOTW&quot;</span><span class="p">,</span> <span class="s2">&quot;GTA&quot;</span><span class="p">]</span>
<span class="n">games</span><span class="o">.</span><span class="n">reverse</span><span class="p">()</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;</span><span class="se">\n</span><span class="s1">Reversed List:&#39;</span><span class="p">),</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">games</span><span class="p">))</span>


<span class="n">random</span><span class="o">.</span><span class="n">shuffle</span><span class="p">(</span><span class="n">games</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;</span><span class="se">\n</span><span class="s1">Random Order:&#39;</span><span class="p">),</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">games</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Name: Jishnu &lt;class &#39;str&#39;&gt;
Age: 16 &lt;class &#39;int&#39;&gt;
Grade: 11 &lt;class &#39;int&#39;&gt;
Favorite Color:  Blue &lt;class &#39;str&#39;&gt;

Random Language: R
Random Dream Car: McLaren 750

Name:Jishnu Age:16 Grade:11 Languages:[&#39;Python&#39;, &#39;HTML&#39;, &#39;CSS&#39;, &#39;C&#39;, &#39;Java&#39;, &#39;JavaScript&#39;, &#39;C&#39;, &#39;R&#39;, &#39;C++&#39;, &#39;Bash&#39;] Favorite Color: Blue

Reversed List:
GTA, Zelda:BOTW, Pokemon, Minecraft, Fortnite, League of Legends, Apex Legends, Valorant

Random Order:
League of Legends, GTA, Apex Legends, Valorant, Pokemon, Minecraft, Zelda:BOTW, Fortnite
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
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">People</span> <span class="o">=</span> <span class="p">[]</span>

<span class="c1"># InfoDB is a data structure with expected Keys and Values</span>

<span class="c1"># Append to List a Dictionary of key/values related to a person and hobbies</span>
<span class="n">People</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;FirstName&quot;</span><span class="p">:</span> <span class="s2">&quot;Jishnu&quot;</span><span class="p">,</span>
    <span class="s2">&quot;LastName&quot;</span><span class="p">:</span> <span class="s2">&quot;Singiresu&quot;</span><span class="p">,</span>
    <span class="s2">&quot;DOB&quot;</span><span class="p">:</span> <span class="s2">&quot;April 20&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Email&quot;</span><span class="p">:</span> <span class="s2">&quot;broburn123@gmail.com&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Dream Car&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;McLaren 750&quot;</span><span class="p">],</span>
    <span class="s2">&quot;Hobbies&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;Sleeping&quot;</span><span class="p">,</span> <span class="s2">&quot;Playing Games&quot;</span><span class="p">,</span> <span class="s2">&quot;Hanging Out with Friends&quot;</span><span class="p">]</span>
<span class="p">})</span>

<span class="c1"># Append to List a 2nd Dictionary of key/values</span>
<span class="n">People</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;FirstName&quot;</span><span class="p">:</span> <span class="s2">&quot;Luka&quot;</span><span class="p">,</span>
    <span class="s2">&quot;LastName&quot;</span><span class="p">:</span> <span class="s2">&quot;Van Den Boomen&quot;</span><span class="p">,</span>
    <span class="s2">&quot;DOB&quot;</span><span class="p">:</span> <span class="s2">&quot;September 19&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Email&quot;</span><span class="p">:</span> <span class="s2">&quot;unknowndutch@gmail.com&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Dream Car&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;F1 Racing Car&quot;</span><span class="p">],</span>
    <span class="s2">&quot;Hobbies&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;Biking&quot;</span><span class="p">,</span><span class="s2">&quot;Sleeping&quot;</span><span class="p">,</span> <span class="s2">&quot;Playing Video Games&quot;</span><span class="p">]</span>
<span class="p">})</span>


<span class="c1"># Print the data structure</span>
<span class="nb">print</span><span class="p">(</span><span class="n">People</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[{&#39;FirstName&#39;: &#39;Jishnu&#39;, &#39;LastName&#39;: &#39;Singiresu&#39;, &#39;DOB&#39;: &#39;April 20&#39;, &#39;Email&#39;: &#39;broburn123@gmail.com&#39;, &#39;Dream Car&#39;: [&#39;McLaren 750&#39;], &#39;Hobbies&#39;: [&#39;Sleeping&#39;, &#39;Playing Games&#39;, &#39;Hanging Out with Friends&#39;]}, {&#39;FirstName&#39;: &#39;Luka&#39;, &#39;LastName&#39;: &#39;Van Den Boomen&#39;, &#39;DOB&#39;: &#39;September 19&#39;, &#39;Email&#39;: &#39;unknowndutch@gmail.com&#39;, &#39;Dream Car&#39;: [&#39;F1 Racing Car&#39;], &#39;Hobbies&#39;: [&#39;Biking&#39;, &#39;Sleeping&#39;, &#39;Playing Video Games&#39;]}]
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
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">print_data</span><span class="p">(</span><span class="n">person</span><span class="p">):</span> <span class="c1"># defines the data being printed</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Name:&quot;</span><span class="p">,</span> <span class="n">person</span><span class="p">[</span><span class="s2">&quot;FirstName&quot;</span><span class="p">],</span> <span class="n">person</span><span class="p">[</span><span class="s2">&quot;LastName&quot;</span><span class="p">])</span> <span class="c1"># Tells the computer to print certain things from the dictionary</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Birthday:&quot;</span><span class="p">,</span> <span class="n">person</span><span class="p">[</span><span class="s2">&quot;DOB&quot;</span><span class="p">])</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Email:&quot;</span><span class="p">,</span> <span class="n">person</span><span class="p">[</span><span class="s2">&quot;Email&quot;</span><span class="p">])</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Dream Car:&quot;</span><span class="p">,</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">person</span><span class="p">[</span><span class="s2">&quot;Dream Car&quot;</span><span class="p">]))</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Hobbies:&quot;</span><span class="p">,</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">person</span><span class="p">[</span><span class="s2">&quot;Hobbies&quot;</span><span class="p">]))</span>
    <span class="nb">print</span><span class="p">()</span>

<span class="n">print_data</span><span class="p">(</span><span class="n">People</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span> 
<span class="n">print_data</span><span class="p">(</span><span class="n">People</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Name: Jishnu Singiresu
Birthday: April 20
Email: broburn123@gmail.com
Dream Car: McLaren 750
Hobbies: Sleeping, Playing Games, Hanging Out with Friends

Name: Luka Van Den Boomen
Birthday: September 19
Email: unknowndutch@gmail.com
Dream Car: F1 Racing Car
Hobbies: Biking, Sleeping, Playing Video Games

</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Loops">Loops<a class="anchor-link" href="#Loops"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">for_loop</span><span class="p">():</span>             <span class="c1"># for every person in the InfoDB, print their data until there is nothing else to print</span>
    <span class="k">for</span> <span class="n">person</span> <span class="ow">in</span> <span class="n">People</span><span class="p">:</span>
        <span class="n">print_data</span><span class="p">(</span><span class="n">person</span><span class="p">)</span>

<span class="k">def</span> <span class="nf">for_loop_with_index</span><span class="p">():</span>      <span class="c1"># prints out data depending on the length of the dictionary it comes from</span>
    <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">People</span><span class="p">)):</span>
        <span class="n">print_data</span><span class="p">(</span><span class="n">People</span><span class="p">[</span><span class="n">p</span><span class="p">])</span>

<span class="n">for_loop</span><span class="p">()</span>
<span class="n">for_loop_with_index</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Name: Jishnu Singiresu
Birthday: April 20
Email: broburn123@gmail.com
Dream Car: McLaren 750
Hobbies: Sleeping, Playing Games, Hanging Out with Friends

Name: Luka Van Den Boomen
Birthday: September 19
Email: unknowndutch@gmail.com
Dream Car: F1 Racing Car
Hobbies: Biking, Sleeping, Playing Video Games

Name: Jishnu Singiresu
Birthday: April 20
Email: broburn123@gmail.com
Dream Car: McLaren 750
Hobbies: Sleeping, Playing Games, Hanging Out with Friends

Name: Luka Van Den Boomen
Birthday: September 19
Email: unknowndutch@gmail.com
Dream Car: F1 Racing Car
Hobbies: Biking, Sleeping, Playing Video Games

</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="While-Loops">While Loops<a class="anchor-link" href="#While-Loops"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">while_loop</span><span class="p">():</span>       <span class="c1"># i starts at 0</span>
    <span class="n">i</span> <span class="o">=</span> <span class="mi">0</span>
    <span class="k">while</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="nb">len</span><span class="p">(</span><span class="n">People</span><span class="p">):</span>      <span class="c1"># while i is less than the length of the dictionary (2), keep printing the people&#39;s data</span>
        <span class="n">record</span> <span class="o">=</span> <span class="n">People</span><span class="p">[</span><span class="n">i</span><span class="p">]</span>
        <span class="n">print_data</span><span class="p">(</span><span class="n">record</span><span class="p">)</span>
        <span class="n">i</span> <span class="o">=</span> <span class="n">i</span> <span class="o">+</span> <span class="mi">1</span>
    <span class="k">return</span>

<span class="n">while_loop</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Name: Jishnu Singiresu
Birthday: April 20
Email: broburn123@gmail.com
Dream Car: McLaren 750
Hobbies: Sleeping, Playing Games, Hanging Out with Friends

Name: Luka Van Den Boomen
Birthday: September 19
Email: unknowndutch@gmail.com
Dream Car: F1 Racing Car
Hobbies: Biking, Sleeping, Playing Video Games

</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Reversed-While-Loop">Reversed While Loop<a class="anchor-link" href="#Reversed-While-Loop"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">while_loop_reverse</span><span class="p">():</span>       
    <span class="n">i</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">People</span><span class="p">)</span> <span class="o">-</span> <span class="mi">1</span>
    <span class="k">while</span> <span class="n">i</span> <span class="o">&gt;=</span> <span class="mi">0</span><span class="p">:</span>
        <span class="n">print_data</span><span class="p">(</span><span class="n">People</span><span class="p">[</span><span class="n">i</span><span class="p">])</span>
        <span class="n">i</span> <span class="o">=</span> <span class="n">i</span> <span class="o">-</span> <span class="mi">1</span>

<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;REVERSED WHILE LOOP</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
<span class="n">while_loop_reverse</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>REVERSED WHILE LOOP

Name: Luka Van Den Boomen
Birthday: September 19
Email: unknowndutch@gmail.com
Dream Car: F1 Racing Car
Hobbies: Biking, Sleeping, Playing Video Games

Name: Jishnu Singiresu
Birthday: April 20
Email: broburn123@gmail.com
Dream Car: McLaren 750
Hobbies: Sleeping, Playing Games, Hanging Out with Friends

</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Recursive-Loops">Recursive Loops<a class="anchor-link" href="#Recursive-Loops"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">recursive</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="c1"># the recursive loop will keep calling itself until it is greater than or equal to the length of the dictionary</span>
    <span class="k">if</span> <span class="n">i</span> <span class="o">&gt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">People</span><span class="p">):</span>
        <span class="k">return</span>          <span class="c1"># this is where the code will end</span>

    <span class="n">print_data</span><span class="p">(</span><span class="n">People</span><span class="p">[</span><span class="n">i</span><span class="p">])</span>      <span class="c1"># prints the data and keeps printing until it has reached the length of the dictionary</span>
    <span class="k">return</span> <span class="n">recursive</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1</span><span class="p">)</span>

<span class="n">recursive</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Name: Jishnu Singiresu
Birthday: April 20
Email: broburn123@gmail.com
Dream Car: McLaren 750
Hobbies: Sleeping, Playing Games, Hanging Out with Friends

Name: Luka Van Den Boomen
Birthday: September 19
Email: unknowndutch@gmail.com
Dream Car: F1 Racing Car
Hobbies: Biking, Sleeping, Playing Video Games

</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Quiz-using-Lists">Quiz using Lists<a class="anchor-link" href="#Quiz-using-Lists"> </a></h1>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">getpass</span>

<span class="n">Subjects</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;Math&quot;</span><span class="p">,</span> <span class="s2">&quot;U.S. History&quot;</span><span class="p">,</span> <span class="s2">&quot;Random&quot;</span><span class="p">]</span>

<span class="n">Quiz</span> <span class="o">=</span> <span class="p">[]</span>

<span class="n">Quiz</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;What is 2+2?&quot;</span> <span class="p">:</span> <span class="s2">&quot;4&quot;</span><span class="p">,</span>
    <span class="s2">&quot;What is 20 x 15?&quot;</span> <span class="p">:</span> <span class="s2">&quot;300&quot;</span><span class="p">,</span>
<span class="p">})</span>

<span class="n">Quiz</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;What is the year U.S declared independence&quot;</span> <span class="p">:</span> <span class="s2">&quot;1776&quot;</span><span class="p">,</span>
    <span class="s2">&quot;Who is the current U.S president?&quot;</span> <span class="p">:</span> <span class="s2">&quot;Joe Biden&quot;</span>
<span class="p">})</span>

<span class="n">Quiz</span><span class="o">.</span><span class="n">append</span><span class="p">({</span>
    <span class="s2">&quot;What color is cheese?&quot;</span> <span class="p">:</span> <span class="s2">&quot;Yellow&quot;</span><span class="p">,</span>
<span class="p">})</span>


<span class="k">def</span> <span class="nf">question_with_response</span><span class="p">(</span><span class="n">prompt</span><span class="p">):</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Question &quot;</span> <span class="o">+</span> <span class="s2">&quot;: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span>
    <span class="n">msg</span> <span class="o">=</span> <span class="nb">input</span><span class="p">()</span>
    <span class="k">return</span> <span class="n">msg</span>

<span class="k">def</span> <span class="nf">for_loop_index</span><span class="p">():</span>        
    <span class="n">scores</span> <span class="o">=</span> <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">]</span> 
    <span class="n">s</span> <span class="o">=</span> <span class="mi">0</span>
    <span class="k">for</span> <span class="n">subject</span> <span class="ow">in</span> <span class="n">Quiz</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">Subject: &quot;</span> <span class="o">+</span> <span class="n">Subjects</span><span class="p">[</span><span class="n">s</span><span class="p">])</span>
        <span class="k">for</span> <span class="n">ques</span><span class="p">,</span> <span class="n">ans</span> <span class="ow">in</span> <span class="n">subject</span><span class="o">.</span><span class="n">items</span><span class="p">():</span>
            <span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="n">ques</span><span class="p">)</span>
            <span class="k">if</span> <span class="n">rsp</span> <span class="o">==</span> <span class="n">ans</span><span class="p">:</span>
                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;*Ding, Ding, Ding*, Correct answer! You gain 1 point!&quot;</span><span class="p">)</span>
                    <span class="n">scores</span><span class="p">[</span><span class="n">s</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span> 
            <span class="k">else</span><span class="p">:</span>
                <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;*Buzzer sounds*, Damn nice try, better luck next time! You gain no points.&quot;</span><span class="p">)</span>
        <span class="n">s</span> <span class="o">+=</span> <span class="mi">1</span>
    <span class="nb">print</span><span class="p">()</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Correct answers in &quot;</span> <span class="o">+</span> <span class="n">Subjects</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="s2">&quot;: &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">scores</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span> <span class="o">+</span> <span class="s2">&quot; out of &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">Quiz</span><span class="p">[</span><span class="mi">0</span><span class="p">])))</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Correct answers in &quot;</span> <span class="o">+</span> <span class="n">Subjects</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">+</span> <span class="s2">&quot;: &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">scores</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span> <span class="o">+</span> <span class="s2">&quot; out of &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">Quiz</span><span class="p">[</span><span class="mi">1</span><span class="p">])))</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Correct answers in &quot;</span> <span class="o">+</span> <span class="n">Subjects</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+</span> <span class="s2">&quot;: &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">scores</span><span class="p">[</span><span class="mi">2</span><span class="p">])</span> <span class="o">+</span> <span class="s2">&quot; out of &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">Quiz</span><span class="p">[</span><span class="mi">2</span><span class="p">])))</span>
    <span class="k">return</span>

<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Hello everyone!, &#39;</span> <span class="o">+</span> <span class="n">getpass</span><span class="o">.</span><span class="n">getuser</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot; is our participant for today&#39;s trivia, Ready to test your wits?&quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Spelling counts so make sure you check your spelling and capitalize the first letter!&quot;</span><span class="p">)</span>
<span class="n">for_loop_index</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Hello everyone!, jishnus is our participant for today&#39;s trivia, Ready to test your wits?
Spelling counts so make sure you check your spelling and capitalize the first letter!

Subject: Math
Question : What is 2+2?
*Ding, Ding, Ding*, Correct answer! You gain 1 point!
Question : What is 20 x 15?
*Ding, Ding, Ding*, Correct answer! You gain 1 point!

Subject: U.S. History
Question : What is the year U.S declared independence
*Ding, Ding, Ding*, Correct answer! You gain 1 point!
Question : Who is the current U.S president?
*Buzzer sounds*, Damn nice try, better luck next time! You gain no points.

Subject: Random
Question : What color is cheese?
*Ding, Ding, Ding*, Correct answer! You gain 1 point!

Correct answers in Math: 2 out of 2
Correct answers in U.S. History: 1 out of 2
Correct answers in Random: 1 out of 1
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 
