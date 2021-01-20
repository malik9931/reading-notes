### Transforms

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

<p>The actual syntax for the <code>transform</code> property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.</p>

<pre class="highlight css"><code><table class="rouge-table"><tbody><tr><td class="rouge-gutter gl"><pre class="lineno">1
2
3
4
5
6
7</pre></td><td class="rouge-code"><pre><span class="nt">div</span> <span class="p">{</span>
  <span class="nl">-webkit-transform</span><span class="p">:</span> <span class="n">scale</span><span class="p">(</span><span class="m">1.5</span><span class="p">);</span>
     <span class="nl">-moz-transform</span><span class="p">:</span> <span class="n">scale</span><span class="p">(</span><span class="m">1.5</span><span class="p">);</span>
       <span class="nl">-o-transform</span><span class="p">:</span> <span class="n">scale</span><span class="p">(</span><span class="m">1.5</span><span class="p">);</span>
          <span class="nl">transform</span><span class="p">:</span> <span class="n">scale</span><span class="p">(</span><span class="m">1.5</span><span class="p">);</span>
<span class="p">}</span>
</pre></td></tr></tbody></table>
              </code></pre>
              
              
              
              
<p>Notice how the <code>transform</code> property includes multiple vendor prefixes to gain the best support across all browsers. The un-prefixed declaration comes last to overwrite the prefixed versions, should a browser fully support the transform property.</p>



<div class="lesson-title">
<h6>Lesson 8</h6>
<h1>Transitions <abbr title="and">&amp;</abbr> Animations</h1>
</div>


With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

<p>As mentioned, for a <a href="http://www.alistapart.com/articles/understanding-css3-transitions/" rel="nofollow">transition</a> to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the <code>:hover</code>, <code>:focus</code>, <code>:active</code>, and <code>:target</code> pseudo-classes.</p>

<pre><span class="nc">.box</span> <span class="p">{</span>
  <span class="nl">background</span><span class="p">:</span> <span class="m">#2db34a</span><span class="p">;</span>
  <span class="nl">transition-property</span><span class="p">:</span> <span class="n">background</span><span class="p">;</span>
  <span class="nl">transition-duration</span><span class="p">:</span> <span class="m">1s</span><span class="p">;</span>
  <span class="nl">transition-timing-function</span><span class="p">:</span> <span class="n">linear</span><span class="p">;</span>
<span class="p">}</span>
<span class="nc">.box</span><span class="nd">:hover</span> <span class="p">{</span>
  <span class="nl">background</span><span class="p">:</span> <span class="m">#ff7b29</span><span class="p">;</span>
<span class="p">}</span>
</pre>


### Animations
Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

Example:
https://codepen.io/dp_lewis/pen/gCfBv
