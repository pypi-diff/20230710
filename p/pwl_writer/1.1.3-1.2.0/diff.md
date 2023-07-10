# Comparing `tmp/pwl_writer-1.1.3.tar.gz` & `tmp/pwl_writer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl_writer-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pwl_writer-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pwl_writer-1.1.3.tar` & `pwl_writer-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1497 2023-06-23 13:23:50.038539 pwl_writer-1.1.3/.gitignore
--rw-r--r--   0        0        0     1111 2023-06-23 12:40:45.054972 pwl_writer-1.1.3/LICENSE
--rw-r--r--   0        0        0     3934 2023-06-24 11:49:16.390169 pwl_writer-1.1.3/README.md
--rw-r--r--   0        0        0   178465 2023-06-29 14:42:19.179958 pwl_writer-1.1.3/docs/pwl_writer.html
--rw-r--r--   0        0        0     7070 2023-06-29 14:42:18.865952 pwl_writer-1.1.3/docs/pycco.css
--rw-r--r--   0        0        0      190 2023-06-29 14:43:14.609223 pwl_writer-1.1.3/pwl_writer/__init__.py
--rw-r--r--   0        0        0    46836 2023-06-29 14:42:12.360007 pwl_writer-1.1.3/pwl_writer/pwl_writer.py
--rw-r--r--   0        0        0      685 2023-06-24 11:51:38.147038 pwl_writer-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 pwl_writer-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-06-23 13:23:50.038539 pwl_writer-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1111 2023-06-23 12:40:45.054972 pwl_writer-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3934 2023-06-24 11:49:16.390169 pwl_writer-1.2.0/README.md
+-rw-r--r--   0        0        0   248814 2023-07-10 05:56:39.004195 pwl_writer-1.2.0/docs/pwl_writer.html
+-rw-r--r--   0        0        0     7070 2023-07-10 05:56:38.674585 pwl_writer-1.2.0/docs/pycco.css
+-rw-r--r--   0        0        0      192 2023-07-10 05:55:22.844829 pwl_writer-1.2.0/pwl_writer/__init__.py
+-rw-r--r--   0        0        0    60896 2023-07-10 05:55:08.781732 pwl_writer-1.2.0/pwl_writer/pwl_writer.py
+-rw-r--r--   0        0        0      693 2023-07-09 11:09:21.454770 pwl_writer-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4150 2023-07-05 18:36:57.000000 pwl_writer-1.2.0/teste.py
+-rw-r--r--   0        0        0     4602 1970-01-01 00:00:00.000000 pwl_writer-1.2.0/PKG-INFO
```

### Comparing `pwl_writer-1.1.3/.gitignore` & `pwl_writer-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.3/LICENSE` & `pwl_writer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.3/README.md` & `pwl_writer-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.3/docs/pwl_writer.html` & `pwl_writer-1.2.0/docs/pwl_writer.html`

 * *Files 18% similar despite different names*

```diff
@@ -32,56 +32,63 @@
 </li>
 </ul>
 <p>Type stubs for older numpy versions for mypy checking can be found <a href="https://github.com/numpy/numpy-stubs">here</a>.</p>
 <hr />
 <h1>Index</h1>
 <ul>
 <li><a href="#package-summary">Package Summary</a></li>
-<li><a href="#precision-related-exception">Precision Related Exception</a></li>
 <li><a href="#pwl-class">PWL Class</a><ul>
 <li>Dunder Methods<ul>
 <li><a href="#initializer">Initializer</a></li>
 <li><a href="#string-representation">String Representation</a></li>
 <li><a href="#length-calculator">Length Calculator</a></li>
-<li><a href="#object-as-a-callable">Object as a Callable</a></li>
+<li><a href="#object-calling">Object Calling</a></li>
+<li><a href="#object-slicing">Object Slicing</a></li>
+<li><a href="#object-iteration">Object Iteration</a></li>
+</ul>
+</li>
+<li>Mathematical Unary Operators<ul>
+<li><a href="#additive-inverse">Additive Inverse</a></li>
+<li><a href="#absolute-value">Absolute Value</a></li>
+</ul>
+</li>
+<li>Mathematical Binary Operators<ul>
+<li><a href="#addition">Addition</a></li>
+<li><a href="#subtraction">Subtraction</a></li>
+<li><a href="#multiplication">Multiplication</a></li>
+<li><a href="#division">Division</a></li>
+<li><a href="#exponentiation">Exponentiation</a></li>
 </ul>
 </li>
 <li>Properties<ul>
 <li><a href="#time-coordinates">Time Coordinates</a></li>
 <li><a href="#dependent-coordinates">Dependent Coordinates</a></li>
 <li><a href="#default-timestep">Default Timestep</a></li>
 <li><a href="#name">Name</a></li>
 <li><a href="#verbose-flag">Verbose Flag</a></li>
 <li><a href="#plot-enable-flag">Plot Enable Flag</a> <em>(optional feature: requires matplotlib)</em></li>
 </ul>
 </li>
-<li>Methods<ul>
+<li>Instance Methods<ul>
+<li><a href="#initial-condition">Initial Condition</a></li>
 <li><a href="#last-value-holder">Last Value Holder</a></li>
 <li><a href="#linear-transition">Linear Transition</a></li>
 <li><a href="#rectangular-pulse">Rectangular Pulse</a></li>
 <li><a href="#sawtooth-pulse">Sawtooth Pulse</a></li>
 <li><a href="#exponential-transition">Exponential Transition</a></li>
 <li><a href="#half-sine-transition">Half Sine Transition</a></li>
 <li><a href="#smoothstep-transition">Smoothstep Transition</a></li>
-<li><a href="#pwl-file-writer">PWL File Writer</a></li>
-<li><a href="#pwl-plotter">PWL Plotter</a> <em>(optional feature: requires matplotlib)</em></li>
-</ul>
-</li>
-<li>Private Methods <em>(minimal documentation)</em><ul>
-<li><a href="#pwl-point-adder">PWL Point Adder</a></li>
-<li><a href="#colinear-points-eliminator">Colinear Points Eliminator</a></li>
-<li><a href="#nested-linear-transition">Nested Linear Transition</a></li>
+<li><a href="#file-writer">File Writer</a></li>
+<li><a href="#object-copy">Object Copy</a></li>
 </ul>
 </li>
+<li>Class Methods<ul>
+<li><a href="#pwl-plotter">PWL Plotter</a> <em>(optional feature: requires matplotlib)</em></li>
 </ul>
 </li>
-<li>Private Functions <em>(minimal documentation)</em><ul>
-<li><a href="#exponential-function-generator">Exponential Function Generator</a></li>
-<li><a href="#sinusoidal-function-generator">Sinusoidal Function Generator</a></li>
-<li><a href="#smoothstep-function-generator">Smoothstep Function Generator</a></li>
 </ul>
 </li>
 </ul>
 <hr />
 <h1>Package Summary</h1>
 <p>This package defines a class <code>PWL</code> to generate objects that represent time dependent signals <code>x(t)</code> that need to be coded in a PWL file. Those objects are built using little components such as rectangular pulses and sawtooth pulses that can be chained together.</p>
 <p>The motivations for this package are the nuisances of writing PWL files by hand. To properly explain this, let&rsquo;s discuss how PWL files work.</p>
@@ -112,259 +119,279 @@
 <p>For each state, various control signals need to be at specific values. We could create a <code>PWL</code> object for each control signal and define 3 functions that apply all the needed values for the control signals for each state. If we nedded the system to be at mode 1 for 3 seconds, idle for 1 second and at mode 2 for 5 seconds, we could write something like the following:</p>
 <pre><code>   mode1_state(3)
    idle_state(1)
    mode2_state(5)
 </code></pre>
     </div>
     <div class='code'>
-      <div class="highlight"><pre><span></span><span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;PrecisionError&#39;</span><span class="p">,</span> <span class="s1">&#39;PWL&#39;</span><span class="p">]</span>
+      <div class="highlight"><pre><span></span><span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;PWL&#39;</span><span class="p">]</span>
 
-<span class="kn">from</span> <span class="nn">warnings</span> <span class="kn">import</span> <span class="n">warn</span>
+<span class="kn">import</span> <span class="nn">warnings</span>
 <span class="kn">from</span> <span class="nn">numbers</span> <span class="kn">import</span> <span class="n">Real</span>
-<span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Callable</span><span class="p">,</span> <span class="n">Dict</span><span class="p">,</span> <span class="n">List</span><span class="p">,</span> <span class="n">Optional</span>
+<span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Callable</span><span class="p">,</span> <span class="n">List</span><span class="p">,</span> <span class="n">Optional</span><span class="p">,</span> <span class="n">TYPE_CHECKING</span><span class="p">,</span> <span class="n">Union</span><span class="p">,</span> <span class="n">Tuple</span><span class="p">,</span> <span class="n">Iterator</span><span class="p">,</span> <span class="n">TypeVar</span><span class="p">,</span> <span class="n">Any</span><span class="p">,</span> <span class="n">cast</span>
+<span class="kn">import</span> <span class="nn">weakref</span>
 <span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
 
+
 <span class="k">try</span><span class="p">:</span>
     <span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>  <span class="c1"># type: ignore</span>
 <span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
     <span class="n">_has_matplotlib</span> <span class="o">=</span> <span class="kc">False</span>
-    <span class="n">warn</span><span class="p">(</span><span class="s2">&quot;Matplotlib package not found. Optional plotting features deactivated.&quot;</span><span class="p">,</span> <span class="ne">ImportWarning</span><span class="p">)</span>
+    <span class="n">warnings</span><span class="o">.</span><span class="n">warn</span><span class="p">(</span><span class="s2">&quot;Matplotlib package not found. Optional plotting features deactivated.&quot;</span><span class="p">,</span> <span class="ne">ImportWarning</span><span class="p">)</span>
 <span class="k">else</span><span class="p">:</span>
-    <span class="n">_has_matplotlib</span> <span class="o">=</span> <span class="kc">True</span></pre></div>
+    <span class="n">_has_matplotlib</span> <span class="o">=</span> <span class="kc">True</span>
+
+<span class="k">if</span> <span class="n">TYPE_CHECKING</span><span class="p">:</span>
+    <span class="n">WeakDict</span> <span class="o">=</span> <span class="n">weakref</span><span class="o">.</span><span class="n">WeakValueDictionary</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="s2">&quot;PWL&quot;</span><span class="p">]</span>
+
+<span class="n">TFun</span> <span class="o">=</span> <span class="n">TypeVar</span><span class="p">(</span><span class="s2">&quot;TFun&quot;</span><span class="p">,</span> <span class="n">bound</span><span class="o">=</span><span class="n">Callable</span><span class="p">[</span><span class="o">...</span><span class="p">,</span> <span class="n">Any</span><span class="p">])</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-1'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-1'>#</a>
       </div>
-      <hr />
+      
     </div>
     <div class='code'>
-      <div class="highlight"><pre></pre></div>
+      <div class="highlight"><pre><span class="k">class</span> <span class="nc">copy_doc</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-2'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-2'>#</a>
       </div>
-      <h2><span id="precision-related-exception" href="precision-related-exception"> Precision Related Exception </span></h2>
+      
     </div>
     <div class='code'>
-      <div class="highlight"><pre></pre></div>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">copy_func</span><span class="p">:</span> <span class="n">TFun</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="bp">self</span><span class="o">.</span><span class="n">copy_func</span> <span class="o">=</span> <span class="n">copy_func</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-3'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-3'>#</a>
       </div>
-      <p><strong><code>PrecisionError</code> exception class</strong></p>
+      
     </div>
     <div class='code'>
-      <div class="highlight"><pre><span class="k">class</span> <span class="nc">PrecisionError</span><span class="p">(</span><span class="ne">Exception</span><span class="p">):</span></pre></div>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__call__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">func</span><span class="p">:</span> <span class="n">TFun</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">TFun</span><span class="p">:</span>
+        <span class="n">func</span><span class="o">.</span><span class="vm">__doc__</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">copy_func</span><span class="o">.</span><span class="vm">__doc__</span>
+        <span class="k">return</span> <span class="n">func</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-4'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-4'>#</a>
       </div>
-      <p>This class defines an exception meant to be raised when any type of rounding or loss of precision that causes the time coordinates of a PWL object to not be strictly increasing.</p>
+      
     </div>
     <div class='code'>
-      <div class="highlight"><pre></pre></div>
+      <div class="highlight"><pre><span class="k">class</span> <span class="nc">PrecisionError</span><span class="p">(</span><span class="ne">Exception</span><span class="p">):</span>
+    <span class="k">pass</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-5'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-5'>#</a>
       </div>
-      <hr />
+      
     </div>
     <div class='code'>
-      <div class="highlight"><pre></pre></div>
+      <div class="highlight"><pre><span class="k">class</span> <span class="nc">InitialConditionError</span><span class="p">(</span><span class="ne">Exception</span><span class="p">):</span>
+    <span class="k">pass</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-6'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-6'>#</a>
       </div>
-      <h2><span id="pwl-class" href="pwl-class"> PWL Class </span></h2>
+      <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-7'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-7'>#</a>
       </div>
-      <p><strong><code>PWL</code> class</strong></p>
+      <h2><span id="pwl-class" href="pwl-class"> PWL Class </span></h2>
     </div>
     <div class='code'>
-      <div class="highlight"><pre><span class="k">class</span> <span class="nc">PWL</span><span class="p">():</span></pre></div>
+      <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-8'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-8'>#</a>
       </div>
-      <p>This class defines an object that represnts a time dependent signal <code>x(t)</code>. Those objects can operated on by methods to build, event by event, the desired signal as described on the package introduction.</p>
+      <p><strong><code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="n">__dict_of_objects</span><span class="p">:</span> <span class="n">Dict</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="s1">&#39;PWL&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="p">{}</span></pre></div>
+      <div class="highlight"><pre><span class="k">class</span> <span class="nc">PWL</span><span class="p">():</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-9'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-9'>#</a>
       </div>
-      <hr />
+      <p>This class defines an object that represnts a time dependent signal <code>x(t)</code>. Those objects can operated on by methods to build, event by event, the desired signal as described on the package introduction.</p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre></pre></div>
+      <div class="highlight"><pre>    <span class="n">__dict_of_objects</span> <span class="o">=</span> <span class="n">weakref</span><span class="o">.</span><span class="n">WeakValueDictionary</span><span class="p">()</span>  <span class="c1"># type: WeakDict</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-10'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-10'>#</a>
       </div>
-      <h2><span id="initializer" href="initializer"> Initializer </span></h2>
+      <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-11'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-11'>#</a>
       </div>
-      <p><strong>Dunder method <code>__init__</code> of <code>PWL</code> class</strong></p>
+      <h2><span id="initializer" href="initializer"> Initializer </span></h2>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">verbose</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
+      <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-12'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-12'>#</a>
       </div>
+      <p><strong><code>__init__</code> dunder method of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">verbose</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-13'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-13'>#</a>
+      </div>
       <h3>Summary</h3>
 <p>Initializer for the <code>PWL</code> class.</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>t_step</code> (<code>float</code>) : Default timestep for all operations. Should be strictly positive.</li>
 <li><code>name</code> (<code>str</code>, optional) : Name of the <code>PWL</code> object used for verbose output printing. Should not be empty. If not set, automatically generates a name based on already taken names.</li>
 <li><code>verbose</code> (<code>bool</code>, optional) : Flag indicating if verbose output should be printed. If not set, defaults to <code>False</code>.</li>
 </ul>
 <h3>Raises</h3>
 <ul>
 <li><code>TypeError</code> : Raised if either <code>t_step</code> is not a real number, <code>name</code> is not a string or <code>verbose</code> is not a boolean.</li>
-<li><code>ValueError</code> : Raised if <code>t_step</code> is not strictly positive or <code>name</code> is empty.</li>
+<li><code>ValueError</code> : Raised if <code>t_step</code> is not strictly positive or <code>name</code> is either empty or already taken.</li>
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="n">name</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">i</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span>
-            <span class="k">while</span> <span class="sa">f</span><span class="s2">&quot;pwl_</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">&quot;</span> <span class="ow">in</span> <span class="n">PWL</span><span class="o">.</span><span class="n">__dict_of_objects</span><span class="p">:</span>
+            <span class="k">while</span> <span class="sa">f</span><span class="s2">&quot;pwl_</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">&quot;</span> <span class="ow">in</span> <span class="n">PWL</span><span class="o">.</span><span class="n">__dict_of_objects</span><span class="o">.</span><span class="n">keys</span><span class="p">():</span>
                 <span class="n">i</span> <span class="o">+=</span> <span class="mi">1</span>
             <span class="n">name</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;pwl_</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">&quot;</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">t_step</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="nb">str</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;name&#39; should either be a string but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;name&#39; should either be a string but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">name</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">verbose</span><span class="p">,</span> <span class="nb">bool</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;verbose&#39; should be a boolean but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">verbose</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;verbose&#39; should be a boolean but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">verbose</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">t_step</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="n">name</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;Argument &#39;name&#39; should not be empty.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;Argument &#39;name&#39; should not be empty&quot;</span><span class="p">)</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">:</span> <span class="n">List</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">:</span> <span class="n">List</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_t_step</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">t_step</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="n">name</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="n">verbose</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_plot_flag</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
 
-        <span class="k">if</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">PWL</span><span class="o">.</span> <span class="n">__dict_of_objects</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Name &#39;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&#39; already in use.&quot;</span><span class="p">)</span>
+        <span class="k">if</span> <span class="n">name</span> <span class="ow">in</span> <span class="n">PWL</span><span class="o">.</span><span class="n">__dict_of_objects</span><span class="o">.</span><span class="n">keys</span><span class="p">():</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Name &#39;</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&#39; already in use&quot;</span><span class="p">)</span>
 
-        <span class="n">PWL</span><span class="o">.</span> <span class="n">__dict_of_objects</span><span class="p">[</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span></pre></div>
+        <span class="n">PWL</span><span class="o">.</span><span class="n">__dict_of_objects</span><span class="p">[</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-13'>
+  <div class='section' id='section-14'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-13'>#</a>
+        <a class='octothorpe' href='#section-14'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-14'>
+  <div class='section' id='section-15'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-14'>#</a>
+        <a class='octothorpe' href='#section-15'>#</a>
       </div>
       <h2><span id="string-representation" href="string-representation"> String Representation </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-15'>
+  <div class='section' id='section-16'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-15'>#</a>
+        <a class='octothorpe' href='#section-16'>#</a>
       </div>
-      <p><strong>Dunder method <code>__str__</code> of <code>PWL</code> class</strong></p>
+      <p><strong><code>__str__</code> dunder method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__str__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-16'>
+  <div class='section' id='section-17'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-16'>#</a>
+        <a class='octothorpe' href='#section-17'>#</a>
       </div>
       <h3>Summary</h3>
 <p>String representation of <code>PWL</code> instances in the form <code>[name]: PWL object with [# of points] and duration of [total time duration] seconds</code>.</p>
 <h3>Returns</h3>
 <ul>
 <li><code>str</code></li>
 </ul>
@@ -372,107 +399,107 @@
     <div class='code'>
       <div class="highlight"><pre>        <span class="n">duration</span> <span class="o">=</span> <span class="mi">0</span> <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span> <span class="k">else</span> <span class="nb">max</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span>
 
         <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">: PWL object with </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span><span class="si">}</span><span class="s2"> points and duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> seconds&quot;</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-17'>
+  <div class='section' id='section-18'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-17'>#</a>
+        <a class='octothorpe' href='#section-18'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-18'>
+  <div class='section' id='section-19'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-18'>#</a>
+        <a class='octothorpe' href='#section-19'>#</a>
       </div>
       <h2><span id="length-calculator" href="length-calculator"> Length Calculator </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-19'>
+  <div class='section' id='section-20'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-19'>#</a>
+        <a class='octothorpe' href='#section-20'>#</a>
       </div>
-      <p><strong>Dunder method <code>__len__</code> of <code>PWL</code> class</strong></p>
+      <p><strong><code>__len__</code> dunder method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__len__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-20'>
+  <div class='section' id='section-21'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-20'>#</a>
+        <a class='octothorpe' href='#section-21'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Length of <code>PWL</code> instances defined as the number of <code>(t, x)</code> points they contain.</p>
 <h3>Returns</h3>
 <ul>
 <li><code>int</code></li>
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">return</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-21'>
+  <div class='section' id='section-22'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-21'>#</a>
+        <a class='octothorpe' href='#section-22'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-22'>
+  <div class='section' id='section-23'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-22'>#</a>
+        <a class='octothorpe' href='#section-23'>#</a>
       </div>
-      <h2><span id="object-as-a-callable" href="object-as-a-callable"> Object as a Callable </span></h2>
+      <h2><span id="object-calling" href="object-calling"> Object Calling </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-23'>
+  <div class='section' id='section-24'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-23'>#</a>
+        <a class='octothorpe' href='#section-24'>#</a>
       </div>
-      <p><strong>Dunder method <code>__call__</code> of <code>PWL</code> class</strong></p>
+      <p><strong><code>__call__</code> dunder method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__call__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-24'>
+  <div class='section' id='section-25'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-24'>#</a>
+        <a class='octothorpe' href='#section-25'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Call <code>PWL</code> object as a function by linearly interpolating between it&rsquo;s time and dependent coordinates.</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>t</code> (<code>float</code>) : Time instant to evaluate the object at. If negative, returns zero. If bigger than the duration of the object, returns the object&rsquo;s last dependent coordinate.</li>
 </ul>
@@ -483,181 +510,991 @@
 <h3>Raises</h3>
 <ul>
 <li><code>TypeError</code> : Raised if <code>t</code> is not a real number.</li>
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
 
         <span class="n">t_list</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span>
         <span class="n">x_list</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span>
 
         <span class="k">return</span> <span class="n">np</span><span class="o">.</span><span class="n">interp</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="n">t</span><span class="p">,</span> <span class="n">xp</span><span class="o">=</span><span class="n">t_list</span><span class="p">,</span> <span class="n">fp</span><span class="o">=</span><span class="n">x_list</span><span class="p">,</span> <span class="n">left</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-25'>
+  <div class='section' id='section-26'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-25'>#</a>
+        <a class='octothorpe' href='#section-26'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-26'>
+  <div class='section' id='section-27'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-26'>#</a>
+        <a class='octothorpe' href='#section-27'>#</a>
+      </div>
+      <h2><span id="object-slicing" href="object-slicing"> Object Slicing </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-28'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-28'>#</a>
+      </div>
+      <p><strong><code>__getitem__</code> dunder method of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__getitem__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">index</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="nb">int</span><span class="p">,</span> <span class="nb">slice</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Union</span><span class="p">[</span><span class="n">Tuple</span><span class="p">[</span><span class="nb">float</span><span class="p">,</span> <span class="nb">float</span><span class="p">],</span> <span class="n">List</span><span class="p">[</span><span class="n">Tuple</span><span class="p">[</span><span class="nb">float</span><span class="p">,</span> <span class="nb">float</span><span class="p">]]]:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-29'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-29'>#</a>
+      </div>
+      <h3>Summary</h3>
+<p>Slice <code>PWL</code> objects.</p>
+<h3>Arguments</h3>
+<ul>
+<li><code>index</code> (<code>int</code> or <code>slice</code>) : Index for list of <code>(t, x)</code> points.</li>
+</ul>
+<h3>Returns</h3>
+<ul>
+<li><code>Tuple[float, float]</code> : Returned if single index is passed.</li>
+<li><code>List[Tuple[float, float]]</code> : Rerturned if multiple indices are passed.</li>
+</ul>
+<h3>Raises</h3>
+<ul>
+<li><code>TypeError</code> : Raised if <code>index</code> is not an integer or slice.</li>
+<li><code>IndexError</code> : Raised if <code>index</code> is out of bounds.</li>
+</ul>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">index</span><span class="p">,</span> <span class="p">(</span><span class="nb">int</span><span class="p">,</span> <span class="nb">slice</span><span class="p">)):</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;PWL indices must be integers or slices, not </span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">index</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+
+        <span class="n">coordinates_pair</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="nb">zip</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">t_list</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">x_list</span><span class="p">))</span>
+
+        <span class="k">return</span> <span class="n">coordinates_pair</span><span class="p">[</span><span class="n">index</span><span class="p">]</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-30'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-30'>#</a>
+      </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-31'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-31'>#</a>
+      </div>
+      <h2><span id="object-iteration" href="object-iteration"> Object Iteration </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-32'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-32'>#</a>
+      </div>
+      <p><strong><code>__iter__</code> dunder method of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__iter__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Iterator</span><span class="p">[</span><span class="n">Tuple</span><span class="p">[</span><span class="nb">float</span><span class="p">,</span> <span class="nb">float</span><span class="p">]]:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-33'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-33'>#</a>
+      </div>
+      <h3>Summary</h3>
+<p>Creates a generator object that yields all the <code>(t, x)</code> points as tuples.</p>
+<h3>Yields</h3>
+<ul>
+<li><code>Tuple[float, float]</code></li>
+</ul>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>        <span class="k">yield from</span> <span class="nb">list</span><span class="p">(</span><span class="nb">zip</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">t_list</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">x_list</span><span class="p">))</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-34'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-34'>#</a>
+      </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-35'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-35'>#</a>
+      </div>
+      <h2><span id="additive-inverse" href="additive-inverse"> Additive Inverse </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-36'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-36'>#</a>
+      </div>
+      <p><strong><code>__neg__</code> dunder method of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__neg__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-37'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-37'>#</a>
+      </div>
+      <h3>Summary</h3>
+<p>Implements point-wise additive inversion (multiplying by -1).</p>
+<p>The new <code>PWL</code> objects created has <code>t_step</code> equal to the operand&rsquo;s <code>t_step</code>.</p>
+<h3>Arguments</h3>
+<ul>
+<li>Operand (<code>PWL</code> or <code>float</code>) : Thing being additivly inverted.</li>
+</ul>
+<h3>Returns</h3>
+<ul>
+<li><code>PWL</code> : The additive inverse of the operand.</li>
+</ul>
+<h3>See Also</h3>
+<ul>
+<li><a href="#multiplication">Multiplication</a></li>
+</ul>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>        <span class="k">return</span> <span class="o">-</span><span class="mi">1</span><span class="o">*</span><span class="bp">self</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-38'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-38'>#</a>
+      </div>
+      
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__pos__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span>
+        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">copy</span><span class="p">()</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-39'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-39'>#</a>
+      </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-40'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-40'>#</a>
+      </div>
+      <h2><span id="absolute-value" href="absolute-value"> Absolute Value </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-41'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-41'>#</a>
+      </div>
+      <p><strong><code>__abs__</code> dunder method of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__abs__</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-42'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-42'>#</a>
+      </div>
+      <h3>Summary</h3>
+<p>Implements point-wise absolute value operation.</p>
+<p>The new <code>PWL</code> objects created has <code>t_step</code> equal to the operand&rsquo;s <code>t_step</code>.</p>
+<h3>Arguments</h3>
+<ul>
+<li>Operand (<code>PWL</code> or <code>float</code>) : Thing whose absolute value is being taken.</li>
+</ul>
+<h3>Returns</h3>
+<ul>
+<li><code>PWL</code> : The absolute value of the operand.</li>
+</ul>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>        <span class="n">new_pwl</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="n">t_step</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">t_step</span><span class="p">)</span>
+
+        <span class="k">for</span> <span class="n">t</span><span class="p">,</span> <span class="n">x</span> <span class="ow">in</span> <span class="bp">self</span><span class="p">:</span>
+            <span class="n">new_x</span> <span class="o">=</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">np</span><span class="o">.</span><span class="n">absolute</span><span class="p">(</span><span class="n">x</span><span class="p">))</span>
+            <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">new_x</span><span class="p">)</span>
+
+        <span class="k">return</span> <span class="n">new_pwl</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-43'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-43'>#</a>
+      </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-44'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-44'>#</a>
+      </div>
+      <h2><span id="addition" href="addition"> Addition </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-45'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-45'>#</a>
+      </div>
+      <p><strong><code>__add__</code> and <code>__radd__</code>  dunder methods of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__add__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="s2">&quot;PWL&quot;</span><span class="p">,</span> <span class="nb">float</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-46'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-46'>#</a>
+      </div>
+      <h3>Summary</h3>
+<p>Implements point-wise addition of <code>PWL</code> objects with real numbers and other <code>PWL</code> objects.</p>
+<p>The new <code>PWL</code> objects created has <code>t_step</code> equal to the lower <code>t_step</code> between the operands.</p>
+<p>If one operand is longer than the other, extends the shorter one by holding it&rsquo;s last value.</p>
+<h3>Arguments</h3>
+<ul>
+<li>Addends (<code>PWL</code> or <code>float</code>) : Things being added together.</li>
+</ul>
+<h3>Returns</h3>
+<ul>
+<li><code>PWL</code> : The sum of the addends.</li>
+</ul>
+<h3>Raises</h3>
+<ul>
+<li><code>TypeError</code> : Raised if operation is not implemented between the operands.</li>
+</ul>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="p">(</span><span class="n">Real</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)):</span>
+            <span class="k">return</span> <span class="bp">NotImplemented</span>
+
+        <span class="n">t_step</span> <span class="o">=</span> <span class="nb">min</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">t_step</span><span class="p">,</span> <span class="n">other</span><span class="o">.</span><span class="n">t_step</span><span class="p">)</span> <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">t_step</span>
+        <span class="n">new_pwl</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="n">t_step</span><span class="o">=</span><span class="n">t_step</span><span class="p">)</span>
+
+        <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
+            <span class="n">other_copy</span> <span class="o">=</span> <span class="nb">float</span><span class="p">(</span><span class="n">other</span><span class="p">)</span>
+            <span class="n">other</span> <span class="o">=</span> <span class="k">lambda</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">:</span> <span class="n">other_copy</span>
+
+        <span class="n">unsorted_t_set</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">t_list</span> <span class="o">+</span> <span class="n">other</span><span class="o">.</span><span class="n">t_list</span><span class="p">)</span>
+        <span class="n">t_list</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="n">unsorted_t_set</span><span class="p">))</span>
+        <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">t_list</span><span class="p">:</span>
+            <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="bp">self</span><span class="p">(</span><span class="n">t</span><span class="p">)</span> <span class="o">+</span> <span class="n">other</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
+
+        <span class="k">return</span> <span class="n">new_pwl</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-47'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-47'>#</a>
+      </div>
+      
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="nd">@copy_doc</span><span class="p">(</span><span class="fm">__add__</span><span class="p">)</span>
+    <span class="k">def</span> <span class="fm">__radd__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span>
+        <span class="k">return</span> <span class="bp">self</span> <span class="o">+</span> <span class="n">other</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-48'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-48'>#</a>
+      </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-49'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-49'>#</a>
+      </div>
+      <h2><span id="subtraction" href="subtraction"> Subtraction </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-50'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-50'>#</a>
+      </div>
+      <p><strong><code>__sub__</code> and <code>__rsub__</code>  dunder methods of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__sub__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="s2">&quot;PWL&quot;</span><span class="p">,</span> <span class="nb">float</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-51'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-51'>#</a>
+      </div>
+      <h3>Summary</h3>
+<p>Implements point-wise subtraction of <code>PWL</code> objects with real numbers and other <code>PWL</code> objects.</p>
+<p>The new <code>PWL</code> objects created has <code>t_step</code> equal to the lower <code>t_step</code> between the operands.</p>
+<p>If one operand is longer than the other, extends the shorter one by holding it&rsquo;s last value.</p>
+<h3>Arguments</h3>
+<ul>
+<li>Minuend (<code>PWL</code> or <code>float</code>) : Thing from which we subtract the subtrahend.</li>
+<li>Subtrahend (<code>PWL</code> or <code>float</code>) : Thing being subtracted from the minuend.</li>
+</ul>
+<h3>Returns</h3>
+<ul>
+<li><code>PWL</code> : The difference of the minuend an subtrahend.</li>
+</ul>
+<h3>Raises</h3>
+<ul>
+<li><code>TypeError</code> : Raised if operation is not implemented between the operands.</li>
+</ul>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="p">(</span><span class="n">Real</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)):</span>
+            <span class="k">return</span> <span class="bp">NotImplemented</span>
+
+        <span class="n">t_step</span> <span class="o">=</span> <span class="nb">min</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">t_step</span><span class="p">,</span> <span class="n">other</span><span class="o">.</span><span class="n">t_step</span><span class="p">)</span> <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">t_step</span>
+        <span class="n">new_pwl</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="n">t_step</span><span class="o">=</span><span class="n">t_step</span><span class="p">)</span>
+
+        <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
+            <span class="n">other_copy</span> <span class="o">=</span> <span class="nb">float</span><span class="p">(</span><span class="n">other</span><span class="p">)</span>
+            <span class="n">other</span> <span class="o">=</span> <span class="k">lambda</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">:</span> <span class="n">other_copy</span>
+
+        <span class="n">unsorted_t_set</span> <span class="o">=</span> <span class="nb">set</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">t_list</span> <span class="o">+</span> <span class="n">other</span><span class="o">.</span><span class="n">t_list</span><span class="p">)</span>
+        <span class="n">t_list</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="n">unsorted_t_set</span><span class="p">))</span>
+        <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">t_list</span><span class="p">:</span>
+            <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="bp">self</span><span class="p">(</span><span class="n">t</span><span class="p">)</span> <span class="o">-</span> <span class="n">other</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
+
+        <span class="k">return</span> <span class="n">new_pwl</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-52'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-52'>#</a>
+      </div>
+      
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="nd">@copy_doc</span><span class="p">(</span><span class="fm">__sub__</span><span class="p">)</span>
+    <span class="k">def</span> <span class="fm">__rsub__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span>
+        <span class="n">t_step</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">t_step</span>
+        <span class="n">new_pwl</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="n">t_step</span><span class="o">=</span><span class="n">t_step</span><span class="p">)</span>
+
+        <span class="k">for</span> <span class="n">t</span><span class="p">,</span> <span class="n">x</span> <span class="ow">in</span> <span class="bp">self</span><span class="p">:</span>
+            <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">other</span><span class="o">-</span><span class="n">x</span><span class="p">)</span>
+
+        <span class="k">return</span> <span class="n">new_pwl</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-53'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-53'>#</a>
+      </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-54'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-54'>#</a>
+      </div>
+      <h2><span id="multiplication" href="multiplication"> Multiplication </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-55'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-55'>#</a>
+      </div>
+      <p><strong><code>__mul__</code> and <code>__rmul__</code>  dunder methods of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__mul__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="s2">&quot;PWL&quot;</span><span class="p">,</span> <span class="nb">float</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-56'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-56'>#</a>
+      </div>
+      <h3>Summary</h3>
+<p>Implements point-wise multiplication of <code>PWL</code> objects with real numbers and other <code>PWL</code> objects.</p>
+<p>The new <code>PWL</code> objects created has <code>t_step</code> equal to the lower <code>t_step</code> between the operands.</p>
+<p>If one operand is longer than the other, extends the shorter one by holding it&rsquo;s last value.</p>
+<h3>Arguments</h3>
+<ul>
+<li>Factors (<code>PWL</code> or <code>float</code>) : Things being multiplied together.</li>
+</ul>
+<h3>Returns</h3>
+<ul>
+<li><code>PWL</code> : The product of the factors.</li>
+</ul>
+<h3>Raises</h3>
+<ul>
+<li><code>TypeError</code> : Raised if operation is not implemented between the operands.</li>
+</ul>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="p">(</span><span class="n">Real</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)):</span>
+            <span class="k">return</span> <span class="bp">NotImplemented</span>
+
+        <span class="n">t_step</span> <span class="o">=</span> <span class="nb">min</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">t_step</span><span class="p">,</span> <span class="n">other</span><span class="o">.</span><span class="n">t_step</span><span class="p">)</span> <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">t_step</span>
+        <span class="n">t_max</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">],</span> <span class="n">other</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">])</span> <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+        <span class="n">x_last</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">multiply</span><span class="p">(</span><span class="bp">self</span><span class="p">(</span><span class="n">t_max</span><span class="p">),</span> <span class="n">other</span><span class="p">(</span><span class="n">t_max</span><span class="p">))</span> <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)</span> <span class="k">else</span> <span class="n">np</span><span class="o">.</span><span class="n">multiply</span><span class="p">(</span><span class="bp">self</span><span class="p">(</span><span class="n">t_max</span><span class="p">),</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">other</span><span class="p">))</span>
+        <span class="n">t_list</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">t_max</span><span class="p">,</span> <span class="n">t_step</span><span class="p">)</span>
+
+        <span class="n">new_pwl</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="n">t_step</span><span class="o">=</span><span class="n">t_step</span><span class="p">)</span>
+
+        <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
+            <span class="n">other_copy</span> <span class="o">=</span> <span class="nb">float</span><span class="p">(</span><span class="n">other</span><span class="p">)</span>
+            <span class="n">other</span> <span class="o">=</span> <span class="k">lambda</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">:</span> <span class="n">other_copy</span>
+
+        <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">t_list</span><span class="p">:</span>
+            <span class="n">new_x</span> <span class="o">=</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">np</span><span class="o">.</span><span class="n">multiply</span><span class="p">(</span><span class="bp">self</span><span class="p">(</span><span class="n">t</span><span class="p">),</span> <span class="n">other</span><span class="p">(</span><span class="n">t</span><span class="p">)))</span>
+            <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">new_x</span><span class="p">)</span>
+
+        <span class="k">if</span> <span class="n">t_max</span> <span class="o">&gt;</span> <span class="n">new_pwl</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]:</span>
+            <span class="n">new_x</span> <span class="o">=</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">x_last</span><span class="p">)</span>
+            <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t_max</span><span class="p">,</span> <span class="n">new_x</span><span class="p">)</span>
+
+        <span class="k">return</span> <span class="n">new_pwl</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-57'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-57'>#</a>
+      </div>
+      
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="nd">@copy_doc</span><span class="p">(</span><span class="fm">__mul__</span><span class="p">)</span>
+    <span class="k">def</span> <span class="fm">__rmul__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span>
+        <span class="k">return</span> <span class="bp">self</span> <span class="o">*</span> <span class="n">other</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-58'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-58'>#</a>
+      </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-59'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-59'>#</a>
+      </div>
+      <h2><span id="division" href="division"> Division </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-60'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-60'>#</a>
+      </div>
+      <p><strong><code>__truediv__</code> and <code>__rtruediv__</code>  dunder methods of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__truediv__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="s2">&quot;PWL&quot;</span><span class="p">,</span> <span class="nb">float</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-61'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-61'>#</a>
+      </div>
+      <h3>Summary</h3>
+<p>Implements point-wise division of <code>PWL</code> objects with real numbers and other <code>PWL</code> objects.</p>
+<p>The new <code>PWL</code> objects created has <code>t_step</code> equal to the lower <code>t_step</code> between the operands.</p>
+<p>If one operand is longer than the other, extends the shorter one by holding it&rsquo;s last value.</p>
+<h3>Arguments</h3>
+<ul>
+<li>Numerator (<code>PWL</code> or <code>float</code>) : Thing being divided by the denominator.</li>
+<li>Denominator (<code>PWL</code> or <code>float</code>) : Thing that the numerator is being divided by.</li>
+</ul>
+<h3>Returns</h3>
+<ul>
+<li><code>PWL</code> : The ratio of the numerator and denominator.</li>
+</ul>
+<h3>Raises</h3>
+<ul>
+<li><code>TypeError</code> : Raised if operation is not implemented between the operands.</li>
+<li><code>ZeroDivisionError</code> : Raised if the denominator contains the point <code>(t, 0)</code> for any <code>t</code>.</li>
+</ul>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="p">(</span><span class="n">Real</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)):</span>
+            <span class="k">return</span> <span class="bp">NotImplemented</span>
+
+        <span class="n">t_step</span> <span class="o">=</span> <span class="nb">min</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">t_step</span><span class="p">,</span> <span class="n">other</span><span class="o">.</span><span class="n">t_step</span><span class="p">)</span> <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">t_step</span>
+        <span class="n">t_max</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">],</span> <span class="n">other</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">])</span> <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+        <span class="n">x_last</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">multiply</span><span class="p">(</span><span class="bp">self</span><span class="p">(</span><span class="n">t_max</span><span class="p">),</span> <span class="n">other</span><span class="p">(</span><span class="n">t_max</span><span class="p">))</span> <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)</span> <span class="k">else</span> <span class="n">np</span><span class="o">.</span><span class="n">true_divide</span><span class="p">(</span><span class="bp">self</span><span class="p">(</span><span class="n">t_max</span><span class="p">),</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">other</span><span class="p">))</span>
+        <span class="n">t_list</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">t_max</span><span class="p">,</span> <span class="n">t_step</span><span class="p">)</span>
+
+        <span class="n">new_pwl</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="n">t_step</span><span class="o">=</span><span class="n">t_step</span><span class="p">)</span>
+
+        <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
+            <span class="n">other_copy</span> <span class="o">=</span> <span class="nb">float</span><span class="p">(</span><span class="n">other</span><span class="p">)</span>
+            <span class="n">other</span> <span class="o">=</span> <span class="k">lambda</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">:</span> <span class="n">other_copy</span>
+
+        <span class="k">with</span> <span class="n">warnings</span><span class="o">.</span><span class="n">catch_warnings</span><span class="p">():</span>
+            <span class="n">warnings</span><span class="o">.</span><span class="n">simplefilter</span><span class="p">(</span><span class="s1">&#39;ignore&#39;</span><span class="p">)</span>
+            <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">t_list</span><span class="p">:</span>
+                <span class="n">left_x</span> <span class="o">=</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">np</span><span class="o">.</span><span class="n">true_divide</span><span class="p">(</span><span class="bp">self</span><span class="p">(</span><span class="n">t</span><span class="o">-</span><span class="n">t_step</span><span class="o">/</span><span class="mi">2</span><span class="p">),</span> <span class="n">other</span><span class="p">(</span><span class="n">t</span><span class="o">-</span><span class="n">t_step</span><span class="o">/</span><span class="mi">2</span><span class="p">)))</span>
+                <span class="n">center_x</span> <span class="o">=</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">np</span><span class="o">.</span><span class="n">true_divide</span><span class="p">(</span><span class="bp">self</span><span class="p">(</span><span class="n">t</span><span class="p">),</span> <span class="n">other</span><span class="p">(</span><span class="n">t</span><span class="p">)))</span>
+                <span class="n">rigth_x</span> <span class="o">=</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">np</span><span class="o">.</span><span class="n">true_divide</span><span class="p">(</span><span class="bp">self</span><span class="p">(</span><span class="n">t</span><span class="o">+</span><span class="n">t_step</span><span class="o">/</span><span class="mi">2</span><span class="p">),</span> <span class="n">other</span><span class="p">(</span><span class="n">t</span><span class="o">+</span><span class="n">t_step</span><span class="o">/</span><span class="mi">2</span><span class="p">)))</span>
+
+                <span class="k">if</span> <span class="n">np</span><span class="o">.</span><span class="n">isfinite</span><span class="p">(</span><span class="n">center_x</span><span class="p">):</span>
+                    <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">center_x</span><span class="p">)</span>
+                <span class="k">elif</span> <span class="n">np</span><span class="o">.</span><span class="n">isfinite</span><span class="p">(</span><span class="n">left_x</span><span class="p">)</span> <span class="ow">and</span> <span class="n">np</span><span class="o">.</span><span class="n">isfinite</span><span class="p">(</span><span class="n">rigth_x</span><span class="p">):</span>
+                    <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="p">(</span><span class="n">left_x</span><span class="o">+</span><span class="n">rigth_x</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span><span class="p">)</span>
+                <span class="k">elif</span> <span class="n">np</span><span class="o">.</span><span class="n">isfinite</span><span class="p">(</span><span class="n">left_x</span><span class="p">):</span>
+                    <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">left_x</span><span class="p">)</span>
+                <span class="k">elif</span> <span class="n">np</span><span class="o">.</span><span class="n">isfinite</span><span class="p">(</span><span class="n">rigth_x</span><span class="p">):</span>
+                    <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">rigth_x</span><span class="p">)</span>
+                <span class="k">else</span><span class="p">:</span>
+                    <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
+
+        <span class="k">if</span> <span class="n">t_max</span> <span class="o">&gt;</span> <span class="n">new_pwl</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]:</span>
+            <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t_max</span><span class="p">,</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">x_last</span><span class="p">))</span>
+
+        <span class="k">return</span> <span class="n">new_pwl</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-62'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-62'>#</a>
+      </div>
+      
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="nd">@copy_doc</span><span class="p">(</span><span class="fm">__truediv__</span><span class="p">)</span>
+    <span class="k">def</span> <span class="fm">__rtruediv__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span>
+        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
+            <span class="k">return</span> <span class="bp">NotImplemented</span>
+
+        <span class="n">t_step</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">t_step</span>
+        <span class="n">t_max</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+        <span class="n">t_list</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">t_max</span><span class="p">,</span> <span class="n">t_step</span><span class="p">)</span>
+        <span class="n">x_last</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">true_divide</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="bp">self</span><span class="p">(</span><span class="n">t_max</span><span class="p">))</span>
+
+        <span class="n">new_pwl</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="n">t_step</span><span class="o">=</span><span class="n">t_step</span><span class="p">)</span>
+
+        <span class="k">with</span> <span class="n">warnings</span><span class="o">.</span><span class="n">catch_warnings</span><span class="p">():</span>
+            <span class="n">warnings</span><span class="o">.</span><span class="n">simplefilter</span><span class="p">(</span><span class="s1">&#39;ignore&#39;</span><span class="p">)</span>
+            <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">t_list</span><span class="p">:</span>
+                <span class="n">left_x</span> <span class="o">=</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">np</span><span class="o">.</span><span class="n">true_divide</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="bp">self</span><span class="p">(</span><span class="n">t</span><span class="o">-</span><span class="n">t_step</span><span class="o">/</span><span class="mi">2</span><span class="p">)))</span>
+                <span class="n">center_x</span> <span class="o">=</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">np</span><span class="o">.</span><span class="n">true_divide</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="bp">self</span><span class="p">(</span><span class="n">t</span><span class="p">)))</span>
+                <span class="n">rigth_x</span> <span class="o">=</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">np</span><span class="o">.</span><span class="n">true_divide</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="bp">self</span><span class="p">(</span><span class="n">t</span><span class="o">+</span><span class="n">t_step</span><span class="o">/</span><span class="mi">2</span><span class="p">)))</span>
+
+                <span class="k">if</span> <span class="n">np</span><span class="o">.</span><span class="n">isfinite</span><span class="p">(</span><span class="n">center_x</span><span class="p">):</span>
+                    <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">center_x</span><span class="p">)</span>
+                <span class="k">elif</span> <span class="n">np</span><span class="o">.</span><span class="n">isfinite</span><span class="p">(</span><span class="n">left_x</span><span class="p">)</span> <span class="ow">and</span> <span class="n">np</span><span class="o">.</span><span class="n">isfinite</span><span class="p">(</span><span class="n">rigth_x</span><span class="p">):</span>
+                    <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="p">(</span><span class="n">left_x</span><span class="o">+</span><span class="n">rigth_x</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span><span class="p">)</span>
+                <span class="k">elif</span> <span class="n">np</span><span class="o">.</span><span class="n">isfinite</span><span class="p">(</span><span class="n">left_x</span><span class="p">):</span>
+                    <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">left_x</span><span class="p">)</span>
+                <span class="k">elif</span> <span class="n">np</span><span class="o">.</span><span class="n">isfinite</span><span class="p">(</span><span class="n">rigth_x</span><span class="p">):</span>
+                    <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">rigth_x</span><span class="p">)</span>
+                <span class="k">else</span><span class="p">:</span>
+                    <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
+
+        <span class="k">if</span> <span class="n">t_max</span> <span class="o">&gt;</span> <span class="n">new_pwl</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]:</span>
+            <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t_max</span><span class="p">,</span> <span class="n">x_last</span><span class="p">)</span>
+
+        <span class="k">return</span> <span class="n">new_pwl</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-63'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-63'>#</a>
+      </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-64'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-64'>#</a>
+      </div>
+      <h2><span id="exponentiation" href="exponentiation"> Exponentiation </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-65'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-65'>#</a>
+      </div>
+      <p><strong><code>__pow__</code> and <code>__rpow__</code>  dunder methods of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="fm">__pow__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="n">Union</span><span class="p">[</span><span class="s2">&quot;PWL&quot;</span><span class="p">,</span> <span class="nb">float</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-66'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-66'>#</a>
+      </div>
+      <h3>Summary</h3>
+<p>Implements point-wise exponentiation of <code>PWL</code> objects with real numbers and other <code>PWL</code> objects.</p>
+<p>If the result of the exponentiation ends up being a complex number, returns the real part of it.</p>
+<p>The new <code>PWL</code> objects created has <code>t_step</code> equal to the lower <code>t_step</code> between the operands.</p>
+<p>If one operand is longer than the other, extends the shorter one by holding it&rsquo;s last value.</p>
+<h3>Arguments</h3>
+<ul>
+<li>Base (<code>PWL</code> or <code>float</code>) : Thing being raised to the exponent.</li>
+<li>Exponent (<code>PWL</code> or <code>float</code>) : Thing to raise the base to.</li>
+</ul>
+<h3>Returns</h3>
+<ul>
+<li><code>PWL</code> : The power with the given base and exponent.</li>
+</ul>
+<h3>Raises</h3>
+<ul>
+<li><code>TypeError</code> : Raised if operation is not implemented between the operands.</li>
+</ul>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="p">(</span><span class="n">Real</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)):</span>
+            <span class="k">return</span> <span class="bp">NotImplemented</span>
+
+        <span class="n">t_step</span> <span class="o">=</span> <span class="nb">min</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">t_step</span><span class="p">,</span> <span class="n">other</span><span class="o">.</span><span class="n">t_step</span><span class="p">)</span> <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">t_step</span>
+        <span class="n">t_max</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">],</span> <span class="n">other</span><span class="o">.</span><span class="n">t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">])</span> <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+        <span class="n">x_last</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">multiply</span><span class="p">(</span><span class="bp">self</span><span class="p">(</span><span class="n">t_max</span><span class="p">),</span> <span class="n">other</span><span class="p">(</span><span class="n">t_max</span><span class="p">))</span> <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">PWL</span><span class="p">)</span> <span class="k">else</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">np</span><span class="o">.</span><span class="n">power</span><span class="p">(</span><span class="bp">self</span><span class="p">(</span><span class="n">t_max</span><span class="p">),</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">other</span><span class="p">),</span> <span class="n">dtype</span><span class="o">=</span><span class="nb">complex</span><span class="p">)</span><span class="o">.</span><span class="n">real</span><span class="p">)</span>
+        <span class="n">t_list</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">t_max</span><span class="p">,</span> <span class="n">t_step</span><span class="p">)</span>
+
+        <span class="n">new_pwl</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="n">t_step</span><span class="o">=</span><span class="n">t_step</span><span class="p">)</span>
+
+        <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
+            <span class="n">other_copy</span> <span class="o">=</span> <span class="nb">float</span><span class="p">(</span><span class="n">other</span><span class="p">)</span>
+            <span class="n">other</span> <span class="o">=</span> <span class="k">lambda</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">:</span> <span class="n">other_copy</span>
+
+        <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">t_list</span><span class="p">:</span>
+            <span class="n">new_x</span> <span class="o">=</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">np</span><span class="o">.</span><span class="n">power</span><span class="p">(</span><span class="bp">self</span><span class="p">(</span><span class="n">t</span><span class="p">),</span> <span class="n">other</span><span class="p">(</span><span class="n">t</span><span class="p">),</span> <span class="n">dtype</span><span class="o">=</span><span class="nb">complex</span><span class="p">)</span><span class="o">.</span><span class="n">real</span><span class="p">)</span>
+            <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">new_x</span><span class="p">)</span>
+
+        <span class="k">if</span> <span class="n">t_max</span> <span class="o">&gt;</span> <span class="n">new_pwl</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]:</span>
+            <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t_max</span><span class="p">,</span> <span class="n">cast</span><span class="p">(</span><span class="nb">float</span><span class="p">,</span> <span class="n">x_last</span><span class="p">))</span>
+
+        <span class="k">return</span> <span class="n">new_pwl</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-67'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-67'>#</a>
+      </div>
+      
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="nd">@copy_doc</span><span class="p">(</span><span class="fm">__pow__</span><span class="p">)</span>
+    <span class="k">def</span> <span class="fm">__rpow__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">other</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span>
+        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
+            <span class="k">return</span> <span class="bp">NotImplemented</span>
+
+        <span class="n">t_step</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">t_step</span>
+        <span class="n">t_max</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+        <span class="n">x_last</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">power</span><span class="p">(</span><span class="bp">self</span><span class="p">(</span><span class="n">t_max</span><span class="p">),</span> <span class="n">other</span><span class="p">,</span> <span class="n">dtype</span><span class="o">=</span><span class="nb">complex</span><span class="p">)</span><span class="o">.</span><span class="n">real</span>
+        <span class="n">t_list</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">t_max</span><span class="p">,</span> <span class="n">t_step</span><span class="p">)</span>
+
+        <span class="n">new_pwl</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="n">t_step</span><span class="o">=</span><span class="n">t_step</span><span class="p">)</span>
+
+        <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">t_list</span><span class="p">:</span>
+            <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">np</span><span class="o">.</span><span class="n">power</span><span class="p">(</span><span class="n">other</span><span class="p">,</span> <span class="bp">self</span><span class="p">(</span><span class="n">t</span><span class="p">),</span> <span class="n">dtype</span><span class="o">=</span><span class="nb">complex</span><span class="p">)</span><span class="o">.</span><span class="n">real</span><span class="p">)</span>
+
+        <span class="k">if</span> <span class="n">t_max</span> <span class="o">&gt;</span> <span class="n">new_pwl</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]:</span>
+            <span class="n">new_pwl</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t_max</span><span class="p">,</span> <span class="n">x_last</span><span class="p">)</span>
+
+        <span class="k">return</span> <span class="n">new_pwl</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-68'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-68'>#</a>
+      </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-69'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-69'>#</a>
       </div>
       <h2><span id="time-coordinates" href="time-coordinates"> Time Coordinates </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-27'>
+  <div class='section' id='section-70'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-27'>#</a>
+        <a class='octothorpe' href='#section-70'>#</a>
       </div>
       <p><strong><code>t_list</code> property of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">t_list</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">float</span><span class="p">]:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-28'>
+  <div class='section' id='section-71'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-28'>#</a>
+        <a class='octothorpe' href='#section-71'>#</a>
       </div>
       <h3>Type</h3>
 <ul>
 <li><code>list[float]</code></li>
 </ul>
 <h3>Summary</h3>
 <p>Read only property containing all the time coordinates of a <code>PWL</code> object.</p>
 <h3>Raises</h3>
 <ul>
 <li><code>AttributeError</code> : Raised if assignment was attempetd.</li>
 </ul>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span></pre></div>
+      <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[:]</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-29'>
+  <div class='section' id='section-72'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-29'>#</a>
+        <a class='octothorpe' href='#section-72'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-30'>
+  <div class='section' id='section-73'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-30'>#</a>
+        <a class='octothorpe' href='#section-73'>#</a>
       </div>
       <h2><span id="dependent-coordinates" href="dependent-coordinates"> Dependent Coordinates </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-31'>
+  <div class='section' id='section-74'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-31'>#</a>
+        <a class='octothorpe' href='#section-74'>#</a>
       </div>
       <p><strong><code>x_list</code> property of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">x_list</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="nb">float</span><span class="p">]:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-32'>
+  <div class='section' id='section-75'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-32'>#</a>
+        <a class='octothorpe' href='#section-75'>#</a>
       </div>
       <h3>Type</h3>
 <ul>
 <li><code>list[float]</code></li>
 </ul>
 <h3>Summary</h3>
 <p>Read only property containing all the dependent coordinates of a <code>PWL</code> object.</p>
 <h3>Raises</h3>
 <ul>
 <li><code>AttributeError</code> : Raised if assignment was attempetd.</li>
 </ul>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span></pre></div>
+      <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[:]</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-33'>
+  <div class='section' id='section-76'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-33'>#</a>
+        <a class='octothorpe' href='#section-76'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-34'>
+  <div class='section' id='section-77'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-34'>#</a>
+        <a class='octothorpe' href='#section-77'>#</a>
       </div>
       <h2><span id="default-timestep" href="default-timestep"> Default Timestep </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-35'>
+  <div class='section' id='section-78'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-35'>#</a>
+        <a class='octothorpe' href='#section-78'>#</a>
       </div>
       <p><strong><code>t_step</code> property of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">t_step</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-36'>
+  <div class='section' id='section-79'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-36'>#</a>
+        <a class='octothorpe' href='#section-79'>#</a>
       </div>
       <h3>Type</h3>
 <ul>
 <li><code>float</code></li>
 </ul>
 <h3>Summary</h3>
 <p>Property defining the default timestep of a <code>PWL</code> object.</p>
@@ -668,76 +1505,74 @@
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_step</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-37'>
+  <div class='section' id='section-80'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-37'>#</a>
+        <a class='octothorpe' href='#section-80'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@t_step</span><span class="o">.</span><span class="n">setter</span>
     <span class="k">def</span> <span class="nf">t_step</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_t_step</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">new_t_step</span><span class="p">,</span> <span class="nb">float</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Property &#39;t_step&#39; should be a real number but an object of type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">new_t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39; was assigned to it.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Property &#39;t_step&#39; should be a real number but an object of type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">new_t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39; was assigned to it&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="n">new_t_step</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Propety &#39;t_step&#39; should be strictly positive but a value of </span><span class="si">{</span><span class="n">new_t_step</span><span class="si">}</span><span class="s2"> was assigned to it.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Propety &#39;t_step&#39; should be strictly positive but a value of </span><span class="si">{</span><span class="n">new_t_step</span><span class="si">}</span><span class="s2"> was assigned to it&quot;</span><span class="p">)</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_t_step</span> <span class="o">=</span> <span class="n">new_t_step</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-38'>
+  <div class='section' id='section-81'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-38'>#</a>
+        <a class='octothorpe' href='#section-81'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-39'>
+  <div class='section' id='section-82'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-39'>#</a>
+        <a class='octothorpe' href='#section-82'>#</a>
       </div>
       <h2><span id="name" href="name"> Name </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-40'>
+  <div class='section' id='section-83'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-40'>#</a>
+        <a class='octothorpe' href='#section-83'>#</a>
       </div>
       <p><strong><code>name</code> property of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">name</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-41'>
+  <div class='section' id='section-84'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-41'>#</a>
+        <a class='octothorpe' href='#section-84'>#</a>
       </div>
       <h3>Type</h3>
 <ul>
 <li><code>str</code></li>
 </ul>
 <h3>Summary</h3>
 <p>Property defining the name of a <code>PWL</code> object for verbose output printing.</p>
@@ -748,81 +1583,79 @@
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_name</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-42'>
+  <div class='section' id='section-85'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-42'>#</a>
+        <a class='octothorpe' href='#section-85'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@name</span><span class="o">.</span><span class="n">setter</span>
     <span class="k">def</span> <span class="nf">name</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">new_name</span><span class="p">,</span> <span class="nb">str</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Property &#39;name&#39; should be a string but an object of type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">new_name</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39; was assigned to it.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Property &#39;name&#39; should be a string but an object of type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">new_name</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39; was assigned to it&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="n">new_name</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="s2">&quot;An empty string cannot be assigned to the &#39;name&#39; property.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;An empty string cannot be assigned to the &#39;name&#39; property&quot;</span><span class="p">)</span>
 
-        <span class="k">if</span> <span class="n">new_name</span> <span class="ow">in</span> <span class="n">PWL</span><span class="o">.</span> <span class="n">__dict_of_objects</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Name &#39;</span><span class="si">{</span><span class="n">new_name</span><span class="si">}</span><span class="s2">&#39; already in use.&quot;</span><span class="p">)</span>
+        <span class="k">if</span> <span class="n">new_name</span> <span class="ow">in</span> <span class="n">PWL</span><span class="o">.</span><span class="n">__dict_of_objects</span><span class="o">.</span><span class="n">keys</span><span class="p">():</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Name &#39;</span><span class="si">{</span><span class="n">new_name</span><span class="si">}</span><span class="s2">&#39; already in use&quot;</span><span class="p">)</span>
 
-        <span class="n">PWL</span><span class="o">.</span> <span class="n">__dict_of_objects</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span>
-        <span class="n">PWL</span><span class="o">.</span> <span class="n">__dict_of_objects</span><span class="p">[</span><span class="n">new_name</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span>
+        <span class="n">PWL</span><span class="o">.</span><span class="n">__dict_of_objects</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="p">)</span>
+        <span class="n">PWL</span><span class="o">.</span><span class="n">__dict_of_objects</span><span class="p">[</span><span class="n">new_name</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_name</span> <span class="o">=</span> <span class="n">new_name</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-43'>
+  <div class='section' id='section-86'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-43'>#</a>
+        <a class='octothorpe' href='#section-86'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-44'>
+  <div class='section' id='section-87'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-44'>#</a>
+        <a class='octothorpe' href='#section-87'>#</a>
       </div>
       <h2><span id="verbose-flag" href="verbose-flag"> Verbose Flag </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-45'>
+  <div class='section' id='section-88'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-45'>#</a>
+        <a class='octothorpe' href='#section-88'>#</a>
       </div>
       <p><strong><code>verbose</code> property of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">verbose</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-46'>
+  <div class='section' id='section-89'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-46'>#</a>
+        <a class='octothorpe' href='#section-89'>#</a>
       </div>
       <h3>Type</h3>
 <ul>
 <li><code>bool</code></li>
 </ul>
 <h3>Summary</h3>
 <p>Property defining if verbose output should be printed or not.</p>
@@ -832,73 +1665,72 @@
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-47'>
+  <div class='section' id='section-90'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-47'>#</a>
+        <a class='octothorpe' href='#section-90'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@verbose</span><span class="o">.</span><span class="n">setter</span>
     <span class="k">def</span> <span class="nf">verbose</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_verbose</span><span class="p">:</span> <span class="nb">bool</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">new_verbose</span><span class="p">,</span> <span class="nb">bool</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Attribute &#39;verbose&#39; should be a boolean but an object of type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">new_verbose</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39; was assigned to it.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Attribute &#39;verbose&#39; should be a boolean but an object of type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">new_verbose</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39; was assigned to it&quot;</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span> <span class="o">=</span> <span class="n">new_verbose</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-48'>
+  <div class='section' id='section-91'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-48'>#</a>
+        <a class='octothorpe' href='#section-91'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-49'>
+  <div class='section' id='section-92'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-49'>#</a>
+        <a class='octothorpe' href='#section-92'>#</a>
       </div>
       <h2><span id="plot-enable-flag" href="plot-enable-flag"> Plot Enable Flag </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-50'>
+  <div class='section' id='section-93'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-50'>#</a>
+        <a class='octothorpe' href='#section-93'>#</a>
       </div>
       <p><strong><code>plot_flag</code> property of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">plot_flag</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-51'>
+  <div class='section' id='section-94'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-51'>#</a>
+        <a class='octothorpe' href='#section-94'>#</a>
       </div>
       <p><em>Optional feature: Requires matplotlib</em></p>
 <h3>Type</h3>
 <ul>
 <li><code>bool</code></li>
 </ul>
 <h3>Summary</h3>
@@ -910,245 +1742,322 @@
 <h3>See Also</h3>
 <ul>
 <li><a href="#pwl-plotter">PWL Plotter</a></li>
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="p">(</span><span class="ow">not</span> <span class="n">_has_matplotlib</span><span class="p">)</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-            <span class="nb">print</span><span class="p">(</span>
-                <span class="s2">&quot;Optional features deactivated. Using the plot_flag does nothing in this case.&quot;</span><span class="p">)</span>
+            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Optional features deactivated. Using the plot_flag does nothing in this case&quot;</span><span class="p">)</span>
 
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_plot_flag</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-52'>
+  <div class='section' id='section-95'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-52'>#</a>
+        <a class='octothorpe' href='#section-95'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@plot_flag</span><span class="o">.</span><span class="n">setter</span>
     <span class="k">def</span> <span class="nf">plot_flag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">new_plot_flag</span><span class="p">:</span> <span class="nb">bool</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">new_plot_flag</span><span class="p">,</span> <span class="nb">bool</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Attribute &#39;plot_flag&#39; should be a boolean but an object of type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">new_plot_flag</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39; was assigned to it.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Attribute &#39;plot_flag&#39; should be a boolean but an object of type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">new_plot_flag</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39; was assigned to it&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="p">(</span><span class="ow">not</span> <span class="n">_has_matplotlib</span><span class="p">)</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-            <span class="nb">print</span><span class="p">(</span>
-                <span class="s2">&quot;Optional features deactivated. Using the plot_flag does nothing in this case.&quot;</span><span class="p">)</span>
+            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Optional features deactivated. Using the plot_flag does nothing in this case&quot;</span><span class="p">)</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_plot_flag</span> <span class="o">=</span> <span class="n">new_plot_flag</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-53'>
+  <div class='section' id='section-96'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-53'>#</a>
+        <a class='octothorpe' href='#section-96'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-54'>
+  <div class='section' id='section-97'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-54'>#</a>
+        <a class='octothorpe' href='#section-97'>#</a>
+      </div>
+      <h2><span id="initial-condition" href="initial-condition"> Initial Condition </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-98'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-98'>#</a>
+      </div>
+      <p><strong><code>initial</code> method of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">initial</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">x0</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">0</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-99'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-99'>#</a>
+      </div>
+      <h3>Summary</h3>
+<p>Method that sets the initial condition for the <code>PWL</code> object.</p>
+<h3>Parameters</h3>
+<ul>
+<li><code>x0</code> (<code>float</code>, optional) : Initial condition for <code>t=0</code>.</li>
+</ul>
+<h3>Returns</h3>
+<ul>
+<li><code>PWL</code> : Returns the object itself.</li>
+</ul>
+<h3>Raises</h3>
+<ul>
+<li><code>TypeError</code> : Raised if <code>x0</code> is not a real number.increasing.</li>
+<li><code>InitialConditionError</code> : Raised if the object already has initial conditions.</li>
+</ul>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">x0</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;x0&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">x0</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
+        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">!=</span> <span class="mi">0</span><span class="p">:</span>
+            <span class="k">raise</span> <span class="n">InitialConditionError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;PWL object already has initial condition of </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">x_list</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+
+        <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">x0</span><span class="p">)</span>
+
+        <span class="k">return</span> <span class="bp">self</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-100'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-100'>#</a>
+      </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-101'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-101'>#</a>
       </div>
       <h2><span id="last-value-holder" href="last-value-holder"> Last Value Holder </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-55'>
+  <div class='section' id='section-102'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-55'>#</a>
+        <a class='octothorpe' href='#section-102'>#</a>
       </div>
       <p><strong><code>hold</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">hold</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">hold</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-56'>
+  <div class='section' id='section-103'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-56'>#</a>
+        <a class='octothorpe' href='#section-103'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that holds the last value from the previous event for a given duration.</p>
 <p>If the <code>PWL</code> object is empty, adds the point <code>(0, 0)</code> and holds that.</p>
 <h3>Parameters</h3>
 <ul>
 <li><code>duration</code> (<code>float</code>) : Duration to hold the last value for. Should be strictly positive.</li>
 </ul>
+<h3>Returns</h3>
+<ul>
+<li><code>PWL</code> : Returns the object itself.</li>
+</ul>
 <h3>Raises</h3>
 <ul>
 <li><code>TypeError</code> : Raised if <code>duration</code> is not a real number.</li>
 <li><code>ValueError</code> : Raised if <code>duration</code> is not strictly positive.</li>
 <li><code>PrecisionError</code> : Raised if computational noise causes the time coordinates to not be strictly increasing.</li>
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">duration</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">duration</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding hold with duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding hold with duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">==</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;    Empty PWL object. Adding initial (0, 0) point.&quot;</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
+                <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;    Empty PWL object. Adding initial (0, 0) point&quot;</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
 
         <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">last_x</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
 
-        <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">last_x</span><span class="p">)</span></pre></div>
+        <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">last_x</span><span class="p">)</span>
+
+        <span class="k">return</span> <span class="bp">self</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-57'>
+  <div class='section' id='section-104'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-57'>#</a>
+        <a class='octothorpe' href='#section-104'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-58'>
+  <div class='section' id='section-105'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-58'>#</a>
+        <a class='octothorpe' href='#section-105'>#</a>
       </div>
       <h2><span id="linear-transition" href="linear-transition"> Linear Transition </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-59'>
+  <div class='section' id='section-106'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-59'>#</a>
+        <a class='octothorpe' href='#section-106'>#</a>
       </div>
       <p><strong><code>lin_transition</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">lin_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">lin_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-60'>
+  <div class='section' id='section-107'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-60'>#</a>
+        <a class='octothorpe' href='#section-107'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that generates a linear transition from the last value of the previous event to a given target with a given duration.</p>
 <p>If the <code>PWL</code> object is empty, adds the point <code>(0, 0)</code> and transitions from that.</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>target</code> (<code>float</code>) : Value to transition to.</li>
 <li><code>duration</code> (<code>float</code>) : Duration of the transition. Should be strictly positive.</li>
 </ul>
+<p>### Returns</p>
+<ul>
+<li><code>PWL</code> : Returns the object itself.</li>
+</ul>
 <h3>Raises</h3>
 <ul>
 <li><code>TypeError</code> : Raised if either <code>target</code> or duration` is not a real number.</li>
 <li><code>ValueError</code> : Raised if <code>duration</code> is not strictly positive.</li>
 <li><code>PrecisionError</code> : Raised if computational noise causes the time coordinates to not be strictly increasing.</li>
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;target&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">target</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;target&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">target</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">duration</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">duration</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+
+        <span class="bp">self</span><span class="o">.</span><span class="n">_nested_lin_transition</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">duration</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
 
-        <span class="bp">self</span><span class="o">.</span><span class="n">_lin_transition</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">duration</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span></pre></div>
+        <span class="k">return</span> <span class="bp">self</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-61'>
+  <div class='section' id='section-108'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-61'>#</a>
+        <a class='octothorpe' href='#section-108'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-62'>
+  <div class='section' id='section-109'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-62'>#</a>
+        <a class='octothorpe' href='#section-109'>#</a>
       </div>
       <h2><span id="rectangular-pulse" href="rectangular-pulse"> Rectangular Pulse </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-63'>
+  <div class='section' id='section-110'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-63'>#</a>
+        <a class='octothorpe' href='#section-110'>#</a>
       </div>
       <p><strong><code>rect_pulse</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">rect_pulse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">rect_pulse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-64'>
+  <div class='section' id='section-111'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-64'>#</a>
+        <a class='octothorpe' href='#section-111'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that generates a rectangular pulse with given amplitude and duration.</p>
 <p>If <code>duration</code> is less than or equal to <code>t_step</code> (<code>self.t_step</code> if <code>t_step</code> is not set), substitutes the pulse by a linear transition from the last value of the previous event to <code>value</code> with duration <code>t_step</code> (<code>self.t_step</code> if <code>t_step</code> is not set).</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>value</code> (<code>float</code>) : Amplitude of the pulse.</li>
 <li><code>duration</code> (<code>float</code>) : Duration of the pulse. Should be strictly positive.</li>
 <li><code>t_step</code> (<code>float</code>, optional) : Transition time for the discontinuity. Should be strictly positive. If not set, uses <code>self.t_step</code>.</li>
 </ul>
+<p>### Returns</p>
+<ul>
+<li><code>PWL</code> : Returns the object itself.</li>
+</ul>
 <h3>Raises</h3>
 <ul>
 <li><code>TypeError</code> : Raised if either <code>value</code>, duration<code>or</code>t_step` is not a real number.</li>
 <li><code>ValueError</code> : Raised if either <code>duration</code> or <code>t_step</code> is not strictly positive.</li>
 <li><code>PrecisionError</code> : Raised if computational noise causes the time coordinates to not be strictly increasing.</li>
 </ul>
 <h3>See Also</h3>
@@ -1157,102 +2066,102 @@
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="n">t_step</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">t_step</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_step</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;value&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">value</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;value&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">value</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">duration</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">t_step</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should either be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should either be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">duration</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="n">t_step</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding rectangular pulse with value of </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">, duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> and time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding rectangular pulse with value of </span><span class="si">{</span><span class="n">value</span><span class="si">}</span><span class="s2">, duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> and time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">duration</span> <span class="o">&lt;=</span> <span class="n">t_step</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">(</span>
-                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> is less than or equal to time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">. Converting to linear transition.&quot;</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_lin_transition</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">t_step</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
-            <span class="k">return</span>
+                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> is less than or equal to time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">. Converting to linear transition&quot;</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_nested_lin_transition</span><span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">t_step</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
+            <span class="k">return</span> <span class="bp">self</span>
 
         <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">==</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">value</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">value</span><span class="p">)</span>
             <span class="n">last_t</span> <span class="o">=</span> <span class="mi">0</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">value</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">value</span><span class="p">)</span>
 
-        <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">value</span><span class="p">)</span></pre></div>
+        <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">value</span><span class="p">)</span>
+
+        <span class="k">return</span> <span class="bp">self</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-65'>
+  <div class='section' id='section-112'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-65'>#</a>
+        <a class='octothorpe' href='#section-112'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-66'>
+  <div class='section' id='section-113'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-66'>#</a>
+        <a class='octothorpe' href='#section-113'>#</a>
       </div>
       <h2><span id="sawtooth-pulse" href="sawtooth-pulse"> Sawtooth Pulse </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-67'>
+  <div class='section' id='section-114'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-67'>#</a>
+        <a class='octothorpe' href='#section-114'>#</a>
       </div>
       <p><strong><code>sawtooth_pulse</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">sawtooth_pulse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">start</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">end</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">sawtooth_pulse</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">start</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">end</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-68'>
+  <div class='section' id='section-115'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-68'>#</a>
+        <a class='octothorpe' href='#section-115'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that generates a sawtooth pulse with given starting and ending amplitudes and duration.</p>
 <p>If <code>duration</code> is less than or equal to <code>t_step</code> (<code>self.t_step</code> if <code>t_step</code> is not set), substitutes the pulse by a linear transition from the last value of the previous event to <code>end</code> with duration <code>t_step</code> (<code>self.t_step</code> if <code>t_step</code> is not set).</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>start</code> (<code>float</code>) : Amplitude at the start of the pulse.</li>
 <li><code>end</code> (<code>float</code>) : Amplitude at the end of the pulse.</li>
 <li><code>duration</code> (<code>float</code>) : Duration of the pulse. Should be strictly positive.</li>
 <li><code>t_step</code> (<code>float</code>, optional) : Transition time for the discontinuity. Should be strictly positive. If not set, uses <code>self.t_step</code>.</li>
 </ul>
+<p>### Returns</p>
+<ul>
+<li><code>PWL</code> : Returns the object itself.</li>
+</ul>
 <h3>Raises</h3>
 <ul>
 <li><code>TypeError</code> : Raised if either <code>start</code>, <code>end</code>, duration<code>or</code>t_step` is not a real number.</li>
 <li><code>ValueError</code> : Raised if either <code>duration</code> or <code>t_step</code> is not strictly positive.</li>
 <li><code>PrecisionError</code> : Raised if computational noise causes the time coordinates to not be strictly increasing.</li>
 </ul>
 <h3>See Also</h3>
@@ -1261,94 +2170,89 @@
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="n">t_step</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">t_step</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_step</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">start</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;start&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">start</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;start&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">start</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">end</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;end&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">end</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;end&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">end</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">duration</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">t_step</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should either be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should either be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">duration</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="n">t_step</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding sawtoth pulse from </span><span class="si">{</span><span class="n">start</span><span class="si">}</span><span class="s2"> to </span><span class="si">{</span><span class="n">end</span><span class="si">}</span><span class="s2"> with duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> and time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding sawtoth pulse from </span><span class="si">{</span><span class="n">start</span><span class="si">}</span><span class="s2"> to </span><span class="si">{</span><span class="n">end</span><span class="si">}</span><span class="s2"> with duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> and time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">duration</span> <span class="o">&lt;=</span> <span class="n">t_step</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">(</span>
-                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> is less than or equal to time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">. Converting to linear transition.&quot;</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_lin_transition</span><span class="p">(</span><span class="n">end</span><span class="p">,</span> <span class="n">t_step</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
-            <span class="k">return</span>
+                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> is less than or equal to time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">. Converting to linear transition&quot;</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_nested_lin_transition</span><span class="p">(</span><span class="n">end</span><span class="p">,</span> <span class="n">t_step</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
+            <span class="k">return</span> <span class="bp">self</span>
 
         <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">==</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">start</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">start</span><span class="p">)</span>
             <span class="n">last_t</span> <span class="o">=</span> <span class="mi">0</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">start</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">start</span><span class="p">)</span>
 
-        <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">end</span><span class="p">)</span></pre></div>
+        <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">end</span><span class="p">)</span>
+
+        <span class="k">return</span> <span class="bp">self</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-69'>
+  <div class='section' id='section-116'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-69'>#</a>
+        <a class='octothorpe' href='#section-116'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-70'>
+  <div class='section' id='section-117'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-70'>#</a>
+        <a class='octothorpe' href='#section-117'>#</a>
       </div>
       <h2><span id="exponential-transition" href="exponential-transition"> Exponential Transition </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-71'>
+  <div class='section' id='section-118'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-71'>#</a>
+        <a class='octothorpe' href='#section-118'>#</a>
       </div>
       <p><strong><code>exp_transition</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">exp_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">tau</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">exp_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">tau</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-72'>
+  <div class='section' id='section-119'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-72'>#</a>
+        <a class='octothorpe' href='#section-119'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that generates an exponential transition from the last value of the previous event to a given target with a given duration.</p>
 <p>If the <code>PWL</code> object is empty, adds the point <code>(0, 0)</code> and transitions from that.</p>
 <p>Let&rsquo;s call <code>x0</code> the last value of the previous event and <code>t0</code> the instant when the transition begins. The transition will follow thw following form:</p>
 <pre><code>f(t) = A + B*exp(-t/tau)
 </code></pre>
@@ -1361,14 +2265,18 @@
 <h3>Arguments</h3>
 <ul>
 <li><code>target</code> (<code>float</code>) : Value to transition to.</li>
 <li><code>duration</code> (<code>float</code>) : Duration of the transition. Should be strictly positive.</li>
 <li><code>tau</code> (<code>float</code>) : Time constant of the exponential. SHould be non zero.</li>
 <li><code>t_step</code> (<code>float</code>, optional) : Timestep between consecutive points inside the transition. Should be strictly positive. If not set, uses <code>self.t_step</code>.</li>
 </ul>
+<p>### Returns</p>
+<ul>
+<li><code>PWL</code> : Returns the object itself.</li>
+</ul>
 <h3>Raises</h3>
 <ul>
 <li><code>TypeError</code> : Raised if either <code>target</code>, <code>duration</code>, tau<code>or</code>t_step` is not a real number.</li>
 <li><code>ValueError</code> : Raised if either <code>duration</code> or <code>t_step</code> is not strictly positive or <code>tau</code> is equal to zero.</li>
 <li><code>PrecisionError</code> : Raised if computational noise causes the time coordinates to not be strictly increasing.</li>
 </ul>
 <h3>See Also</h3>
@@ -1377,103 +2285,97 @@
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="n">t_step</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">t_step</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_step</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;target&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">target</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;target&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">target</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">duration</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">tau</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;tau&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">tau</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;tau&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">tau</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">t_step</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should either be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should either be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">duration</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="n">tau</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;Argument &#39;tau&#39; should be non zero.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;Argument &#39;tau&#39; should be non zero&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="n">t_step</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding exponential transition with target of </span><span class="si">{</span><span class="n">target</span><span class="si">}</span><span class="s2">, time constant of </span><span class="si">{</span><span class="n">tau</span><span class="si">}</span><span class="s2">, duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> and time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding exponential transition with target of </span><span class="si">{</span><span class="n">target</span><span class="si">}</span><span class="s2">, time constant of </span><span class="si">{</span><span class="n">tau</span><span class="si">}</span><span class="s2">, duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> and time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">duration</span> <span class="o">&lt;=</span> <span class="n">t_step</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">(</span>
-                    <span class="sa">f</span><span class="s2">&quot;    Duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> is less than or equal to time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">. Converting to linear transition.&quot;</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_lin_transition</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">t_step</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span>
-            <span class="k">return</span>
+                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;    Duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> is less than or equal to time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">. Converting to linear transition&quot;</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_nested_lin_transition</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">t_step</span><span class="p">,</span> <span class="mi">2</span><span class="p">)</span>
+            <span class="k">return</span> <span class="bp">self</span>
 
         <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">==</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;    Empty PWL object. Adding initial (0, 0) point.&quot;</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
+                <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;    Empty PWL object. Adding initial (0, 0) point&quot;</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
 
         <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">last_x</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
 
-        <span class="n">f</span> <span class="o">=</span> <span class="n">_exp_transition_func</span><span class="p">(</span><span class="n">tau</span><span class="o">=</span><span class="n">tau</span><span class="p">,</span> <span class="n">t1</span><span class="o">=</span><span class="n">last_t</span><span class="p">,</span> <span class="n">t2</span><span class="o">=</span><span class="n">last_t</span> <span class="o">+</span>
-                                 <span class="n">duration</span><span class="p">,</span> <span class="n">f1</span><span class="o">=</span><span class="n">last_x</span><span class="p">,</span> <span class="n">f2</span><span class="o">=</span><span class="n">target</span><span class="p">)</span>
+        <span class="n">f</span> <span class="o">=</span> <span class="n">exp_transition_func</span><span class="p">(</span><span class="n">tau</span><span class="o">=</span><span class="n">tau</span><span class="p">,</span> <span class="n">t1</span><span class="o">=</span><span class="n">last_t</span><span class="p">,</span> <span class="n">t2</span><span class="o">=</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">f1</span><span class="o">=</span><span class="n">last_x</span><span class="p">,</span> <span class="n">f2</span><span class="o">=</span><span class="n">target</span><span class="p">)</span>
 
         <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">t_step</span><span class="p">):</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">f</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">f</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
 
-        <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
+        <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span>
+
+        <span class="k">return</span> <span class="bp">self</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-73'>
+  <div class='section' id='section-120'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-73'>#</a>
+        <a class='octothorpe' href='#section-120'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-74'>
+  <div class='section' id='section-121'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-74'>#</a>
+        <a class='octothorpe' href='#section-121'>#</a>
       </div>
       <h2><span id="half-sine-transition" href="half-sine-transition"> Half Sine Transition </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-75'>
+  <div class='section' id='section-122'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-75'>#</a>
+        <a class='octothorpe' href='#section-122'>#</a>
       </div>
       <p><strong><code>sin_transition</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">sin_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">sin_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-76'>
+  <div class='section' id='section-123'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-76'>#</a>
+        <a class='octothorpe' href='#section-123'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that generates a half sine transition from the last value of the previous event to a given target with a given duration.</p>
 <p>If the <code>PWL</code> object is empty, adds the point <code>(0, 0)</code> and transitions from that.</p>
 <p>Let&rsquo;s call <code>x0</code> the last value of the previous event and <code>t0</code> the instant when the transition begins. The transition will follow thw following form:</p>
 <pre><code>f(t) = A + B*sin(w*t - phi)
 </code></pre>
@@ -1486,14 +2388,18 @@
 <p>If <code>duration</code> is less than or equal to <code>t_step</code> (<code>self.t_step</code> if <code>t_step</code> is not set), substitutes the pulse by a linear transition from the last value of the previous event to <code>target</code> with duration <code>t_step</code> (<code>self.t_step</code> if <code>t_step</code> is not set).</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>target</code> (<code>float</code>) : Value to transition to.</li>
 <li><code>duration</code> (<code>float</code>) : Duration of the transition. Should be strictly positive.</li>
 <li><code>t_step</code> (<code>float</code>, optional) : Timestep between consecutive points inside the transition. Should be strictly positive. If not set, uses <code>self.t_step</code>.</li>
 </ul>
+<p>### Returns</p>
+<ul>
+<li><code>PWL</code> : Returns the object itself.</li>
+</ul>
 <h3>Raises</h3>
 <ul>
 <li><code>TypeError</code> : Raised if either <code>target</code>, <code>duration</code> or <code>t_step</code> is not a real number.</li>
 <li><code>ValueError</code> : Raised if either <code>duration</code> or <code>t_step</code> is not strictly positive.</li>
 <li><code>PrecisionError</code> : Raised if computational noise causes the time coordinates to not be strictly increasing.</li>
 </ul>
 <h3>See Also</h3>
@@ -1502,98 +2408,94 @@
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="n">t_step</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">t_step</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_step</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;target&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">target</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;target&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">target</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">duration</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">t_step</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should either be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should either be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">duration</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="n">t_step</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding sinusoidal transition with target of </span><span class="si">{</span><span class="n">target</span><span class="si">}</span><span class="s2">, duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> and time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding sinusoidal transition with target of </span><span class="si">{</span><span class="n">target</span><span class="si">}</span><span class="s2">, duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> and time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">duration</span> <span class="o">&lt;=</span> <span class="n">t_step</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">(</span>
-                    <span class="sa">f</span><span class="s2">&quot;    Duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> is less than or equal to time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">. Converting to linear transition.&quot;</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_lin_transition</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">t_step</span><span class="p">,</span> <span class="n">n</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
-            <span class="k">return</span>
+                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;    Duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> is less than or equal to time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">. Converting to linear transition&quot;</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_nested_lin_transition</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">t_step</span><span class="p">,</span> <span class="n">n</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
+            <span class="k">return</span> <span class="bp">self</span>
 
         <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">==</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;    Empty PWL object. Adding initial (0, 0) point.&quot;</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
+                <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;    Empty PWL object. Adding initial (0, 0) point&quot;</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
 
         <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">last_x</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
 
-        <span class="n">f</span> <span class="o">=</span> <span class="n">_sin_transition_func</span><span class="p">(</span>
+        <span class="n">f</span> <span class="o">=</span> <span class="n">sin_transition_func</span><span class="p">(</span>
             <span class="n">t1</span><span class="o">=</span><span class="n">last_t</span><span class="p">,</span> <span class="n">t2</span><span class="o">=</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">f1</span><span class="o">=</span><span class="n">last_x</span><span class="p">,</span> <span class="n">f2</span><span class="o">=</span><span class="n">target</span><span class="p">)</span>
 
         <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">t_step</span><span class="p">):</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">f</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">f</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
+
+        <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span>
 
-        <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
+        <span class="k">return</span> <span class="bp">self</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-77'>
+  <div class='section' id='section-124'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-77'>#</a>
+        <a class='octothorpe' href='#section-124'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-78'>
+  <div class='section' id='section-125'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-78'>#</a>
+        <a class='octothorpe' href='#section-125'>#</a>
       </div>
       <h2><span id="smoothstep-transition" href="smoothstep-transition"> Smoothstep Transition </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-79'>
+  <div class='section' id='section-126'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-79'>#</a>
+        <a class='octothorpe' href='#section-126'>#</a>
       </div>
       <p><strong><code>smoothstep_transition</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">smoothstep_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">smoothstep_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t_step</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">float</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-80'>
+  <div class='section' id='section-127'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-80'>#</a>
+        <a class='octothorpe' href='#section-127'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that generates a smoothstep transition from the last value of the previous event to a given target with a given duration.</p>
 <p>If the <code>PWL</code> object is empty, adds the point <code>(0, 0)</code> and transitions from that.</p>
 <p>Let&rsquo;s call <code>x0</code> the last value of the previous event and <code>t0</code> the instant when the transition begins. The transition will follow thw following form:</p>
 <pre><code>f(t) = A + B*t + C*t^2 + D*t^3
 </code></pre>
@@ -1605,14 +2507,18 @@
 <p>If <code>duration</code> is less than or equal to <code>t_step</code> (<code>self.t_step</code> if <code>t_step</code> is not set), substitutes the pulse by a linear transition from the last value of the previous event to <code>target</code> with duration <code>t_step</code> (<code>self.t_step</code> if <code>t_step</code> is not set).</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>target</code> (<code>float</code>) : Value to transition to.</li>
 <li><code>duration</code> (<code>float</code>) : Duration of the transition. Should be strictly positive.</li>
 <li><code>t_step</code> (<code>float</code>, optional) : Timestep between consecutive points inside the transition. Should be strictly positive. If not set, uses <code>self.t_step</code>.</li>
 </ul>
+<p>### Returns</p>
+<ul>
+<li><code>PWL</code> : Returns the object itself.</li>
+</ul>
 <h3>Raises</h3>
 <ul>
 <li><code>TypeError</code> : Raised if either <code>target</code>, <code>duration</code> or <code>t_step</code> is not a real number.</li>
 <li><code>ValueError</code> : Raised if either <code>duration</code> or <code>t_step</code> is not strictly positive.</li>
 <li><code>PrecisionError</code> : Raised if computational noise causes the time coordinates to not be strictly increasing.</li>
 </ul>
 <h3>See Also</h3>
@@ -1621,98 +2527,94 @@
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="n">t_step</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">t_step</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_step</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;target&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">target</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;target&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">target</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">duration</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">duration</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">t_step</span><span class="p">,</span> <span class="n">Real</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should either be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should either be a real number but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">t_step</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">duration</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;duration&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="n">t_step</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;t_step&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding smoothstep transition with target of </span><span class="si">{</span><span class="n">target</span><span class="si">}</span><span class="s2">, duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> and time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding smoothstep transition with target of </span><span class="si">{</span><span class="n">target</span><span class="si">}</span><span class="s2">, duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> and time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">duration</span> <span class="o">&lt;=</span> <span class="n">t_step</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">(</span>
-                    <span class="sa">f</span><span class="s2">&quot;    Duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> is less than or equal to time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">. Converting to linear transition.&quot;</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_lin_transition</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">t_step</span><span class="p">,</span> <span class="n">n</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
-            <span class="k">return</span>
+                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;    Duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2"> is less than or equal to time step of </span><span class="si">{</span><span class="n">t_step</span><span class="si">}</span><span class="s2">. Converting to linear transition&quot;</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_nested_lin_transition</span><span class="p">(</span><span class="n">target</span><span class="p">,</span> <span class="n">t_step</span><span class="p">,</span> <span class="n">n</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
+            <span class="k">return</span> <span class="bp">self</span>
 
         <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">==</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;    Empty PWL object. Adding initial (0, 0) point.&quot;</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
+                <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;    Empty PWL object. Adding initial (0, 0) point&quot;</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
 
         <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">last_x</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
 
-        <span class="n">f</span> <span class="o">=</span> <span class="n">_smoothstep_transition_func</span><span class="p">(</span>
+        <span class="n">f</span> <span class="o">=</span> <span class="n">smoothstep_transition_func</span><span class="p">(</span>
             <span class="n">t1</span><span class="o">=</span><span class="n">last_t</span><span class="p">,</span> <span class="n">t2</span><span class="o">=</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">f1</span><span class="o">=</span><span class="n">last_x</span><span class="p">,</span> <span class="n">f2</span><span class="o">=</span><span class="n">target</span><span class="p">)</span>
 
         <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">t_step</span><span class="p">):</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">f</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">f</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
 
-        <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
+        <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span>
+
+        <span class="k">return</span> <span class="bp">self</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-81'>
+  <div class='section' id='section-128'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-81'>#</a>
+        <a class='octothorpe' href='#section-128'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-82'>
+  <div class='section' id='section-129'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-82'>#</a>
+        <a class='octothorpe' href='#section-129'>#</a>
       </div>
-      <h2><span id="pwl-file-writer" href="pwl-file-writer"> PWL File Writer </span></h2>
+      <h2><span id="file-writer" href="file-writer"> File Writer </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-83'>
+  <div class='section' id='section-130'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-83'>#</a>
+        <a class='octothorpe' href='#section-130'>#</a>
       </div>
       <p><strong><code>write</code> method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">write</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">filename</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">precision</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">10</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-84'>
+  <div class='section' id='section-131'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-84'>#</a>
+        <a class='octothorpe' href='#section-131'>#</a>
       </div>
       <h3>Summary</h3>
 <p>Method that takes a <code>PWL</code> object and writes a PWL file with it&rsquo;s <code>(t, x)</code> coordinates in scientific notation.</p>
 <p>If the specified file already exists, overwrites it.</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>filename</code> (<code>str</code>, optional) : Name of file to be created. If not set, uses <code>self.name</code> if an added <code>.txt</code> extension.</li>
@@ -1726,26 +2628,23 @@
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="n">filename</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="n">filename</span> <span class="o">=</span> <span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s1">.txt&#39;</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">filename</span><span class="p">,</span> <span class="nb">str</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;filename&#39; should be a string but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;filename&#39; should be a string but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">filename</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">precision</span><span class="p">,</span> <span class="nb">int</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;precision&#39; should be an integer but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">precision</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;precision&#39; should be an integer but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">precision</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">precision</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;precision&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">precision</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;precision&#39; should be strictly positive but has value of </span><span class="si">{</span><span class="n">precision</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Writing PWL file to </span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Writing PWL file to </span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="n">t_list</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span>
         <span class="n">x_list</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span>
 
         <span class="k">with</span> <span class="nb">open</span><span class="p">(</span><span class="n">filename</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
             <span class="n">ti_str</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">format_float_scientific</span><span class="p">(</span>
                 <span class="n">t_list</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">precision</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="n">unique</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">sign</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
@@ -1755,102 +2654,165 @@
             <span class="n">last_t</span> <span class="o">=</span> <span class="n">ti_str</span>
             <span class="k">for</span> <span class="n">ti</span><span class="p">,</span> <span class="n">xi</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">t_list</span><span class="p">[</span><span class="mi">1</span><span class="p">:],</span> <span class="n">x_list</span><span class="p">[</span><span class="mi">1</span><span class="p">:]):</span>
                 <span class="n">ti_str</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">format_float_scientific</span><span class="p">(</span>
                     <span class="n">ti</span><span class="p">,</span> <span class="n">precision</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="n">unique</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">sign</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
                 <span class="n">xi_str</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">format_float_scientific</span><span class="p">(</span>
                     <span class="n">xi</span><span class="p">,</span> <span class="n">precision</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="n">unique</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">sign</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
                 <span class="k">if</span> <span class="n">ti_str</span> <span class="o">==</span> <span class="n">last_t</span><span class="p">:</span>
-                    <span class="k">raise</span> <span class="n">PrecisionError</span><span class="p">(</span>
-                        <span class="s2">&quot;The chosen precision level caused the written time coordinates to not be strictly increasing.&quot;</span><span class="p">)</span>
+                    <span class="k">raise</span> <span class="n">PrecisionError</span><span class="p">(</span><span class="s2">&quot;The chosen precision level caused the written time coordinates to not be strictly increasing&quot;</span><span class="p">)</span>
                 <span class="n">file</span><span class="o">.</span><span class="n">write</span><span class="p">(</span>
                     <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">ti_str</span><span class="si">}</span><span class="s2">    </span><span class="si">{</span><span class="n">xi_str</span><span class="si">}</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
                 <span class="n">last_t</span> <span class="o">=</span> <span class="n">ti_str</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-85'>
+  <div class='section' id='section-132'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-85'>#</a>
+        <a class='octothorpe' href='#section-132'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-86'>
+  <div class='section' id='section-133'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-86'>#</a>
+        <a class='octothorpe' href='#section-133'>#</a>
+      </div>
+      <h2><span id="object-copy" href="object-copy"> Object Copy </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-134'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-134'>#</a>
+      </div>
+      <p><strong><code>copy</code> class method of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">copy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="s2">&quot;PWL&quot;</span><span class="p">:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-135'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-135'>#</a>
+      </div>
+      <h3>Summary</h3>
+<p>Method that creates a deep copy of a <code>PWL</code> object.</p>
+<h3>Arguments</h3>
+<ul>
+<li><code>name</code> (<code>str</code>, optional) : Name of the <code>PWL</code> object used for verbose output printing. Should not be empty. If not set, automatically generates a name based on already taken names. </li>
+</ul>
+<h3>Returns</h3>
+<ul>
+<li><code>PWL</code></li>
+</ul>
+<h3>Raises</h3>
+<ul>
+<li><code>TypeError</code> : Raised if <code>name</code> is not a string.</li>
+<li><code>ValueError</code> : Raised if <code>name</code> is either empty or already taken.</li>
+</ul>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>        <span class="n">new_pwl</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="n">t_step</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">t_step</span><span class="p">,</span> <span class="n">name</span><span class="o">=</span><span class="n">name</span><span class="p">,</span> <span class="n">verbose</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">verbose</span><span class="p">)</span>
+
+        <span class="n">new_pwl</span><span class="o">.</span><span class="n">_t_list</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">t_list</span>
+        <span class="n">new_pwl</span><span class="o">.</span><span class="n">_x_list</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">x_list</span>
+
+        <span class="k">return</span> <span class="n">new_pwl</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-136'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-136'>#</a>
+      </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-137'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-137'>#</a>
       </div>
       <h2><span id="pwl-plotter" href="pwl-plotter"> PWL Plotter </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-87'>
+  <div class='section' id='section-138'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-87'>#</a>
+        <a class='octothorpe' href='#section-138'>#</a>
       </div>
       <p><strong><code>plot</code> class method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="nd">@classmethod</span>
     <span class="k">def</span> <span class="nf">plot</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">merge</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-88'>
+  <div class='section' id='section-139'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-88'>#</a>
+        <a class='octothorpe' href='#section-139'>#</a>
       </div>
       <p><em>Optional feature: Requires matplotlib</em></p>
 <h3>Summary</h3>
 <p>Class method that takes all instances of the <code>PWL</code> class with plot enable flag set to <code>True</code> and plots them on the same time axis.</p>
 <h3>Arguments</h3>
 <ul>
-<li><code>merge</code> (<code>bool</code>, optional) : Flag indicating if all signals should be ploted on the same strip or separeted. If not set, defaults to False.</li>
+<li><code>merge</code> (<code>bool</code>, optional) : Flag indicating if all signals should be ploted on the same strip or separeted. If not set, defaults to <code>False</code>.</li>
 </ul>
 <h3>Raises</h3>
 <ul>
 <li><code>TypeError</code> : Raised if <code>merge</code> is not a boolean.</li>
 <li><code>ImportError</code> : Raised if the matplotlib package is not installed.</li>
 </ul>
 <h3>See Also</h3>
 <ul>
 <li><a href="#plot-enable-flag">Plot Enable Flag</a></li>
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="n">_has_matplotlib</span><span class="p">:</span>
-            <span class="k">raise</span> <span class="ne">ImportError</span><span class="p">(</span>
-                <span class="s2">&quot;Optional plotting features are deactivated. Install matplotlib to use.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">ImportError</span><span class="p">(</span><span class="s2">&quot;Optional plotting features are deactivated. Install matplotlib to use&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">merge</span><span class="p">,</span> <span class="nb">bool</span><span class="p">):</span>
-            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Argument &#39;merge&#39; should be a boolean but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">merge</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Argument &#39;merge&#39; should be a boolean but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">merge</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
 
         <span class="n">dict_of_objects</span> <span class="o">=</span> <span class="p">{</span><span class="n">key</span><span class="p">:</span> <span class="n">pwl</span> <span class="k">for</span> <span class="n">key</span><span class="p">,</span>
                            <span class="n">pwl</span> <span class="ow">in</span> <span class="bp">cls</span><span class="o">.</span><span class="n">__dict_of_objects</span><span class="o">.</span><span class="n">items</span><span class="p">()</span> <span class="k">if</span> <span class="n">pwl</span><span class="o">.</span><span class="n">plot_flag</span><span class="p">}</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="n">dict_of_objects</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">None</span>
 
         <span class="k">if</span> <span class="n">merge</span><span class="p">:</span>
             <span class="n">axs</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">subplots</span><span class="p">(</span><span class="n">nrows</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span> <span class="n">sharex</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">squeeze</span><span class="o">=</span><span class="kc">False</span><span class="p">)[</span><span class="mi">1</span><span class="p">]</span>
             <span class="n">axs</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">repeat</span><span class="p">(</span><span class="n">axs</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">dict_of_objects</span><span class="p">))</span>
         <span class="k">else</span><span class="p">:</span>
-            <span class="n">axs</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">subplots</span><span class="p">(</span><span class="n">nrows</span><span class="o">=</span><span class="nb">len</span><span class="p">(</span><span class="n">dict_of_objects</span><span class="p">),</span>
-                               <span class="n">sharex</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">squeeze</span><span class="o">=</span><span class="kc">False</span><span class="p">)[</span><span class="mi">1</span><span class="p">]</span>
+            <span class="n">axs</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">subplots</span><span class="p">(</span><span class="n">nrows</span><span class="o">=</span><span class="nb">len</span><span class="p">(</span><span class="n">dict_of_objects</span><span class="p">),</span> <span class="n">sharex</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">squeeze</span><span class="o">=</span><span class="kc">False</span><span class="p">)[</span><span class="mi">1</span><span class="p">]</span>
             <span class="n">axs</span> <span class="o">=</span> <span class="n">axs</span><span class="o">.</span><span class="n">flatten</span><span class="p">()</span>
         <span class="n">x_max</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">0</span>
 
         <span class="k">for</span> <span class="n">key</span><span class="p">,</span> <span class="n">ax</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">dict_of_objects</span><span class="p">,</span> <span class="n">axs</span><span class="p">):</span>
             <span class="n">pwl</span> <span class="o">=</span> <span class="n">dict_of_objects</span><span class="p">[</span><span class="n">key</span><span class="p">]</span>
             <span class="k">if</span> <span class="ow">not</span> <span class="n">pwl</span><span class="o">.</span><span class="n">_plot_flag</span><span class="p">:</span>
                 <span class="k">continue</span>
@@ -1862,449 +2824,216 @@
             <span class="n">ax</span><span class="o">.</span><span class="n">set_ylabel</span><span class="p">(</span><span class="n">label</span><span class="p">)</span>
 
         <span class="n">axs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">set_xlim</span><span class="p">(</span><span class="n">xmin</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">xmax</span><span class="o">=</span><span class="n">x_max</span><span class="p">)</span>
         <span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-89'>
+  <div class='section' id='section-140'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-89'>#</a>
-      </div>
-      <h1><span id="private-methods-and-functions" href="private-methods-and-functions"> Private Methods and Functions </span></h1>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-90'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-90'>#</a>
-      </div>
-      <p>From this point forward, all listed methods and functions are not intended to be used by the user. Brief descriptions will be provided, but documentation will be kept to a minimum.</p>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-91'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-91'>#</a>
+        <a class='octothorpe' href='#section-140'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-92'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-92'>#</a>
-      </div>
-      <h2><span id="pwl-point-adder" href="pwl-point-adder"> PWL Point Adder </span></h2>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-93'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-93'>#</a>
-      </div>
-      <p><strong><code>_add</code> private method of <code>PWL</code> class</strong></p>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">x</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-94'>
+  <div class='section' id='section-141'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-94'>#</a>
+        <a class='octothorpe' href='#section-141'>#</a>
       </div>
-      <p>Private method that adds a <code>(t, x)</code> point to a <code>PWL</code> object of any size.</p>
+      
     </div>
     <div class='code'>
-      <div class="highlight"><pre>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">t</span> <span class="o">&lt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]:</span>
-            <span class="k">raise</span> <span class="n">PrecisionError</span><span class="p">(</span>
-                <span class="sa">f</span><span class="s2">&quot;Internal Python rounding caused the time coordinates to not be strictly increasing when adding points to </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_insert</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">x</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">t</span> <span class="o">&lt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]:</span>
+            <span class="k">raise</span> <span class="n">PrecisionError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Internal Python rounding caused the time coordinates to not be strictly increasing when adding points to </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">==</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">)</span> <span class="o">&lt;</span> <span class="mi">2</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">t</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">x</span><span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_colinear_eliminator</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">t</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-95'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-95'>#</a>
-      </div>
-      <hr />
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-96'>
+  <div class='section' id='section-142'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-96'>#</a>
+        <a class='octothorpe' href='#section-142'>#</a>
       </div>
-      <h2><span id="colinear-points-eliminator" href="colinear-points-eliminator"> Colinear Points Eliminator </span></h2>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-97'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-97'>#</a>
-      </div>
-      <p><strong><code>_colinear_eliminator</code> private method of <code>PWL</code> class</strong></p>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_colinear_eliminator</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">x</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-98'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-98'>#</a>
-      </div>
-      <p>Private method that adds a <code>(t, x)</code> point to a <code>PWL</code> object with 2 or more points without consecutive colinear points.</p>
+      
     </div>
     <div class='code'>
-      <div class="highlight"><pre>        <span class="n">t_n_1</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_colinear_eliminator</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">x</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="n">t_n_1</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">t_n_2</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
 
         <span class="n">x_n_1</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">x_n_2</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
 
         <span class="n">last_m</span> <span class="o">=</span> <span class="p">(</span><span class="n">x_n_1</span> <span class="o">-</span> <span class="n">x_n_2</span><span class="p">)</span><span class="o">/</span><span class="p">(</span><span class="n">t_n_1</span> <span class="o">-</span> <span class="n">t_n_2</span><span class="p">)</span>
         <span class="n">new_m</span> <span class="o">=</span> <span class="p">(</span><span class="n">x</span> <span class="o">-</span> <span class="n">x_n_1</span><span class="p">)</span><span class="o">/</span><span class="p">(</span><span class="n">t</span> <span class="o">-</span> <span class="n">t_n_1</span><span class="p">)</span>
 
-        <span class="k">if</span> <span class="n">last_m</span> <span class="o">==</span> <span class="n">new_m</span><span class="p">:</span>
+        <span class="k">if</span> <span class="n">is_within</span><span class="p">(</span><span class="n">last_m</span><span class="p">,</span> <span class="n">new_m</span><span class="p">):</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span> <span class="o">=</span> <span class="n">t</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span> <span class="o">=</span> <span class="n">x</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">t</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">x</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-99'>
+  <div class='section' id='section-143'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-99'>#</a>
-      </div>
-      <hr />
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-100'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-100'>#</a>
+        <a class='octothorpe' href='#section-143'>#</a>
       </div>
-      <h2><span id="nested-linear-transition" href="nested-linear-transition"> Nested Linear Transition </span></h2>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-101'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-101'>#</a>
-      </div>
-      <p><strong><code>_lin_transition</code> private method of <code>PWL</code> class</strong></p>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_lin_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">n</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-102'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-102'>#</a>
-      </div>
-      <p>Private method to generate a linear transition. The difference between this method and the <a href="#linear-transition">public linear transition</a> method is that this method prints indented verbose output when called from within any of the public methods that revert to a linear transition in certain conditions.</p>
+      
     </div>
     <div class='code'>
-      <div class="highlight"><pre>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_nested_lin_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">n</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
             <span class="k">if</span> <span class="n">n</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">(</span>
-                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding linear transition with target of </span><span class="si">{</span><span class="n">target</span><span class="si">}</span><span class="s2"> and duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Adding linear transition with target of </span><span class="si">{</span><span class="n">target</span><span class="si">}</span><span class="s2"> and duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
             <span class="k">else</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">(</span>
-                    <span class="n">n</span><span class="o">*</span><span class="s2">&quot;    &quot;</span><span class="o">+</span><span class="sa">f</span><span class="s2">&quot;Adding linear transition with target of </span><span class="si">{</span><span class="n">target</span><span class="si">}</span><span class="s2"> and duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+                <span class="nb">print</span><span class="p">(</span><span class="n">n</span><span class="o">*</span><span class="s2">&quot;    &quot;</span><span class="o">+</span><span class="sa">f</span><span class="s2">&quot;Adding linear transition with target of </span><span class="si">{</span><span class="n">target</span><span class="si">}</span><span class="s2"> and duration of </span><span class="si">{</span><span class="n">duration</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">==</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">((</span><span class="n">n</span><span class="o">+</span><span class="mi">1</span><span class="p">)</span><span class="o">*</span><span class="s2">&quot;    &quot;</span><span class="o">+</span><span class="s2">&quot;Empty PWL object. Adding initial (0, 0) point.&quot;</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
+                <span class="nb">print</span><span class="p">((</span><span class="n">n</span><span class="o">+</span><span class="mi">1</span><span class="p">)</span><span class="o">*</span><span class="s2">&quot;    &quot;</span><span class="o">+</span><span class="s2">&quot;Empty PWL object. Adding initial (0, 0) point&quot;</span><span class="p">)</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
 
         <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-        <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-103'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-103'>#</a>
-      </div>
-      <hr />
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
+        <span class="bp">self</span><span class="o">.</span><span class="n">_insert</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-104'>
+  <div class='section' id='section-144'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-104'>#</a>
+        <a class='octothorpe' href='#section-144'>#</a>
       </div>
-      <h2><span id="exponential-function-generator" href="exponential-function-generator"> Exponential Function Generator </span></h2>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-105'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-105'>#</a>
-      </div>
-      <p><strong><code>_exp_transition_func</code> private function</strong></p>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre><span class="k">def</span> <span class="nf">_exp_transition_func</span><span class="p">(</span><span class="n">tau</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t2</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f2</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="nb">float</span><span class="p">],</span> <span class="nb">float</span><span class="p">]:</span></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-106'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-106'>#</a>
-      </div>
-      <p>Private function that generates an exponential function passing trough 2 fixed points.</p>
+      
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="n">A</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">f2</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span> <span class="o">/</span> \
-        <span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span>
+      <div class="highlight"><pre><span class="k">def</span> <span class="nf">exp_transition_func</span><span class="p">(</span><span class="n">tau</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t2</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f2</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="nb">float</span><span class="p">],</span> <span class="nb">float</span><span class="p">]:</span>
+    <span class="n">A</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">f2</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span> <span class="o">/</span> <span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span>
     <span class="n">B</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span> <span class="o">-</span> <span class="n">f2</span><span class="p">)</span><span class="o">/</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="o">-</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="o">-</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-107'>
+  <div class='section' id='section-145'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-107'>#</a>
+        <a class='octothorpe' href='#section-145'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">f</span><span class="p">(</span><span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
         <span class="n">result</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">A</span> <span class="o">+</span> <span class="n">B</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="o">-</span><span class="n">t</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">result</span>
 
     <span class="k">return</span> <span class="n">f</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-108'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-108'>#</a>
-      </div>
-      <hr />
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-109'>
+  <div class='section' id='section-146'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-109'>#</a>
+        <a class='octothorpe' href='#section-146'>#</a>
       </div>
-      <h2><span id="sinusoidal-function-generator" href="sinusoidal-function-generator"> Sinusoidal Function Generator </span></h2>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-110'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-110'>#</a>
-      </div>
-      <p><strong><code>_sin_transition_func</code> private function</strong></p>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre><span class="k">def</span> <span class="nf">_sin_transition_func</span><span class="p">(</span><span class="n">t1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t2</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f2</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="nb">float</span><span class="p">],</span> <span class="nb">float</span><span class="p">]:</span></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-111'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-111'>#</a>
-      </div>
-      <p>Private function that generates a sinusoidal function passing trough 2 fixed points.</p>
+      
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="n">fm</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span><span class="o">+</span><span class="n">f2</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span>
+      <div class="highlight"><pre><span class="k">def</span> <span class="nf">sin_transition_func</span><span class="p">(</span><span class="n">t1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t2</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f2</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="nb">float</span><span class="p">],</span> <span class="nb">float</span><span class="p">]:</span>
+    <span class="n">fm</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span><span class="o">+</span><span class="n">f2</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span>
     <span class="n">tm</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">t1</span><span class="o">+</span><span class="n">t2</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span>
     <span class="n">T</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">2</span><span class="o">*</span><span class="p">(</span><span class="n">t2</span><span class="o">-</span><span class="n">t1</span><span class="p">)</span>
     <span class="n">w</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">2</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">pi</span><span class="o">/</span><span class="n">T</span>
     <span class="n">phi</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">w</span><span class="o">*</span><span class="n">tm</span>
     <span class="n">A</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">f2</span><span class="o">-</span><span class="n">fm</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-112'>
+  <div class='section' id='section-147'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-112'>#</a>
+        <a class='octothorpe' href='#section-147'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">f</span><span class="p">(</span><span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
         <span class="n">result</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">fm</span> <span class="o">+</span> <span class="n">A</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">sin</span><span class="p">(</span><span class="n">w</span><span class="o">*</span><span class="n">t</span> <span class="o">-</span> <span class="n">phi</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">result</span>
 
     <span class="k">return</span> <span class="n">f</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-113'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-113'>#</a>
-      </div>
-      <hr />
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-114'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-114'>#</a>
-      </div>
-      <h2><span id="smoothstep-function-generator" href="smoothstep-function-generator"> Smoothstep Function Generator </span></h2>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-115'>
+  <div class='section' id='section-148'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-115'>#</a>
+        <a class='octothorpe' href='#section-148'>#</a>
       </div>
-      <p><strong><code>_smoothstep_transition_func</code> private function</strong></p>
-    </div>
-    <div class='code'>
-      <div class="highlight"><pre><span class="k">def</span> <span class="nf">_smoothstep_transition_func</span><span class="p">(</span><span class="n">t1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t2</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f2</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="nb">float</span><span class="p">],</span> <span class="nb">float</span><span class="p">]:</span></pre></div>
-    </div>
-  </div>
-  <div class='clearall'></div>
-  <div class='section' id='section-116'>
-    <div class='docs'>
-      <div class='octowrap'>
-        <a class='octothorpe' href='#section-116'>#</a>
-      </div>
-      <p>Private function that generates a smoothstep function passing trough 2 fixed points.</p>
+      
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="n">Am</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">([[</span><span class="mi">1</span><span class="p">,</span> <span class="n">t1</span><span class="p">,</span> <span class="n">t1</span><span class="o">**</span><span class="mi">2</span><span class="p">,</span> <span class="n">t1</span><span class="o">**</span><span class="mi">3</span><span class="p">],</span>
+      <div class="highlight"><pre><span class="k">def</span> <span class="nf">smoothstep_transition_func</span><span class="p">(</span><span class="n">t1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t2</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f2</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="nb">float</span><span class="p">],</span> <span class="nb">float</span><span class="p">]:</span>
+    <span class="n">Am</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">([[</span><span class="mi">1</span><span class="p">,</span> <span class="n">t1</span><span class="p">,</span> <span class="n">t1</span><span class="o">**</span><span class="mi">2</span><span class="p">,</span> <span class="n">t1</span><span class="o">**</span><span class="mi">3</span><span class="p">],</span>
                    <span class="p">[</span><span class="mi">1</span><span class="p">,</span> <span class="n">t2</span><span class="p">,</span> <span class="n">t2</span><span class="o">**</span><span class="mi">2</span><span class="p">,</span> <span class="n">t2</span><span class="o">**</span><span class="mi">3</span><span class="p">],</span>
                    <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="o">*</span><span class="n">t1</span><span class="p">,</span> <span class="mi">3</span><span class="o">*</span><span class="n">t1</span><span class="o">**</span><span class="mi">2</span><span class="p">],</span>
                    <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="o">*</span><span class="n">t2</span><span class="p">,</span> <span class="mi">3</span><span class="o">*</span><span class="n">t2</span><span class="o">**</span><span class="mi">2</span><span class="p">]])</span>
     <span class="n">Bm</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">([</span><span class="n">f1</span><span class="p">,</span> <span class="n">f2</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">])</span>
     <span class="n">A</span><span class="p">,</span> <span class="n">B</span><span class="p">,</span> <span class="n">C</span><span class="p">,</span> <span class="n">D</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">linalg</span><span class="o">.</span><span class="n">solve</span><span class="p">(</span><span class="n">Am</span><span class="p">,</span> <span class="n">Bm</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-117'>
+  <div class='section' id='section-149'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-117'>#</a>
+        <a class='octothorpe' href='#section-149'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">f</span><span class="p">(</span><span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
         <span class="n">result</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">A</span> <span class="o">+</span> <span class="n">B</span><span class="o">*</span><span class="n">t</span> <span class="o">+</span> <span class="n">C</span><span class="o">*</span><span class="n">t</span><span class="o">**</span><span class="mi">2</span> <span class="o">+</span> <span class="n">D</span><span class="o">*</span><span class="n">t</span><span class="o">**</span><span class="mi">3</span>
         <span class="k">return</span> <span class="n">result</span>
 
     <span class="k">return</span> <span class="n">f</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-118'>
+  <div class='section' id='section-150'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-118'>#</a>
+        <a class='octothorpe' href='#section-150'>#</a>
       </div>
-      <hr />
+      
     </div>
     <div class='code'>
-      <div class="highlight"><pre><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-    <span class="n">pwl0</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="mf">0.001</span><span class="p">)</span>
-    <span class="n">pwl1</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="mf">0.001</span><span class="p">)</span>
-
-    <span class="n">pwl0</span><span class="o">.</span><span class="n">hold</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
-    <span class="n">pwl1</span><span class="o">.</span><span class="n">hold</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
-
-    <span class="n">pwl0</span><span class="o">.</span><span class="n">sin_transition</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
-    <span class="n">pwl1</span><span class="o">.</span><span class="n">sin_transition</span><span class="p">(</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
+      <div class="highlight"><pre><span class="k">def</span> <span class="nf">is_within</span><span class="p">(</span><span class="n">x</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">y</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">tol</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.01</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+    <span class="n">error</span> <span class="o">=</span> <span class="mi">0</span> <span class="k">if</span> <span class="n">x</span> <span class="o">==</span> <span class="n">y</span> <span class="k">else</span> <span class="mi">2</span><span class="o">*</span><span class="nb">abs</span><span class="p">(</span><span class="n">x</span><span class="o">-</span><span class="n">y</span><span class="p">)</span><span class="o">/</span><span class="p">(</span><span class="nb">abs</span><span class="p">(</span><span class="n">x</span><span class="p">)</span><span class="o">+</span><span class="nb">abs</span><span class="p">(</span><span class="n">y</span><span class="p">))</span>
 
-    <span class="n">pwl0</span><span class="o">.</span><span class="n">hold</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
-    <span class="n">pwl1</span><span class="o">.</span><span class="n">hold</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
+    <span class="k">return</span> <span class="n">error</span> <span class="o">&lt;=</span> <span class="n">tol</span>
 
-    <span class="n">pwl0</span><span class="o">.</span><span class="n">sin_transition</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
 
-    <span class="n">pwl1</span><span class="o">.</span><span class="n">plot_flag</span> <span class="o">=</span> <span class="kc">False</span>
+<span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+    <span class="n">t</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="mf">0.01</span><span class="p">,</span> <span class="n">name</span><span class="o">=</span><span class="s2">&quot;t&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">lin_transition</span><span class="p">(</span><span class="mi">10</span><span class="p">,</span> <span class="mi">10</span><span class="p">)</span>
+    <span class="n">x</span> <span class="o">=</span> <span class="o">-</span><span class="p">(</span><span class="mi">1</span><span class="o">/</span><span class="mi">3</span><span class="p">)</span><span class="o">*</span><span class="p">(</span><span class="n">t</span><span class="o">**</span><span class="mi">3</span><span class="p">)</span><span class="o">+</span><span class="mi">5</span><span class="o">*</span><span class="p">(</span><span class="n">t</span><span class="o">**</span><span class="mi">2</span><span class="p">)</span><span class="o">-</span><span class="mi">15</span><span class="o">*</span><span class="n">t</span>
+    <span class="n">x</span><span class="o">.</span><span class="n">name</span> <span class="o">=</span> <span class="s2">&quot;x&quot;</span>
 
-    <span class="n">PWL</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">merge</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-    <span class="nb">print</span><span class="p">(</span><span class="n">pwl0</span><span class="p">(</span><span class="mf">1.5</span><span class="p">))</span>
+    <span class="n">PWL</span><span class="o">.</span><span class="n">plot</span><span class="p">()</span>
 
 </pre></div>
     </div>
   </div>
   <div class='clearall'></div>
 </div>
 </body>
```

#### html2text {}

```diff
@@ -8,46 +8,51 @@
     * python 3.11.1
           o numpy 1.25.0
           o matplotlib 3.7.1
 Type stubs for older numpy versions for mypy checking can be found here.
 ===============================================================================
 ****** Index ******
     * Package_Summary
-    * Precision_Related_Exception
     * PWL_Class
           o Dunder Methods
                 # Initializer
                 # String_Representation
                 # Length_Calculator
-                # Object_as_a_Callable
+                # Object_Calling
+                # Object_Slicing
+                # Object_Iteration
+          o Mathematical Unary Operators
+                # Additive_Inverse
+                # Absolute_Value
+          o Mathematical Binary Operators
+                # Addition
+                # Subtraction
+                # Multiplication
+                # Division
+                # Exponentiation
           o Properties
                 # Time_Coordinates
                 # Dependent_Coordinates
                 # Default_Timestep
                 # Name
                 # Verbose_Flag
                 # Plot_Enable_Flag (optional feature: requires matplotlib)
-          o Methods
+          o Instance Methods
+                # Initial_Condition
                 # Last_Value_Holder
                 # Linear_Transition
                 # Rectangular_Pulse
                 # Sawtooth_Pulse
                 # Exponential_Transition
                 # Half_Sine_Transition
                 # Smoothstep_Transition
-                # PWL_File_Writer
+                # File_Writer
+                # Object_Copy
+          o Class Methods
                 # PWL_Plotter (optional feature: requires matplotlib)
-          o Private Methods (minimal documentation)
-                # PWL_Point_Adder
-                # Colinear_Points_Eliminator
-                # Nested_Linear_Transition
-    * Private Functions (minimal documentation)
-          o Exponential_Function_Generator
-          o Sinusoidal_Function_Generator
-          o Smoothstep_Function_Generator
 ===============================================================================
 ****** Package Summary ******
 This package defines a class PWL to generate objects that represent time
 dependent signals x(t) that need to be coded in a PWL file. Those objects are
 built using little components such as rectangular pulses and sawtooth pulses
 that can be chained together.
 The motivations for this package are the nuisances of writing PWL files by
@@ -94,58 +99,70 @@
 create a PWL object for each control signal and define 3 functions that apply
 all the needed values for the control signals for each state. If we nedded the
 system to be at mode 1 for 3 seconds, idle for 1 second and at mode 2 for 5
 seconds, we could write something like the following:
    mode1_state(3)
    idle_state(1)
    mode2_state(5)
-__all__ = ['PrecisionError', 'PWL']
+__all__ = ['PWL']
 
-from warnings import warn
+import warnings
 from numbers import Real
-from typing import Callable, Dict, List, Optional
+from typing import Callable, List, Optional, TYPE_CHECKING, Union, Tuple,
+Iterator, TypeVar, Any, cast
+import weakref
 import numpy as np
 
+
 try:
     import matplotlib.pyplot as plt  # type: ignore
 except ImportError:
     _has_matplotlib = False
-    warn("Matplotlib package not found. Optional plotting features
+    warnings.warn("Matplotlib package not found. Optional plotting features
 deactivated.", ImportWarning)
 else:
     _has_matplotlib = True
+
+if TYPE_CHECKING:
+    WeakDict = weakref.WeakValueDictionary[str, "PWL"]
+
+TFun = TypeVar("TFun", bound=Callable[..., Any])
 #
-===============================================================================
+class copy_doc:
+#
+    def __init__(self, copy_func: TFun) -> None:
+        self.copy_func = copy_func
 #
-***** Precision Related Exception *****
+    def __call__(self, func: TFun) -> TFun:
+        func.__doc__ = self.copy_func.__doc__
+        return func
 #
-PrecisionError exception class
 class PrecisionError(Exception):
+    pass
 #
-This class defines an exception meant to be raised when any type of rounding or
-loss of precision that causes the time coordinates of a PWL object to not be
-strictly increasing.
+class InitialConditionError(Exception):
+    pass
 #
 ===============================================================================
 #
 ***** PWL Class *****
 #
 PWL class
 class PWL():
 #
 This class defines an object that represnts a time dependent signal x(t). Those
 objects can operated on by methods to build, event by event, the desired signal
 as described on the package introduction.
-    __dict_of_objects: Dict[str, 'PWL'] = {}
+    __dict_of_objects = weakref.WeakValueDictionary()  # type: WeakDict
 #
 ===============================================================================
 #
 ***** Initializer *****
 #
-Dunder method __init__ of PWL class
+__init__ dunder method of PWL class
     def __init__(self, t_step: float, name: Optional[str] = None, verbose: bool
 = False) -> None:
 #
 **** Summary ****
 Initializer for the PWL class.
 **** Arguments ****
     * t_step (float) : Default timestep for all operations. Should be strictly
@@ -154,58 +171,55 @@
       printing. Should not be empty. If not set, automatically generates a name
       based on already taken names.
     * verbose (bool, optional) : Flag indicating if verbose output should be
       printed. If not set, defaults to False.
 **** Raises ****
     * TypeError : Raised if either t_step is not a real number, name is not a
       string or verbose is not a boolean.
-    * ValueError : Raised if t_step is not strictly positive or name is empty.
+    * ValueError : Raised if t_step is not strictly positive or name is either
+      empty or already taken.
         if name is None:
             i: int = 0
-            while f"pwl_{i}" in PWL.__dict_of_objects:
+            while f"pwl_{i}" in PWL.__dict_of_objects.keys():
                 i += 1
             name = f"pwl_{i}"
 
         if not isinstance(t_step, Real):
-            raise TypeError(
-                f"Argument 't_step' should be a real number but has type '{type
-(t_step).__name__}'.")
+            raise TypeError(f"Argument 't_step' should be a real number but has
+type '{type(t_step).__name__}'")
         if not isinstance(name, str):
-            raise TypeError(
-                f"Argument 'name' should either be a string but has type '{type
-(name).__name__}'.")
+            raise TypeError(f"Argument 'name' should either be a string but has
+type '{type(name).__name__}'")
         if not isinstance(verbose, bool):
-            raise TypeError(
-                f"Argument 'verbose' should be a boolean but has type '{type
-(verbose).__name__}'.")
+            raise TypeError(f"Argument 'verbose' should be a boolean but has
+type '{type(verbose).__name__}'")
 
         if t_step <= 0:
-            raise ValueError(
-                f"Argument 't_step' should be strictly positive but has value
-of {t_step}.")
+            raise ValueError(f"Argument 't_step' should be strictly positive
+but has value of {t_step}")
         if not name:
-            raise ValueError("Argument 'name' should not be empty.")
+            raise ValueError("Argument 'name' should not be empty")
 
         self._t_list: List[float] = []
         self._x_list: List[float] = []
         self._t_step: float = t_step
         self._name: str = name
         self._verbose: bool = verbose
         self._plot_flag: bool = True
 
-        if name in PWL. __dict_of_objects:
-            raise ValueError(f"Name '{name}' already in use.")
+        if name in PWL.__dict_of_objects.keys():
+            raise ValueError(f"Name '{name}' already in use")
 
-        PWL. __dict_of_objects[name] = self
+        PWL.__dict_of_objects[name] = self
 #
 ===============================================================================
 #
 ***** String Representation *****
 #
-Dunder method __str__ of PWL class
+__str__ dunder method of PWL class
     def __str__(self) -> str:
 #
 **** Summary ****
 String representation of PWL instances in the form [name]: PWL object with [#
 of points] and duration of [total time duration] seconds.
 **** Returns ****
     * str
@@ -214,66 +228,461 @@
         return f"{self.name}: PWL object with {len(self._t_list)} points and
 duration of {duration} seconds"
 #
 ===============================================================================
 #
 ***** Length Calculator *****
 #
-Dunder method __len__ of PWL class
+__len__ dunder method of PWL class
     def __len__(self) -> int:
 #
 **** Summary ****
 Length of PWL instances defined as the number of (t, x) points they contain.
 **** Returns ****
     * int
         return len(self._t_list)
 #
 ===============================================================================
 #
-***** Object as a Callable *****
+***** Object Calling *****
 #
-Dunder method __call__ of PWL class
+__call__ dunder method of PWL class
     def __call__(self, t: float) -> float:
 #
 **** Summary ****
 Call PWL object as a function by linearly interpolating between it’s time and
 dependent coordinates.
 **** Arguments ****
     * t (float) : Time instant to evaluate the object at. If negative, returns
       zero. If bigger than the duration of the object, returns the object’s
       last dependent coordinate.
 **** Returns ****
     * float
 **** Raises ****
     * TypeError : Raised if t is not a real number.
         if not isinstance(t, Real):
-            raise TypeError(
-                f"Argument 't' should be a real number but has type '{type
-(t).__name__}'.")
+            raise TypeError(f"Argument 't' should be a real number but has type
+'{type(t).__name__}'")
 
         t_list = self._t_list
         x_list = self._x_list
 
         return np.interp(x=t, xp=t_list, fp=x_list, left=0)
 #
 ===============================================================================
 #
+***** Object Slicing *****
+#
+__getitem__ dunder method of PWL class
+    def __getitem__(self, index: Union[int, slice]) -> Union[Tuple[float,
+float], List[Tuple[float, float]]]:
+#
+**** Summary ****
+Slice PWL objects.
+**** Arguments ****
+    * index (int or slice) : Index for list of (t, x) points.
+**** Returns ****
+    * Tuple[float, float] : Returned if single index is passed.
+    * List[Tuple[float, float]] : Rerturned if multiple indices are passed.
+**** Raises ****
+    * TypeError : Raised if index is not an integer or slice.
+    * IndexError : Raised if index is out of bounds.
+        if not isinstance(index, (int, slice)):
+            raise TypeError(f"PWL indices must be integers or slices, not {type
+(index).__name__}")
+
+        coordinates_pair = list(zip(self.t_list, self.x_list))
+
+        return coordinates_pair[index]
+#
+===============================================================================
+#
+***** Object Iteration *****
+#
+__iter__ dunder method of PWL class
+    def __iter__(self) -> Iterator[Tuple[float, float]]:
+#
+**** Summary ****
+Creates a generator object that yields all the (t, x) points as tuples.
+**** Yields ****
+    * Tuple[float, float]
+        yield from list(zip(self.t_list, self.x_list))
+#
+===============================================================================
+#
+***** Additive Inverse *****
+#
+__neg__ dunder method of PWL class
+    def __neg__(self) -> "PWL":
+#
+**** Summary ****
+Implements point-wise additive inversion (multiplying by -1).
+The new PWL objects created has t_step equal to the operand’s t_step.
+**** Arguments ****
+    * Operand (PWL or float) : Thing being additivly inverted.
+**** Returns ****
+    * PWL : The additive inverse of the operand.
+**** See Also ****
+    * Multiplication
+        return -1*self
+#
+    def __pos__(self) -> "PWL":
+        return self.copy()
+#
+===============================================================================
+#
+***** Absolute Value *****
+#
+__abs__ dunder method of PWL class
+    def __abs__(self) -> "PWL":
+#
+**** Summary ****
+Implements point-wise absolute value operation.
+The new PWL objects created has t_step equal to the operand’s t_step.
+**** Arguments ****
+    * Operand (PWL or float) : Thing whose absolute value is being taken.
+**** Returns ****
+    * PWL : The absolute value of the operand.
+        new_pwl = PWL(t_step=self.t_step)
+
+        for t, x in self:
+            new_x = cast(float, np.absolute(x))
+            new_pwl._insert(t, new_x)
+
+        return new_pwl
+#
+===============================================================================
+#
+***** Addition *****
+#
+__add__ and __radd__ dunder methods of PWL class
+    def __add__(self, other: Union["PWL", float]) -> "PWL":
+#
+**** Summary ****
+Implements point-wise addition of PWL objects with real numbers and other PWL
+objects.
+The new PWL objects created has t_step equal to the lower t_step between the
+operands.
+If one operand is longer than the other, extends the shorter one by holding
+it’s last value.
+**** Arguments ****
+    * Addends (PWL or float) : Things being added together.
+**** Returns ****
+    * PWL : The sum of the addends.
+**** Raises ****
+    * TypeError : Raised if operation is not implemented between the operands.
+        if not isinstance(other, (Real, PWL)):
+            return NotImplemented
+
+        t_step = min(self.t_step, other.t_step) if isinstance(other, PWL) else
+self.t_step
+        new_pwl = PWL(t_step=t_step)
+
+        if isinstance(other, Real):
+            other_copy = float(other)
+            other = lambda *args, **kwargs: other_copy
+
+        unsorted_t_set = set(self.t_list + other.t_list)
+        t_list = sorted(list(unsorted_t_set))
+        for t in t_list:
+            new_pwl._insert(t, self(t) + other(t))
+
+        return new_pwl
+#
+    @copy_doc(__add__)
+    def __radd__(self, other: float) -> "PWL":
+        return self + other
+#
+===============================================================================
+#
+***** Subtraction *****
+#
+__sub__ and __rsub__ dunder methods of PWL class
+    def __sub__(self, other: Union["PWL", float]) -> "PWL":
+#
+**** Summary ****
+Implements point-wise subtraction of PWL objects with real numbers and other
+PWL objects.
+The new PWL objects created has t_step equal to the lower t_step between the
+operands.
+If one operand is longer than the other, extends the shorter one by holding
+it’s last value.
+**** Arguments ****
+    * Minuend (PWL or float) : Thing from which we subtract the subtrahend.
+    * Subtrahend (PWL or float) : Thing being subtracted from the minuend.
+**** Returns ****
+    * PWL : The difference of the minuend an subtrahend.
+**** Raises ****
+    * TypeError : Raised if operation is not implemented between the operands.
+        if not isinstance(other, (Real, PWL)):
+            return NotImplemented
+
+        t_step = min(self.t_step, other.t_step) if isinstance(other, PWL) else
+self.t_step
+        new_pwl = PWL(t_step=t_step)
+
+        if isinstance(other, Real):
+            other_copy = float(other)
+            other = lambda *args, **kwargs: other_copy
+
+        unsorted_t_set = set(self.t_list + other.t_list)
+        t_list = sorted(list(unsorted_t_set))
+        for t in t_list:
+            new_pwl._insert(t, self(t) - other(t))
+
+        return new_pwl
+#
+    @copy_doc(__sub__)
+    def __rsub__(self, other: float) -> "PWL":
+        t_step = self.t_step
+        new_pwl = PWL(t_step=t_step)
+
+        for t, x in self:
+            new_pwl._insert(t, other-x)
+
+        return new_pwl
+#
+===============================================================================
+#
+***** Multiplication *****
+#
+__mul__ and __rmul__ dunder methods of PWL class
+    def __mul__(self, other: Union["PWL", float]) -> "PWL":
+#
+**** Summary ****
+Implements point-wise multiplication of PWL objects with real numbers and other
+PWL objects.
+The new PWL objects created has t_step equal to the lower t_step between the
+operands.
+If one operand is longer than the other, extends the shorter one by holding
+it’s last value.
+**** Arguments ****
+    * Factors (PWL or float) : Things being multiplied together.
+**** Returns ****
+    * PWL : The product of the factors.
+**** Raises ****
+    * TypeError : Raised if operation is not implemented between the operands.
+        if not isinstance(other, (Real, PWL)):
+            return NotImplemented
+
+        t_step = min(self.t_step, other.t_step) if isinstance(other, PWL) else
+self.t_step
+        t_max = max(self.t_list[-1], other._t_list[-1]) if isinstance(other,
+PWL) else self._t_list[-1]
+        x_last = np.multiply(self(t_max), other(t_max)) if isinstance(other,
+PWL) else np.multiply(self(t_max), cast(float, other))
+        t_list = np.arange(0, t_max, t_step)
+
+        new_pwl = PWL(t_step=t_step)
+
+        if isinstance(other, Real):
+            other_copy = float(other)
+            other = lambda *args, **kwargs: other_copy
+
+        for t in t_list:
+            new_x = cast(float, np.multiply(self(t), other(t)))
+            new_pwl._insert(t, new_x)
+
+        if t_max > new_pwl._t_list[-1]:
+            new_x = cast(float, x_last)
+            new_pwl._insert(t_max, new_x)
+
+        return new_pwl
+#
+    @copy_doc(__mul__)
+    def __rmul__(self, other: float) -> "PWL":
+        return self * other
+#
+===============================================================================
+#
+***** Division *****
+#
+__truediv__ and __rtruediv__ dunder methods of PWL class
+    def __truediv__(self, other: Union["PWL", float]) -> "PWL":
+#
+**** Summary ****
+Implements point-wise division of PWL objects with real numbers and other PWL
+objects.
+The new PWL objects created has t_step equal to the lower t_step between the
+operands.
+If one operand is longer than the other, extends the shorter one by holding
+it’s last value.
+**** Arguments ****
+    * Numerator (PWL or float) : Thing being divided by the denominator.
+    * Denominator (PWL or float) : Thing that the numerator is being divided
+      by.
+**** Returns ****
+    * PWL : The ratio of the numerator and denominator.
+**** Raises ****
+    * TypeError : Raised if operation is not implemented between the operands.
+    * ZeroDivisionError : Raised if the denominator contains the point (t, 0)
+      for any t.
+        if not isinstance(other, (Real, PWL)):
+            return NotImplemented
+
+        t_step = min(self.t_step, other.t_step) if isinstance(other, PWL) else
+self.t_step
+        t_max = max(self.t_list[-1], other._t_list[-1]) if isinstance(other,
+PWL) else self._t_list[-1]
+        x_last = np.multiply(self(t_max), other(t_max)) if isinstance(other,
+PWL) else np.true_divide(self(t_max), cast(float, other))
+        t_list = np.arange(0, t_max, t_step)
+
+        new_pwl = PWL(t_step=t_step)
+
+        if isinstance(other, Real):
+            other_copy = float(other)
+            other = lambda *args, **kwargs: other_copy
+
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore')
+            for t in t_list:
+                left_x = cast(float, np.true_divide(self(t-t_step/2), other(t-
+t_step/2)))
+                center_x = cast(float, np.true_divide(self(t), other(t)))
+                rigth_x = cast(float, np.true_divide(self(t+t_step/2), other
+(t+t_step/2)))
+
+                if np.isfinite(center_x):
+                    new_pwl._insert(t, center_x)
+                elif np.isfinite(left_x) and np.isfinite(rigth_x):
+                    new_pwl._insert(t, (left_x+rigth_x)/2)
+                elif np.isfinite(left_x):
+                    new_pwl._insert(t, left_x)
+                elif np.isfinite(rigth_x):
+                    new_pwl._insert(t, rigth_x)
+                else:
+                    new_pwl._insert(t, 0)
+
+        if t_max > new_pwl._t_list[-1]:
+            new_pwl._insert(t_max, cast(float, x_last))
+
+        return new_pwl
+#
+    @copy_doc(__truediv__)
+    def __rtruediv__(self, other: float) -> "PWL":
+        if not isinstance(other, Real):
+            return NotImplemented
+
+        t_step = self.t_step
+        t_max = self._t_list[-1]
+        t_list = np.arange(0, t_max, t_step)
+        x_last = np.true_divide(other, self(t_max))
+
+        new_pwl = PWL(t_step=t_step)
+
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore')
+            for t in t_list:
+                left_x = cast(float, np.true_divide(other, self(t-t_step/2)))
+                center_x = cast(float, np.true_divide(other, self(t)))
+                rigth_x = cast(float, np.true_divide(other, self(t+t_step/2)))
+
+                if np.isfinite(center_x):
+                    new_pwl._insert(t, center_x)
+                elif np.isfinite(left_x) and np.isfinite(rigth_x):
+                    new_pwl._insert(t, (left_x+rigth_x)/2)
+                elif np.isfinite(left_x):
+                    new_pwl._insert(t, left_x)
+                elif np.isfinite(rigth_x):
+                    new_pwl._insert(t, rigth_x)
+                else:
+                    new_pwl._insert(t, 0)
+
+        if t_max > new_pwl._t_list[-1]:
+            new_pwl._insert(t_max, x_last)
+
+        return new_pwl
+#
+===============================================================================
+#
+***** Exponentiation *****
+#
+__pow__ and __rpow__ dunder methods of PWL class
+    def __pow__(self, other: Union["PWL", float]) -> "PWL":
+#
+**** Summary ****
+Implements point-wise exponentiation of PWL objects with real numbers and other
+PWL objects.
+If the result of the exponentiation ends up being a complex number, returns the
+real part of it.
+The new PWL objects created has t_step equal to the lower t_step between the
+operands.
+If one operand is longer than the other, extends the shorter one by holding
+it’s last value.
+**** Arguments ****
+    * Base (PWL or float) : Thing being raised to the exponent.
+    * Exponent (PWL or float) : Thing to raise the base to.
+**** Returns ****
+    * PWL : The power with the given base and exponent.
+**** Raises ****
+    * TypeError : Raised if operation is not implemented between the operands.
+        if not isinstance(other, (Real, PWL)):
+            return NotImplemented
+
+        t_step = min(self.t_step, other.t_step) if isinstance(other, PWL) else
+self.t_step
+        t_max = max(self.t_list[-1], other.t_list[-1]) if isinstance(other,
+PWL) else self.t_list[-1]
+        x_last = np.multiply(self(t_max), other(t_max)) if isinstance(other,
+PWL) else cast(float, np.power(self(t_max), cast(float, other),
+dtype=complex).real)
+        t_list = np.arange(0, t_max, t_step)
+
+        new_pwl = PWL(t_step=t_step)
+
+        if isinstance(other, Real):
+            other_copy = float(other)
+            other = lambda *args, **kwargs: other_copy
+
+        for t in t_list:
+            new_x = cast(float, np.power(self(t), other(t),
+dtype=complex).real)
+            new_pwl._insert(t, new_x)
+
+        if t_max > new_pwl._t_list[-1]:
+            new_pwl._insert(t_max, cast(float, x_last))
+
+        return new_pwl
+#
+    @copy_doc(__pow__)
+    def __rpow__(self, other: float) -> "PWL":
+        if not isinstance(other, Real):
+            return NotImplemented
+
+        t_step = self.t_step
+        t_max = self.t_list[-1]
+        x_last = np.power(self(t_max), other, dtype=complex).real
+        t_list = np.arange(0, t_max, t_step)
+
+        new_pwl = PWL(t_step=t_step)
+
+        for t in t_list:
+            new_pwl._insert(t, np.power(other, self(t), dtype=complex).real)
+
+        if t_max > new_pwl._t_list[-1]:
+            new_pwl._insert(t_max, x_last)
+
+        return new_pwl
+#
+===============================================================================
+#
 ***** Time Coordinates *****
 #
 t_list property of PWL class
     @property
     def t_list(self) -> List[float]:
 #
 **** Type ****
     * list[float]
 **** Summary ****
 Read only property containing all the time coordinates of a PWL object.
 **** Raises ****
     * AttributeError : Raised if assignment was attempetd.
-        return self._t_list
+        return self._t_list[:]
 #
 ===============================================================================
 #
 ***** Dependent Coordinates *****
 #
 x_list property of PWL class
     @property
@@ -281,15 +690,15 @@
 #
 **** Type ****
     * list[float]
 **** Summary ****
 Read only property containing all the dependent coordinates of a PWL object.
 **** Raises ****
     * AttributeError : Raised if assignment was attempetd.
-        return self._x_list
+        return self._x_list[:]
 #
 ===============================================================================
 #
 ***** Default Timestep *****
 #
 t_step property of PWL class
     @property
@@ -303,21 +712,19 @@
     * TypeError : Raised if the assigned value is not a real number.
     * ValueError : Raised if the assigned value is not strictly positive.
         return self._t_step
 #
     @t_step.setter
     def t_step(self, new_t_step: float) -> None:
         if not isinstance(new_t_step, float):
-            raise TypeError(
-                f"Property 't_step' should be a real number but an object of
-type '{type(new_t_step).__name__}' was assigned to it.")
+            raise TypeError(f"Property 't_step' should be a real number but an
+object of type '{type(new_t_step).__name__}' was assigned to it")
         if new_t_step <= 0:
-            raise ValueError(
-                f"Propety 't_step' should be strictly positive but a value of
-{new_t_step} was assigned to it.")
+            raise ValueError(f"Propety 't_step' should be strictly positive but
+a value of {new_t_step} was assigned to it")
 
         self._t_step = new_t_step
 #
 ===============================================================================
 #
 ***** Name *****
 #
@@ -334,26 +741,25 @@
     * ValueError : Raised if the assigned value is an empty string or already
       in use.
         return self._name
 #
     @name.setter
     def name(self, new_name: str) -> None:
         if not isinstance(new_name, str):
-            raise TypeError(
-                f"Property 'name' should be a string but an object of type '
-{type(new_name).__name__}' was assigned to it.")
+            raise TypeError(f"Property 'name' should be a string but an object
+of type '{type(new_name).__name__}' was assigned to it")
         if not new_name:
-            raise ValueError(
-                "An empty string cannot be assigned to the 'name' property.")
+            raise ValueError("An empty string cannot be assigned to the 'name'
+property")
 
-        if new_name in PWL. __dict_of_objects:
-            raise ValueError(f"Name '{new_name}' already in use.")
+        if new_name in PWL.__dict_of_objects.keys():
+            raise ValueError(f"Name '{new_name}' already in use")
 
-        PWL. __dict_of_objects.pop(self._name)
-        PWL. __dict_of_objects[new_name] = self
+        PWL.__dict_of_objects.pop(self._name)
+        PWL.__dict_of_objects[new_name] = self
         self._name = new_name
 #
 ===============================================================================
 #
 ***** Verbose Flag *****
 #
 verbose property of PWL class
@@ -368,17 +774,16 @@
     * TypeError : Raised if the assigned value is not a boolean.
         return self._verbose
 #
     @verbose.setter
     def verbose(self, new_verbose: bool) -> None:
 
         if not isinstance(new_verbose, bool):
-            raise TypeError(
-                f"Attribute 'verbose' should be a boolean but an object of type
-'{type(new_verbose).__name__}' was assigned to it.")
+            raise TypeError(f"Attribute 'verbose' should be a boolean but an
+object of type '{type(new_verbose).__name__}' was assigned to it")
         self._verbose = new_verbose
 #
 ===============================================================================
 #
 ***** Plot Enable Flag *****
 #
 plot_flag property of PWL class
@@ -391,272 +796,295 @@
 **** Summary ****
 Property defining if object should be plotted by the PWL plotter method.
 **** Raises ****
     * TypeError : Raised if the assigned value is not a boolean.
 **** See Also ****
     * PWL_Plotter
         if (not _has_matplotlib) and self._verbose:
-            print(
-                "Optional features deactivated. Using the plot_flag does
-nothing in this case.")
+            print("Optional features deactivated. Using the plot_flag does
+nothing in this case")
 
         return self._plot_flag
 #
     @plot_flag.setter
     def plot_flag(self, new_plot_flag: bool) -> None:
 
         if not isinstance(new_plot_flag, bool):
-            raise TypeError(
-                f"Attribute 'plot_flag' should be a boolean but an object of
-type '{type(new_plot_flag).__name__}' was assigned to it.")
+            raise TypeError(f"Attribute 'plot_flag' should be a boolean but an
+object of type '{type(new_plot_flag).__name__}' was assigned to it")
 
         if (not _has_matplotlib) and self._verbose:
-            print(
-                "Optional features deactivated. Using the plot_flag does
-nothing in this case.")
+            print("Optional features deactivated. Using the plot_flag does
+nothing in this case")
 
         self._plot_flag = new_plot_flag
 #
 ===============================================================================
 #
+***** Initial Condition *****
+#
+initial method of PWL class
+    def initial(self, x0: float = 0) -> "PWL":
+#
+**** Summary ****
+Method that sets the initial condition for the PWL object.
+**** Parameters ****
+    * x0 (float, optional) : Initial condition for t=0.
+**** Returns ****
+    * PWL : Returns the object itself.
+**** Raises ****
+    * TypeError : Raised if x0 is not a real number.increasing.
+    * InitialConditionError : Raised if the object already has initial
+      conditions.
+        if not isinstance(x0, Real):
+            raise TypeError(f"Argument 'x0' should be a real number but has
+type '{type(x0).__name__}'")
+        if len(self) != 0:
+            raise InitialConditionError(f"PWL object already has initial
+condition of {self.x_list[0]}")
+
+        self._insert(0, x0)
+
+        return self
+#
+===============================================================================
+#
 ***** Last Value Holder *****
 #
 hold method of PWL class
-    def hold(self, duration: float) -> None:
+    def hold(self, duration: float) -> "PWL":
 #
 **** Summary ****
 Method that holds the last value from the previous event for a given duration.
 If the PWL object is empty, adds the point (0, 0) and holds that.
 **** Parameters ****
     * duration (float) : Duration to hold the last value for. Should be
       strictly positive.
+**** Returns ****
+    * PWL : Returns the object itself.
 **** Raises ****
     * TypeError : Raised if duration is not a real number.
     * ValueError : Raised if duration is not strictly positive.
     * PrecisionError : Raised if computational noise causes the time
       coordinates to not be strictly increasing.
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '
-{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but
+has type '{type(duration).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value
-of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive
+but has value of {duration}")
 
         if self._verbose:
-            print(f"{self._name}: Adding hold with duration of {duration}.")
+            print(f"{self._name}: Adding hold with duration of {duration}")
 
         if len(self._t_list) == len(self._x_list) == 0:
             if self._verbose:
-                print("    Empty PWL object. Adding initial (0, 0) point.")
-            self._add(0, 0)
+                print("    Empty PWL object. Adding initial (0, 0) point")
+            self._insert(0, 0)
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
-        self._add(last_t+duration, last_x)
+        self._insert(last_t+duration, last_x)
+
+        return self
 #
 ===============================================================================
 #
 ***** Linear Transition *****
 #
 lin_transition method of PWL class
-    def lin_transition(self, target: float, duration: float) -> None:
+    def lin_transition(self, target: float, duration: float) -> "PWL":
 #
 **** Summary ****
 Method that generates a linear transition from the last value of the previous
 event to a given target with a given duration.
 If the PWL object is empty, adds the point (0, 0) and transitions from that.
 **** Arguments ****
     * target (float) : Value to transition to.
     * duration (float) : Duration of the transition. Should be strictly
       positive.
+### Returns
+    * PWL : Returns the object itself.
 **** Raises ****
     * TypeError : Raised if either target or duration` is not a real number.
     * ValueError : Raised if duration is not strictly positive.
     * PrecisionError : Raised if computational noise causes the time
       coordinates to not be strictly increasing.
         if not isinstance(target, Real):
-            raise TypeError(
-                f"Argument 'target' should be a real number but has type '{type
-(target).__name__}'.")
+            raise TypeError(f"Argument 'target' should be a real number but has
+type '{type(target).__name__}'")
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '
-{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but
+has type '{type(duration).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value
-of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive
+but has value of {duration}")
 
-        self._lin_transition(target, duration, 0)
+        self._nested_lin_transition(target, duration, 0)
+
+        return self
 #
 ===============================================================================
 #
 ***** Rectangular Pulse *****
 #
 rect_pulse method of PWL class
     def rect_pulse(self, value: float, duration: float, t_step: Optional[float]
-= None) -> None:
+= None) -> "PWL":
 #
 **** Summary ****
 Method that generates a rectangular pulse with given amplitude and duration.
 If duration is less than or equal to t_step (self.t_step if t_step is not set),
 substitutes the pulse by a linear transition from the last value of the
 previous event to value with duration t_step (self.t_step if t_step is not
 set).
 **** Arguments ****
     * value (float) : Amplitude of the pulse.
     * duration (float) : Duration of the pulse. Should be strictly positive.
     * t_step (float, optional) : Transition time for the discontinuity. Should
       be strictly positive. If not set, uses self.t_step.
+### Returns
+    * PWL : Returns the object itself.
 **** Raises ****
     * TypeError : Raised if either value, durationort_step` is not a real
       number.
     * ValueError : Raised if either duration or t_step is not strictly
       positive.
     * PrecisionError : Raised if computational noise causes the time
       coordinates to not be strictly increasing.
 **** See Also ****
     * Linear_Transition
         if t_step is None:
             t_step = self._t_step
 
         if not isinstance(value, Real):
-            raise TypeError(
-                f"Argument 'value' should be a real number but has type '{type
-(value).__name__}'.")
+            raise TypeError(f"Argument 'value' should be a real number but has
+type '{type(value).__name__}'")
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '
-{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but
+has type '{type(duration).__name__}'")
         if not isinstance(t_step, Real):
-            raise TypeError(
-                f"Argument 't_step' should either be a real number but has type
-'{type(t_step).__name__}'.")
+            raise TypeError(f"Argument 't_step' should either be a real number
+but has type '{type(t_step).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value
-of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive
+but has value of {duration}")
         if t_step <= 0:
-            raise ValueError(
-                f"Argument 't_step' should be strictly positive but has value
-of {t_step}.")
+            raise ValueError(f"Argument 't_step' should be strictly positive
+but has value of {t_step}")
 
         if self._verbose:
             print(f"{self._name}: Adding rectangular pulse with value of
-{value}, duration of {duration} and time step of {t_step}.")
+{value}, duration of {duration} and time step of {t_step}")
 
         if duration <= t_step:
             if self._verbose:
-                print(
-                    f"{self._name}: Duration of {duration} is less than or
-equal to time step of {t_step}. Converting to linear transition.")
-            self._lin_transition(value, t_step, 1)
-            return
+                print(f"{self._name}: Duration of {duration} is less than or
+equal to time step of {t_step}. Converting to linear transition")
+            self._nested_lin_transition(value, t_step, 1)
+            return self
 
         if len(self._t_list) == len(self._x_list) == 0:
-            self._add(0, value)
+            self._insert(0, value)
             last_t = 0
         else:
             last_t = self._t_list[-1]
-            self._add(last_t+t_step, value)
+            self._insert(last_t+t_step, value)
+
+        self._insert(last_t+duration, value)
 
-        self._add(last_t+duration, value)
+        return self
 #
 ===============================================================================
 #
 ***** Sawtooth Pulse *****
 #
 sawtooth_pulse method of PWL class
     def sawtooth_pulse(self, start: float, end: float, duration: float, t_step:
-Optional[float] = None) -> None:
+Optional[float] = None) -> "PWL":
 #
 **** Summary ****
 Method that generates a sawtooth pulse with given starting and ending
 amplitudes and duration.
 If duration is less than or equal to t_step (self.t_step if t_step is not set),
 substitutes the pulse by a linear transition from the last value of the
 previous event to end with duration t_step (self.t_step if t_step is not set).
 **** Arguments ****
     * start (float) : Amplitude at the start of the pulse.
     * end (float) : Amplitude at the end of the pulse.
     * duration (float) : Duration of the pulse. Should be strictly positive.
     * t_step (float, optional) : Transition time for the discontinuity. Should
       be strictly positive. If not set, uses self.t_step.
+### Returns
+    * PWL : Returns the object itself.
 **** Raises ****
     * TypeError : Raised if either start, end, durationort_step` is not a real
       number.
     * ValueError : Raised if either duration or t_step is not strictly
       positive.
     * PrecisionError : Raised if computational noise causes the time
       coordinates to not be strictly increasing.
 **** See Also ****
     * Linear_Transition
         if t_step is None:
             t_step = self._t_step
 
         if not isinstance(start, Real):
-            raise TypeError(
-                f"Argument 'start' should be a real number but has type '{type
-(start).__name__}'.")
+            raise TypeError(f"Argument 'start' should be a real number but has
+type '{type(start).__name__}'")
         if not isinstance(end, Real):
-            raise TypeError(
-                f"Argument 'end' should be a real number but has type '{type
-(end).__name__}'.")
+            raise TypeError(f"Argument 'end' should be a real number but has
+type '{type(end).__name__}'")
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '
-{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but
+has type '{type(duration).__name__}'")
         if not isinstance(t_step, Real):
-            raise TypeError(
-                f"Argument 't_step' should either be a real number but has type
-'{type(t_step).__name__}'.")
+            raise TypeError(f"Argument 't_step' should either be a real number
+but has type '{type(t_step).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value
-of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive
+but has value of {duration}")
         if t_step <= 0:
-            raise ValueError(
-                f"Argument 't_step' should be strictly positive but has value
-of {t_step}.")
+            raise ValueError(f"Argument 't_step' should be strictly positive
+but has value of {t_step}")
 
         if self._verbose:
             print(f"{self._name}: Adding sawtoth pulse from {start} to {end}
-with duration of {duration} and time step of {t_step}.")
+with duration of {duration} and time step of {t_step}")
 
         if duration <= t_step:
             if self._verbose:
-                print(
-                    f"{self._name}: Duration of {duration} is less than or
-equal to time step of {t_step}. Converting to linear transition.")
-            self._lin_transition(end, t_step, 1)
-            return
+                print(f"{self._name}: Duration of {duration} is less than or
+equal to time step of {t_step}. Converting to linear transition")
+            self._nested_lin_transition(end, t_step, 1)
+            return self
 
         if len(self._t_list) == len(self._x_list) == 0:
-            self._add(0, start)
+            self._insert(0, start)
             last_t = 0
         else:
             last_t = self._t_list[-1]
-            self._add(last_t+t_step, start)
+            self._insert(last_t+t_step, start)
+
+        self._insert(last_t+duration, end)
 
-        self._add(last_t+duration, end)
+        return self
 #
 ===============================================================================
 #
 ***** Exponential Transition *****
 #
 exp_transition method of PWL class
     def exp_transition(self, target: float, duration: float, tau: float,
-t_step: Optional[float] = None) -> None:
+t_step: Optional[float] = None) -> "PWL":
 #
 **** Summary ****
 Method that generates an exponential transition from the last value of the
 previous event to a given target with a given duration.
 If the PWL object is empty, adds the point (0, 0) and transitions from that.
 Let’s call x0 the last value of the previous event and t0 the instant when the
 transition begins. The transition will follow thw following form:
@@ -673,90 +1101,87 @@
 **** Arguments ****
     * target (float) : Value to transition to.
     * duration (float) : Duration of the transition. Should be strictly
       positive.
     * tau (float) : Time constant of the exponential. SHould be non zero.
     * t_step (float, optional) : Timestep between consecutive points inside the
       transition. Should be strictly positive. If not set, uses self.t_step.
+### Returns
+    * PWL : Returns the object itself.
 **** Raises ****
     * TypeError : Raised if either target, duration, tauort_step` is not a real
       number.
     * ValueError : Raised if either duration or t_step is not strictly positive
       or tau is equal to zero.
     * PrecisionError : Raised if computational noise causes the time
       coordinates to not be strictly increasing.
 **** See Also ****
     * Linear_Transition
         if t_step is None:
             t_step = self._t_step
 
         if not isinstance(target, Real):
-            raise TypeError(
-                f"Argument 'target' should be a real number but has type '{type
-(target).__name__}'.")
+            raise TypeError(f"Argument 'target' should be a real number but has
+type '{type(target).__name__}'")
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '
-{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but
+has type '{type(duration).__name__}'")
         if not isinstance(tau, Real):
-            raise TypeError(
-                f"Argument 'tau' should be a real number but has type '{type
-(tau).__name__}'.")
+            raise TypeError(f"Argument 'tau' should be a real number but has
+type '{type(tau).__name__}'")
         if not isinstance(t_step, Real):
-            raise TypeError(
-                f"Argument 't_step' should either be a real number but has type
-'{type(t_step).__name__}'.")
+            raise TypeError(f"Argument 't_step' should either be a real number
+but has type '{type(t_step).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value
-of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive
+but has value of {duration}")
         if tau == 0:
-            raise ValueError("Argument 'tau' should be non zero.")
+            raise ValueError("Argument 'tau' should be non zero")
         if t_step <= 0:
-            raise ValueError(
-                f"Argument 't_step' should be strictly positive but has value
-of {t_step}.")
+            raise ValueError(f"Argument 't_step' should be strictly positive
+but has value of {t_step}")
 
         if self._verbose:
             print(f"{self._name}: Adding exponential transition with target of
 {target}, time constant of {tau}, duration of {duration} and time step of
-{t_step}.")
+{t_step}")
 
         if duration <= t_step:
             if self._verbose:
-                print(
-                    f"    Duration of {duration} is less than or equal to time
-step of {t_step}. Converting to linear transition.")
-            self._lin_transition(target, t_step, 2)
-            return
+                print(f"    Duration of {duration} is less than or equal to
+time step of {t_step}. Converting to linear transition")
+            self._nested_lin_transition(target, t_step, 2)
+            return self
 
         if len(self._t_list) == len(self._x_list) == 0:
             if self._verbose:
-                print("    Empty PWL object. Adding initial (0, 0) point.")
-            self._add(0, 0)
+                print("    Empty PWL object. Adding initial (0, 0) point")
+            self._insert(0, 0)
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
-        f = _exp_transition_func(tau=tau, t1=last_t, t2=last_t +
-                                 duration, f1=last_x, f2=target)
+        f = exp_transition_func(tau=tau, t1=last_t, t2=last_t+duration,
+f1=last_x, f2=target)
 
         for t in np.arange(last_t+t_step, last_t+duration, t_step):
-            self._add(t, f(t))
+            self._insert(t, f(t))
 
-        self._add(last_t+duration, target)
+        self._insert(last_t+duration, target)
+
+        return self
 #
 ===============================================================================
 #
 ***** Half Sine Transition *****
 #
 sin_transition method of PWL class
     def sin_transition(self, target: float, duration: float, t_step: Optional
-[float] = None) -> None:
+[float] = None) -> "PWL":
 #
 **** Summary ****
 Method that generates a half sine transition from the last value of the
 previous event to a given target with a given duration.
 If the PWL object is empty, adds the point (0, 0) and transitions from that.
 Let’s call x0 the last value of the previous event and t0 the instant when the
 transition begins. The transition will follow thw following form:
@@ -775,83 +1200,81 @@
 set).
 **** Arguments ****
     * target (float) : Value to transition to.
     * duration (float) : Duration of the transition. Should be strictly
       positive.
     * t_step (float, optional) : Timestep between consecutive points inside the
       transition. Should be strictly positive. If not set, uses self.t_step.
+### Returns
+    * PWL : Returns the object itself.
 **** Raises ****
     * TypeError : Raised if either target, duration or t_step is not a real
       number.
     * ValueError : Raised if either duration or t_step is not strictly
       positive.
     * PrecisionError : Raised if computational noise causes the time
       coordinates to not be strictly increasing.
 **** See Also ****
     * Linear_Transition
         if t_step is None:
             t_step = self._t_step
 
         if not isinstance(target, Real):
-            raise TypeError(
-                f"Argument 'target' should be a real number but has type '{type
-(target).__name__}'.")
+            raise TypeError(f"Argument 'target' should be a real number but has
+type '{type(target).__name__}'")
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '
-{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but
+has type '{type(duration).__name__}'")
         if not isinstance(t_step, Real):
-            raise TypeError(
-                f"Argument 't_step' should either be a real number but has type
-'{type(t_step).__name__}'.")
+            raise TypeError(f"Argument 't_step' should either be a real number
+but has type '{type(t_step).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value
-of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive
+but has value of {duration}")
         if t_step <= 0:
-            raise ValueError(
-                f"Argument 't_step' should be strictly positive but has value
-of {t_step}.")
+            raise ValueError(f"Argument 't_step' should be strictly positive
+but has value of {t_step}")
 
         if self._verbose:
             print(f"{self._name}: Adding sinusoidal transition with target of
-{target}, duration of {duration} and time step of {t_step}.")
+{target}, duration of {duration} and time step of {t_step}")
 
         if duration <= t_step:
             if self._verbose:
-                print(
-                    f"    Duration of {duration} is less than or equal to time
-step of {t_step}. Converting to linear transition.")
-            self._lin_transition(target, t_step, n=2)
-            return
+                print(f"    Duration of {duration} is less than or equal to
+time step of {t_step}. Converting to linear transition")
+            self._nested_lin_transition(target, t_step, n=2)
+            return self
 
         if len(self._t_list) == len(self._x_list) == 0:
             if self._verbose:
-                print("    Empty PWL object. Adding initial (0, 0) point.")
-            self._add(0, 0)
+                print("    Empty PWL object. Adding initial (0, 0) point")
+            self._insert(0, 0)
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
-        f = _sin_transition_func(
+        f = sin_transition_func(
             t1=last_t, t2=last_t+duration, f1=last_x, f2=target)
 
         for t in np.arange(last_t+t_step, last_t+duration, t_step):
-            self._add(t, f(t))
+            self._insert(t, f(t))
+
+        self._insert(last_t+duration, target)
 
-        self._add(last_t+duration, target)
+        return self
 #
 ===============================================================================
 #
 ***** Smoothstep Transition *****
 #
 smoothstep_transition method of PWL class
     def smoothstep_transition(self, target: float, duration: float, t_step:
-Optional[float] = None) -> None:
+Optional[float] = None) -> "PWL":
 #
 **** Summary ****
 Method that generates a smoothstep transition from the last value of the
 previous event to a given target with a given duration.
 If the PWL object is empty, adds the point (0, 0) and transitions from that.
 Let’s call x0 the last value of the previous event and t0 the instant when the
 transition begins. The transition will follow thw following form:
@@ -867,79 +1290,77 @@
 set).
 **** Arguments ****
     * target (float) : Value to transition to.
     * duration (float) : Duration of the transition. Should be strictly
       positive.
     * t_step (float, optional) : Timestep between consecutive points inside the
       transition. Should be strictly positive. If not set, uses self.t_step.
+### Returns
+    * PWL : Returns the object itself.
 **** Raises ****
     * TypeError : Raised if either target, duration or t_step is not a real
       number.
     * ValueError : Raised if either duration or t_step is not strictly
       positive.
     * PrecisionError : Raised if computational noise causes the time
       coordinates to not be strictly increasing.
 **** See Also ****
     * Linear_Transition
         if t_step is None:
             t_step = self._t_step
 
         if not isinstance(target, Real):
-            raise TypeError(
-                f"Argument 'target' should be a real number but has type '{type
-(target).__name__}'.")
+            raise TypeError(f"Argument 'target' should be a real number but has
+type '{type(target).__name__}'")
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '
-{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but
+has type '{type(duration).__name__}'")
         if not isinstance(t_step, Real):
-            raise TypeError(
-                f"Argument 't_step' should either be a real number but has type
-'{type(t_step).__name__}'.")
+            raise TypeError(f"Argument 't_step' should either be a real number
+but has type '{type(t_step).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value
-of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive
+but has value of {duration}")
         if t_step <= 0:
-            raise ValueError(
-                f"Argument 't_step' should be strictly positive but has value
-of {t_step}.")
+            raise ValueError(f"Argument 't_step' should be strictly positive
+but has value of {t_step}")
 
         if self._verbose:
             print(f"{self._name}: Adding smoothstep transition with target of
-{target}, duration of {duration} and time step of {t_step}.")
+{target}, duration of {duration} and time step of {t_step}")
 
         if duration <= t_step:
             if self._verbose:
-                print(
-                    f"    Duration of {duration} is less than or equal to time
-step of {t_step}. Converting to linear transition.")
-            self._lin_transition(target, t_step, n=2)
-            return
+                print(f"    Duration of {duration} is less than or equal to
+time step of {t_step}. Converting to linear transition")
+            self._nested_lin_transition(target, t_step, n=2)
+            return self
 
         if len(self._t_list) == len(self._x_list) == 0:
             if self._verbose:
-                print("    Empty PWL object. Adding initial (0, 0) point.")
-            self._add(0, 0)
+                print("    Empty PWL object. Adding initial (0, 0) point")
+            self._insert(0, 0)
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
-        f = _smoothstep_transition_func(
+        f = smoothstep_transition_func(
             t1=last_t, t2=last_t+duration, f1=last_x, f2=target)
 
         for t in np.arange(last_t+t_step, last_t+duration, t_step):
-            self._add(t, f(t))
+            self._insert(t, f(t))
+
+        self._insert(last_t+duration, target)
 
-        self._add(last_t+duration, target)
+        return self
 #
 ===============================================================================
 #
-***** PWL File Writer *****
+***** File Writer *****
 #
 write method of PWL class
     def write(self, filename: Optional[str] = None, precision: int = 10) -
 > None:
 #
 **** Summary ****
 Method that takes a PWL object and writes a PWL file with it’s (t, x)
@@ -957,29 +1378,26 @@
     * ValueError : Raised if precision is not strictly positive.
     * PrecisionError : Raised if precision is such that the rounding causes the
       time coordinates to not be strictly increasing.
         if filename is None:
             filename = f'{self._name}.txt'
 
         if not isinstance(filename, str):
-            raise TypeError(
-                f"Argument 'filename' should be a string but has type '{type
-(filename).__name__}'.")
+            raise TypeError(f"Argument 'filename' should be a string but has
+type '{type(filename).__name__}'")
         if not isinstance(precision, int):
-            raise TypeError(
-                f"Argument 'precision' should be an integer but has type '{type
-(precision).__name__}'.")
+            raise TypeError(f"Argument 'precision' should be an integer but has
+type '{type(precision).__name__}'")
 
         if precision <= 0:
-            raise ValueError(
-                f"Argument 'precision' should be strictly positive but has
-value of {precision}.")
+            raise ValueError(f"Argument 'precision' should be strictly positive
+but has value of {precision}")
 
         if self._verbose:
-            print(f"{self._name}: Writing PWL file to {filename}.")
+            print(f"{self._name}: Writing PWL file to {filename}")
 
         t_list = self._t_list
         x_list = self._x_list
 
         with open(filename, "w") as file:
             ti_str = np.format_float_scientific(
                 t_list[0], precision-1, unique=False, sign=False)
@@ -989,23 +1407,47 @@
             last_t = ti_str
             for ti, xi in zip(t_list[1:], x_list[1:]):
                 ti_str = np.format_float_scientific(
                     ti, precision-1, unique=False, sign=False)
                 xi_str = np.format_float_scientific(
                     xi, precision-1, unique=False, sign=True)
                 if ti_str == last_t:
-                    raise PrecisionError(
-                        "The chosen precision level caused the written time
-coordinates to not be strictly increasing.")
+                    raise PrecisionError("The chosen precision level caused the
+written time coordinates to not be strictly increasing")
                 file.write(
                     f"{ti_str}    {xi_str}\n")
                 last_t = ti_str
 #
 ===============================================================================
 #
+***** Object Copy *****
+#
+copy class method of PWL class
+    def copy(self, name: Optional[str] = None) -> "PWL":
+#
+**** Summary ****
+Method that creates a deep copy of a PWL object.
+**** Arguments ****
+    * name (str, optional) : Name of the PWL object used for verbose output
+      printing. Should not be empty. If not set, automatically generates a name
+      based on already taken names.
+**** Returns ****
+    * PWL
+**** Raises ****
+    * TypeError : Raised if name is not a string.
+    * ValueError : Raised if name is either empty or already taken.
+        new_pwl = PWL(t_step=self.t_step, name=name, verbose=self.verbose)
+
+        new_pwl._t_list = self.t_list
+        new_pwl._x_list = self.x_list
+
+        return new_pwl
+#
+===============================================================================
+#
 ***** PWL Plotter *****
 #
 plot class method of PWL class
     @classmethod
     def plot(cls, merge: bool = False) -> None:
 #
 Optional feature: Requires matplotlib
@@ -1017,36 +1459,34 @@
       on the same strip or separeted. If not set, defaults to False.
 **** Raises ****
     * TypeError : Raised if merge is not a boolean.
     * ImportError : Raised if the matplotlib package is not installed.
 **** See Also ****
     * Plot_Enable_Flag
         if not _has_matplotlib:
-            raise ImportError(
-                "Optional plotting features are deactivated. Install matplotlib
-to use.")
+            raise ImportError("Optional plotting features are deactivated.
+Install matplotlib to use")
 
         if not isinstance(merge, bool):
-            raise TypeError(
-                f"Argument 'merge' should be a boolean but has type '{type
-(merge).__name__}'.")
+            raise TypeError(f"Argument 'merge' should be a boolean but has type
+'{type(merge).__name__}'")
 
         dict_of_objects = {key: pwl for key,
                            pwl in cls.__dict_of_objects.items() if
 pwl.plot_flag}
 
         if not dict_of_objects:
             return None
 
         if merge:
             axs = plt.subplots(nrows=1, sharex=True, squeeze=False)[1]
             axs = np.repeat(axs, len(dict_of_objects))
         else:
-            axs = plt.subplots(nrows=len(dict_of_objects),
-                               sharex=True, squeeze=False)[1]
+            axs = plt.subplots(nrows=len(dict_of_objects), sharex=True,
+squeeze=False)[1]
             axs = axs.flatten()
         x_max: float = 0
 
         for key, ax in zip(dict_of_objects, axs):
             pwl = dict_of_objects[key]
             if not pwl._plot_flag:
                 continue
@@ -1056,173 +1496,110 @@
             label = pwl.name
             ax.plot(x_list, y_list)
             ax.set_ylabel(label)
 
         axs[0].set_xlim(xmin=0, xmax=x_max)
         plt.show()
 #
-****** Private Methods and Functions ******
-#
-From this point forward, all listed methods and functions are not intended to
-be used by the user. Brief descriptions will be provided, but documentation
-will be kept to a minimum.
-#
 ===============================================================================
 #
-***** PWL Point Adder *****
-#
-_add private method of PWL class
-    def _add(self, t: float, x: float) -> None:
-#
-Private method that adds a (t, x) point to a PWL object of any size.
+    def _insert(self, t: float, x: float) -> None:
         if len(self._t_list) >= 1 and t <= self._t_list[-1]:
-            raise PrecisionError(
-                f"Internal Python rounding caused the time coordinates to not
-be strictly increasing when adding points to {self._name}.")
+            raise PrecisionError(f"Internal Python rounding caused the time
+coordinates to not be strictly increasing when adding points to {self._name}")
 
         if len(self._t_list) == len(self._x_list) < 2:
             self._t_list.append(t)
             self._x_list.append(x)
         else:
             self._colinear_eliminator(x, t)
 #
-===============================================================================
-#
-***** Colinear Points Eliminator *****
-#
-_colinear_eliminator private method of PWL class
     def _colinear_eliminator(self, x: float, t: float) -> None:
-#
-Private method that adds a (t, x) point to a PWL object with 2 or more points
-without consecutive colinear points.
         t_n_1 = self._t_list[-1]
         t_n_2 = self._t_list[-2]
 
         x_n_1 = self._x_list[-1]
         x_n_2 = self._x_list[-2]
 
         last_m = (x_n_1 - x_n_2)/(t_n_1 - t_n_2)
         new_m = (x - x_n_1)/(t - t_n_1)
 
-        if last_m == new_m:
+        if is_within(last_m, new_m):
             self._t_list[-1] = t
             self._x_list[-1] = x
         else:
             self._t_list.append(t)
             self._x_list.append(x)
 #
-===============================================================================
-#
-***** Nested Linear Transition *****
-#
-_lin_transition private method of PWL class
-    def _lin_transition(self, target: float, duration: float, n: int) -> None:
-#
-Private method to generate a linear transition. The difference between this
-method and the public_linear_transition method is that this method prints
-indented verbose output when called from within any of the public methods that
-revert to a linear transition in certain conditions.
+    def _nested_lin_transition(self, target: float, duration: float, n: int) -
+> None:
         if self._verbose:
             if n == 0:
-                print(
-                    f"{self._name}: Adding linear transition with target of
-{target} and duration of {duration}.")
+                print(f"{self._name}: Adding linear transition with target of
+{target} and duration of {duration}")
             else:
-                print(
-                    n*"    "+f"Adding linear transition with target of {target}
-and duration of {duration}.")
+                print(n*"    "+f"Adding linear transition with target of
+{target} and duration of {duration}")
 
         if len(self._t_list) == len(self._x_list) == 0:
             if self._verbose:
                 print((n+1)*"    "+"Empty PWL object. Adding initial (0, 0)
-point.")
-            self._add(0, 0)
+point")
+            self._insert(0, 0)
 
         last_t = self._t_list[-1]
-        self._add(last_t+duration, target)
-#
-===============================================================================
-#
-***** Exponential Function Generator *****
+        self._insert(last_t+duration, target)
 #
-_exp_transition_func private function
-def _exp_transition_func(tau: float, t1: float, f1: float, t2: float, f2:
-float) -> Callable[[float], float]:
-#
-Private function that generates an exponential function passing trough 2 fixed
-points.
-    A: float = (f1*np.exp(t1/tau) - f2*np.exp(t2/tau)) / \
-        (np.exp(t1/tau) - np.exp(t2/tau))
+def exp_transition_func(tau: float, t1: float, f1: float, t2: float, f2: float)
+-> Callable[[float], float]:
+    A: float = (f1*np.exp(t1/tau) - f2*np.exp(t2/tau)) / (np.exp(t1/tau) -
+np.exp(t2/tau))
     B: float = (f1 - f2)/(np.exp(-t1/tau) - np.exp(-t2/tau))
 #
     def f(t: float) -> float:
         result: float = A + B*np.exp(-t/tau)
         return result
 
     return f
 #
-===============================================================================
-#
-***** Sinusoidal Function Generator *****
-#
-_sin_transition_func private function
-def _sin_transition_func(t1: float, f1: float, t2: float, f2: float) -
-> Callable[[float], float]:
-#
-Private function that generates a sinusoidal function passing trough 2 fixed
-points.
+def sin_transition_func(t1: float, f1: float, t2: float, f2: float) -> Callable
+[[float], float]:
     fm: float = (f1+f2)/2
     tm: float = (t1+t2)/2
     T: float = 2*(t2-t1)
     w: float = 2*np.pi/T
     phi: float = w*tm
     A: float = f2-fm
 #
     def f(t: float) -> float:
         result: float = fm + A*np.sin(w*t - phi)
         return result
 
     return f
 #
-===============================================================================
-#
-***** Smoothstep Function Generator *****
-#
-_smoothstep_transition_func private function
-def _smoothstep_transition_func(t1: float, f1: float, t2: float, f2: float) -
+def smoothstep_transition_func(t1: float, f1: float, t2: float, f2: float) -
 > Callable[[float], float]:
-#
-Private function that generates a smoothstep function passing trough 2 fixed
-points.
     Am = np.array([[1, t1, t1**2, t1**3],
                    [1, t2, t2**2, t2**3],
                    [0, 1, 2*t1, 3*t1**2],
                    [0, 1, 2*t2, 3*t2**2]])
     Bm = np.array([f1, f2, 0, 0])
     A, B, C, D = np.linalg.solve(Am, Bm)
 #
     def f(t: float) -> float:
         result: float = A + B*t + C*t**2 + D*t**3
         return result
 
     return f
 #
-===============================================================================
-if __name__ == "__main__":
-    pwl0 = PWL(0.001)
-    pwl1 = PWL(0.001)
-
-    pwl0.hold(1)
-    pwl1.hold(1)
+def is_within(x: float, y: float, tol: float = 0.01) -> float:
+    error = 0 if x == y else 2*abs(x-y)/(abs(x)+abs(y))
 
-    pwl0.sin_transition(1, 1)
-    pwl1.sin_transition(-1, 1)
+    return error <= tol
 
-    pwl0.hold(1)
-    pwl1.hold(1)
 
-    pwl0.sin_transition(0, 1)
-
-    pwl1.plot_flag = False
+if __name__ == "__main__":
+    t = PWL(0.01, name="t").lin_transition(10, 10)
+    x = -(1/3)*(t**3)+5*(t**2)-15*t
+    x.name = "x"
 
-    PWL.plot(merge=False)
-    print(pwl0(1.5))
+    PWL.plot()
```

### Comparing `pwl_writer-1.1.3/docs/pycco.css` & `pwl_writer-1.2.0/docs/pycco.css`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.3/pwl_writer/pwl_writer.py` & `pwl_writer-1.2.0/pwl_writer/pwl_writer.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,46 +13,51 @@
 Type stubs for older numpy versions for mypy checking can be found [here](https://github.com/numpy/numpy-stubs).
 
 ----
 
 # Index
 
 * [Package Summary](#package-summary)
-* [Precision Related Exception](#precision-related-exception)
 * [PWL Class](#pwl-class)
         * Dunder Methods
             * [Initializer](#initializer)
             * [String Representation](#string-representation)
             * [Length Calculator](#length-calculator)
-            * [Object as a Callable](#object-as-a-callable)
+            * [Object Calling](#object-calling)
+            * [Object Slicing](#object-slicing)
+            * [Object Iteration](#object-iteration)
+        * Mathematical Unary Operators
+            * [Additive Inverse](#additive-inverse)
+            * [Absolute Value](#absolute-value)
+        * Mathematical Binary Operators
+            * [Addition](#addition)
+            * [Subtraction](#subtraction)
+            * [Multiplication](#multiplication)
+            * [Division](#division)
+            * [Exponentiation](#exponentiation)
         * Properties
             * [Time Coordinates](#time-coordinates)
             * [Dependent Coordinates](#dependent-coordinates)
             * [Default Timestep](#default-timestep)
             * [Name](#name)
             * [Verbose Flag](#verbose-flag)
             * [Plot Enable Flag](#plot-enable-flag) *(optional feature: requires matplotlib)*
-        * Methods
+        * Instance Methods
+            * [Initial Condition](#initial-condition)
             * [Last Value Holder](#last-value-holder)
             * [Linear Transition](#linear-transition)
             * [Rectangular Pulse](#rectangular-pulse)
             * [Sawtooth Pulse](#sawtooth-pulse)
             * [Exponential Transition](#exponential-transition)
             * [Half Sine Transition](#half-sine-transition)
             * [Smoothstep Transition](#smoothstep-transition)
-            * [PWL File Writer](#pwl-file-writer)
+            * [File Writer](#file-writer)
+            * [Object Copy](#object-copy)
+        * Class Methods
             * [PWL Plotter](#pwl-plotter) *(optional feature: requires matplotlib)*
-        * Private Methods *(minimal documentation)*
-            * [PWL Point Adder](#pwl-point-adder)
-            * [Colinear Points Eliminator](#colinear-points-eliminator)
-            * [Nested Linear Transition](#nested-linear-transition)
-* Private Functions *(minimal documentation)*
-        * [Exponential Function Generator](#exponential-function-generator)
-        * [Sinusoidal Function Generator](#sinusoidal-function-generator)
-        * [Smoothstep Function Generator](#smoothstep-function-generator)
         
 ----
 
 # Package Summary
 
 This package defines a class `PWL` to generate objects that represent time dependent signals `x(t)` that need to be coded in a PWL file. Those objects are built using little components such as rectangular pulses and sawtooth pulses that can be chained together.
 
@@ -79,116 +84,125 @@
 For each state, various control signals need to be at specific values. We could create a `PWL` object for each control signal and define 3 functions that apply all the needed values for the control signals for each state. If we nedded the system to be at mode 1 for 3 seconds, idle for 1 second and at mode 2 for 5 seconds, we could write something like the following:
 
         mode1_state(3)
         idle_state(1)
         mode2_state(5)
 """
 
-__all__ = ['PrecisionError', 'PWL']
+__all__ = ['PWL']
 
-from warnings import warn
+import warnings
 from numbers import Real
-from typing import Callable, Dict, List, Optional
+from typing import Callable, List, Optional, TYPE_CHECKING, Union, Tuple, Iterator, TypeVar, Any, cast
+import weakref
 import numpy as np
 
+
 try:
     import matplotlib.pyplot as plt  # type: ignore
 except ImportError:
     _has_matplotlib = False
-    warn("Matplotlib package not found. Optional plotting features deactivated.", ImportWarning)
+    warnings.warn("Matplotlib package not found. Optional plotting features deactivated.", ImportWarning)
 else:
     _has_matplotlib = True
 
-# ----
+if TYPE_CHECKING:
+    WeakDict = weakref.WeakValueDictionary[str, "PWL"]
+
+TFun = TypeVar("TFun", bound=Callable[..., Any])
+
+
+class copy_doc:
+    def __init__(self, copy_func: TFun) -> None:
+        self.copy_func = copy_func
 
-# == Precision Related Exception ==
+    def __call__(self, func: TFun) -> TFun:
+        func.__doc__ = self.copy_func.__doc__
+        return func
 
 
 class PrecisionError(Exception):
-    """**`PrecisionError` exception class**
+    pass
+
+
+class InitialConditionError(Exception):
+    pass
 
-    This class defines an exception meant to be raised when any type of rounding or loss of precision that causes the time coordinates of a PWL object to not be strictly increasing.
-    """
 
 # ----
 
 # == PWL Class ==
 
-
 class PWL():
     """**`PWL` class**
 
     This class defines an object that represnts a time dependent signal `x(t)`. Those objects can operated on by methods to build, event by event, the desired signal as described on the package introduction.
     """
 
-    __dict_of_objects: Dict[str, 'PWL'] = {}
+    __dict_of_objects = weakref.WeakValueDictionary()  # type: WeakDict
 
     # ----
 
     # == Initializer ==
 
     def __init__(self, t_step: float, name: Optional[str] = None, verbose: bool = False) -> None:
-        """**Dunder method `__init__` of `PWL` class**
+        """**`__init__` dunder method of `PWL` class**
 
         ### Summary
 
         Initializer for the `PWL` class.
 
         ### Arguments
 
         * `t_step` (`float`) : Default timestep for all operations. Should be strictly positive.
         * `name` (`str`, optional) : Name of the `PWL` object used for verbose output printing. Should not be empty. If not set, automatically generates a name based on already taken names.
         * `verbose` (`bool`, optional) : Flag indicating if verbose output should be printed. If not set, defaults to `False`.
 
         ### Raises
 
         * `TypeError` : Raised if either `t_step` is not a real number, `name` is not a string or `verbose` is not a boolean.
-        * `ValueError` : Raised if `t_step` is not strictly positive or `name` is empty.
+        * `ValueError` : Raised if `t_step` is not strictly positive or `name` is either empty or already taken.
         """
 
         if name is None:
             i: int = 0
-            while f"pwl_{i}" in PWL.__dict_of_objects:
+            while f"pwl_{i}" in PWL.__dict_of_objects.keys():
                 i += 1
             name = f"pwl_{i}"
 
         if not isinstance(t_step, Real):
-            raise TypeError(
-                f"Argument 't_step' should be a real number but has type '{type(t_step).__name__}'.")
+            raise TypeError(f"Argument 't_step' should be a real number but has type '{type(t_step).__name__}'")
         if not isinstance(name, str):
-            raise TypeError(
-                f"Argument 'name' should either be a string but has type '{type(name).__name__}'.")
+            raise TypeError(f"Argument 'name' should either be a string but has type '{type(name).__name__}'")
         if not isinstance(verbose, bool):
-            raise TypeError(
-                f"Argument 'verbose' should be a boolean but has type '{type(verbose).__name__}'.")
+            raise TypeError(f"Argument 'verbose' should be a boolean but has type '{type(verbose).__name__}'")
 
         if t_step <= 0:
-            raise ValueError(
-                f"Argument 't_step' should be strictly positive but has value of {t_step}.")
+            raise ValueError(f"Argument 't_step' should be strictly positive but has value of {t_step}")
         if not name:
-            raise ValueError("Argument 'name' should not be empty.")
+            raise ValueError("Argument 'name' should not be empty")
 
         self._t_list: List[float] = []
         self._x_list: List[float] = []
         self._t_step: float = t_step
         self._name: str = name
         self._verbose: bool = verbose
         self._plot_flag: bool = True
 
-        if name in PWL. __dict_of_objects:
-            raise ValueError(f"Name '{name}' already in use.")
+        if name in PWL.__dict_of_objects.keys():
+            raise ValueError(f"Name '{name}' already in use")
 
-        PWL. __dict_of_objects[name] = self
+        PWL.__dict_of_objects[name] = self
 
     # ----
 
     # == String Representation ==
 
     def __str__(self) -> str:
-        """**Dunder method `__str__` of `PWL` class**
+        """**`__str__` dunder method of `PWL` class**
 
         ### Summary
 
         String representation of `PWL` instances in the form `[name]: PWL object with [# of points] and duration of [total time duration] seconds`.
 
         ### Returns
 
@@ -200,33 +214,33 @@
         return f"{self.name}: PWL object with {len(self._t_list)} points and duration of {duration} seconds"
 
     # ----
 
     # == Length Calculator ==
 
     def __len__(self) -> int:
-        """**Dunder method `__len__` of `PWL` class**
+        """**`__len__` dunder method of `PWL` class**
 
         ### Summary
 
         Length of `PWL` instances defined as the number of `(t, x)` points they contain.
 
         ### Returns
 
         * `int`
         """
 
         return len(self._t_list)
 
     # ----
 
-    # == Object as a Callable ==
+    # == Object Calling ==
 
     def __call__(self, t: float) -> float:
-        """**Dunder method `__call__` of `PWL` class**
+        """**`__call__` dunder method of `PWL` class**
 
         ### Summary
 
         Call `PWL` object as a function by linearly interpolating between it's time and dependent coordinates.
 
         ### Arguments
 
@@ -238,24 +252,470 @@
 
         ### Raises
 
         * `TypeError` : Raised if `t` is not a real number.
         """
 
         if not isinstance(t, Real):
-            raise TypeError(
-                f"Argument 't' should be a real number but has type '{type(t).__name__}'.")
+            raise TypeError(f"Argument 't' should be a real number but has type '{type(t).__name__}'")
 
         t_list = self._t_list
         x_list = self._x_list
 
         return np.interp(x=t, xp=t_list, fp=x_list, left=0)
 
     # ----
 
+    # == Object Slicing ==
+
+    def __getitem__(self, index: Union[int, slice]) -> Union[Tuple[float, float], List[Tuple[float, float]]]:
+        """**`__getitem__` dunder method of `PWL` class**
+
+        ### Summary
+
+        Slice `PWL` objects.
+
+        ### Arguments
+
+        * `index` (`int` or `slice`) : Index for list of `(t, x)` points.
+
+        ### Returns
+
+        * `Tuple[float, float]` : Returned if single index is passed.
+        * `List[Tuple[float, float]]` : Rerturned if multiple indices are passed.
+
+        ### Raises
+
+        * `TypeError` : Raised if `index` is not an integer or slice.
+        * `IndexError` : Raised if `index` is out of bounds.
+        """
+
+        if not isinstance(index, (int, slice)):
+            raise TypeError(f"PWL indices must be integers or slices, not {type(index).__name__}")
+
+        coordinates_pair = list(zip(self.t_list, self.x_list))
+
+        return coordinates_pair[index]
+
+    # ----
+
+    # == Object Iteration ==
+
+    def __iter__(self) -> Iterator[Tuple[float, float]]:
+        """**`__iter__` dunder method of `PWL` class**
+
+        ### Summary
+
+        Creates a generator object that yields all the `(t, x)` points as tuples.
+
+        ### Yields
+
+        * `Tuple[float, float]`
+        """
+        yield from list(zip(self.t_list, self.x_list))
+
+    # ----
+
+    # == Additive Inverse ==
+
+    def __neg__(self) -> "PWL":
+        """**`__neg__` dunder method of `PWL` class**
+
+        ### Summary
+
+        Implements point-wise additive inversion (multiplying by -1).
+
+        The new `PWL` objects created has `t_step` equal to the operand's `t_step`.
+
+        ### Arguments
+
+        * Operand (`PWL` or `float`) : Thing being additivly inverted.
+
+        ### Returns
+
+        * `PWL` : The additive inverse of the operand.
+
+        ### See Also
+
+        * [Multiplication](#multiplication)
+        """
+        return -1*self
+
+    def __pos__(self) -> "PWL":
+        return self.copy()
+
+    # ----
+
+    # == Absolute Value ==
+
+    def __abs__(self) -> "PWL":
+        """**`__abs__` dunder method of `PWL` class**
+
+        ### Summary
+
+        Implements point-wise absolute value operation.
+
+        The new `PWL` objects created has `t_step` equal to the operand's `t_step`.
+
+        ### Arguments
+
+        * Operand (`PWL` or `float`) : Thing whose absolute value is being taken.
+
+        ### Returns
+
+        * `PWL` : The absolute value of the operand.
+        """
+
+        new_pwl = PWL(t_step=self.t_step)
+
+        for t, x in self:
+            new_x = cast(float, np.absolute(x))
+            new_pwl._insert(t, new_x)
+
+        return new_pwl
+
+    # ----
+
+    # == Addition ==
+
+    def __add__(self, other: Union["PWL", float]) -> "PWL":
+        """**`__add__` and `__radd__`  dunder methods of `PWL` class**
+
+        ### Summary
+
+        Implements point-wise addition of `PWL` objects with real numbers and other `PWL` objects.
+
+        The new `PWL` objects created has `t_step` equal to the lower `t_step` between the operands.
+
+        If one operand is longer than the other, extends the shorter one by holding it's last value.
+
+        ### Arguments
+
+        * Addends (`PWL` or `float`) : Things being added together.
+
+        ### Returns
+
+        * `PWL` : The sum of the addends.
+
+        ### Raises
+
+        * `TypeError` : Raised if operation is not implemented between the operands.
+        """
+
+        if not isinstance(other, (Real, PWL)):
+            return NotImplemented
+
+        t_step = min(self.t_step, other.t_step) if isinstance(other, PWL) else self.t_step
+        new_pwl = PWL(t_step=t_step)
+
+        if isinstance(other, Real):
+            other_copy = float(other)
+            other = lambda *args, **kwargs: other_copy
+
+        unsorted_t_set = set(self.t_list + other.t_list)
+        t_list = sorted(list(unsorted_t_set))
+        for t in t_list:
+            new_pwl._insert(t, self(t) + other(t))
+
+        return new_pwl
+
+    @copy_doc(__add__)
+    def __radd__(self, other: float) -> "PWL":
+        return self + other
+
+    # ----
+
+    # == Subtraction ==
+
+    def __sub__(self, other: Union["PWL", float]) -> "PWL":
+        """**`__sub__` and `__rsub__`  dunder methods of `PWL` class**
+
+        ### Summary
+
+        Implements point-wise subtraction of `PWL` objects with real numbers and other `PWL` objects.
+
+        The new `PWL` objects created has `t_step` equal to the lower `t_step` between the operands.
+
+        If one operand is longer than the other, extends the shorter one by holding it's last value.
+
+        ### Arguments
+
+        * Minuend (`PWL` or `float`) : Thing from which we subtract the subtrahend.
+        * Subtrahend (`PWL` or `float`) : Thing being subtracted from the minuend.
+
+        ### Returns
+
+        * `PWL` : The difference of the minuend an subtrahend.
+
+        ### Raises
+
+        * `TypeError` : Raised if operation is not implemented between the operands.
+        """
+
+        if not isinstance(other, (Real, PWL)):
+            return NotImplemented
+
+        t_step = min(self.t_step, other.t_step) if isinstance(other, PWL) else self.t_step
+        new_pwl = PWL(t_step=t_step)
+
+        if isinstance(other, Real):
+            other_copy = float(other)
+            other = lambda *args, **kwargs: other_copy
+
+        unsorted_t_set = set(self.t_list + other.t_list)
+        t_list = sorted(list(unsorted_t_set))
+        for t in t_list:
+            new_pwl._insert(t, self(t) - other(t))
+
+        return new_pwl
+
+    @copy_doc(__sub__)
+    def __rsub__(self, other: float) -> "PWL":
+        t_step = self.t_step
+        new_pwl = PWL(t_step=t_step)
+
+        for t, x in self:
+            new_pwl._insert(t, other-x)
+
+        return new_pwl
+
+    # ----
+
+    # == Multiplication ==
+
+    def __mul__(self, other: Union["PWL", float]) -> "PWL":
+        """**`__mul__` and `__rmul__`  dunder methods of `PWL` class**
+
+        ### Summary
+
+        Implements point-wise multiplication of `PWL` objects with real numbers and other `PWL` objects.
+
+        The new `PWL` objects created has `t_step` equal to the lower `t_step` between the operands.
+
+        If one operand is longer than the other, extends the shorter one by holding it's last value.
+
+        ### Arguments
+
+        * Factors (`PWL` or `float`) : Things being multiplied together.
+
+        ### Returns
+
+        * `PWL` : The product of the factors.
+
+        ### Raises
+
+        * `TypeError` : Raised if operation is not implemented between the operands.
+        """
+
+        if not isinstance(other, (Real, PWL)):
+            return NotImplemented
+
+        t_step = min(self.t_step, other.t_step) if isinstance(other, PWL) else self.t_step
+        t_max = max(self.t_list[-1], other._t_list[-1]) if isinstance(other, PWL) else self._t_list[-1]
+        x_last = np.multiply(self(t_max), other(t_max)) if isinstance(other, PWL) else np.multiply(self(t_max), cast(float, other))
+        t_list = np.arange(0, t_max, t_step)
+
+        new_pwl = PWL(t_step=t_step)
+
+        if isinstance(other, Real):
+            other_copy = float(other)
+            other = lambda *args, **kwargs: other_copy
+
+        for t in t_list:
+            new_x = cast(float, np.multiply(self(t), other(t)))
+            new_pwl._insert(t, new_x)
+
+        if t_max > new_pwl._t_list[-1]:
+            new_x = cast(float, x_last)
+            new_pwl._insert(t_max, new_x)
+
+        return new_pwl
+
+    @copy_doc(__mul__)
+    def __rmul__(self, other: float) -> "PWL":
+        return self * other
+
+    # ----
+
+    # == Division ==
+
+    def __truediv__(self, other: Union["PWL", float]) -> "PWL":
+        """**`__truediv__` and `__rtruediv__`  dunder methods of `PWL` class**
+
+        ### Summary
+
+        Implements point-wise division of `PWL` objects with real numbers and other `PWL` objects.
+
+        The new `PWL` objects created has `t_step` equal to the lower `t_step` between the operands.
+
+        If one operand is longer than the other, extends the shorter one by holding it's last value.
+
+        ### Arguments
+
+        * Numerator (`PWL` or `float`) : Thing being divided by the denominator.
+        * Denominator (`PWL` or `float`) : Thing that the numerator is being divided by.
+
+        ### Returns
+
+        * `PWL` : The ratio of the numerator and denominator.
+
+        ### Raises
+
+        * `TypeError` : Raised if operation is not implemented between the operands.
+        * `ZeroDivisionError` : Raised if the denominator contains the point `(t, 0)` for any `t`.
+        """
+
+        if not isinstance(other, (Real, PWL)):
+            return NotImplemented
+
+        t_step = min(self.t_step, other.t_step) if isinstance(other, PWL) else self.t_step
+        t_max = max(self.t_list[-1], other._t_list[-1]) if isinstance(other, PWL) else self._t_list[-1]
+        x_last = np.multiply(self(t_max), other(t_max)) if isinstance(other, PWL) else np.true_divide(self(t_max), cast(float, other))
+        t_list = np.arange(0, t_max, t_step)
+
+        new_pwl = PWL(t_step=t_step)
+
+        if isinstance(other, Real):
+            other_copy = float(other)
+            other = lambda *args, **kwargs: other_copy
+
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore')
+            for t in t_list:
+                left_x = cast(float, np.true_divide(self(t-t_step/2), other(t-t_step/2)))
+                center_x = cast(float, np.true_divide(self(t), other(t)))
+                rigth_x = cast(float, np.true_divide(self(t+t_step/2), other(t+t_step/2)))
+
+                if np.isfinite(center_x):
+                    new_pwl._insert(t, center_x)
+                elif np.isfinite(left_x) and np.isfinite(rigth_x):
+                    new_pwl._insert(t, (left_x+rigth_x)/2)
+                elif np.isfinite(left_x):
+                    new_pwl._insert(t, left_x)
+                elif np.isfinite(rigth_x):
+                    new_pwl._insert(t, rigth_x)
+                else:
+                    new_pwl._insert(t, 0)
+
+        if t_max > new_pwl._t_list[-1]:
+            new_pwl._insert(t_max, cast(float, x_last))
+
+        return new_pwl
+
+    @copy_doc(__truediv__)
+    def __rtruediv__(self, other: float) -> "PWL":
+        if not isinstance(other, Real):
+            return NotImplemented
+
+        t_step = self.t_step
+        t_max = self._t_list[-1]
+        t_list = np.arange(0, t_max, t_step)
+        x_last = np.true_divide(other, self(t_max))
+
+        new_pwl = PWL(t_step=t_step)
+
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore')
+            for t in t_list:
+                left_x = cast(float, np.true_divide(other, self(t-t_step/2)))
+                center_x = cast(float, np.true_divide(other, self(t)))
+                rigth_x = cast(float, np.true_divide(other, self(t+t_step/2)))
+
+                if np.isfinite(center_x):
+                    new_pwl._insert(t, center_x)
+                elif np.isfinite(left_x) and np.isfinite(rigth_x):
+                    new_pwl._insert(t, (left_x+rigth_x)/2)
+                elif np.isfinite(left_x):
+                    new_pwl._insert(t, left_x)
+                elif np.isfinite(rigth_x):
+                    new_pwl._insert(t, rigth_x)
+                else:
+                    new_pwl._insert(t, 0)
+
+        if t_max > new_pwl._t_list[-1]:
+            new_pwl._insert(t_max, x_last)
+
+        return new_pwl
+
+    # ----
+
+    # == Exponentiation ==
+
+    def __pow__(self, other: Union["PWL", float]) -> "PWL":
+        """**`__pow__` and `__rpow__`  dunder methods of `PWL` class**
+
+        ### Summary
+
+        Implements point-wise exponentiation of `PWL` objects with real numbers and other `PWL` objects.
+
+        If the result of the exponentiation ends up being a complex number, returns the real part of it.
+
+        The new `PWL` objects created has `t_step` equal to the lower `t_step` between the operands.
+
+        If one operand is longer than the other, extends the shorter one by holding it's last value.
+
+        ### Arguments
+
+        * Base (`PWL` or `float`) : Thing being raised to the exponent.
+        * Exponent (`PWL` or `float`) : Thing to raise the base to.
+
+        ### Returns
+
+        * `PWL` : The power with the given base and exponent.
+
+        ### Raises
+
+        * `TypeError` : Raised if operation is not implemented between the operands.
+        """
+
+        if not isinstance(other, (Real, PWL)):
+            return NotImplemented
+
+        t_step = min(self.t_step, other.t_step) if isinstance(other, PWL) else self.t_step
+        t_max = max(self.t_list[-1], other.t_list[-1]) if isinstance(other, PWL) else self.t_list[-1]
+        x_last = np.multiply(self(t_max), other(t_max)) if isinstance(other, PWL) else cast(float, np.power(self(t_max), cast(float, other), dtype=complex).real)
+        t_list = np.arange(0, t_max, t_step)
+
+        new_pwl = PWL(t_step=t_step)
+
+        if isinstance(other, Real):
+            other_copy = float(other)
+            other = lambda *args, **kwargs: other_copy
+
+        for t in t_list:
+            new_x = cast(float, np.power(self(t), other(t), dtype=complex).real)
+            new_pwl._insert(t, new_x)
+
+        if t_max > new_pwl._t_list[-1]:
+            new_pwl._insert(t_max, cast(float, x_last))
+
+        return new_pwl
+
+    @copy_doc(__pow__)
+    def __rpow__(self, other: float) -> "PWL":
+        if not isinstance(other, Real):
+            return NotImplemented
+
+        t_step = self.t_step
+        t_max = self.t_list[-1]
+        x_last = np.power(self(t_max), other, dtype=complex).real
+        t_list = np.arange(0, t_max, t_step)
+
+        new_pwl = PWL(t_step=t_step)
+
+        for t in t_list:
+            new_pwl._insert(t, np.power(other, self(t), dtype=complex).real)
+
+        if t_max > new_pwl._t_list[-1]:
+            new_pwl._insert(t_max, x_last)
+
+        return new_pwl
+
+    # ----
+
     # == Time Coordinates ==
 
     @property
     def t_list(self) -> List[float]:
         """**`t_list` property of `PWL` class**
 
         ### Type
@@ -267,15 +727,15 @@
         Read only property containing all the time coordinates of a `PWL` object.
 
         ### Raises
 
         * `AttributeError` : Raised if assignment was attempetd.
         """
 
-        return self._t_list
+        return self._t_list[:]
 
     # ----
 
     # == Dependent Coordinates ==
 
     @property
     def x_list(self) -> List[float]:
@@ -290,15 +750,15 @@
         Read only property containing all the dependent coordinates of a `PWL` object.
 
         ### Raises
 
         * `AttributeError` : Raised if assignment was attempetd.
         """
 
-        return self._x_list
+        return self._x_list[:]
 
     # ----
 
     # == Default Timestep ==
 
     @property
     def t_step(self) -> float:
@@ -319,19 +779,17 @@
         """
 
         return self._t_step
 
     @t_step.setter
     def t_step(self, new_t_step: float) -> None:
         if not isinstance(new_t_step, float):
-            raise TypeError(
-                f"Property 't_step' should be a real number but an object of type '{type(new_t_step).__name__}' was assigned to it.")
+            raise TypeError(f"Property 't_step' should be a real number but an object of type '{type(new_t_step).__name__}' was assigned to it")
         if new_t_step <= 0:
-            raise ValueError(
-                f"Propety 't_step' should be strictly positive but a value of {new_t_step} was assigned to it.")
+            raise ValueError(f"Propety 't_step' should be strictly positive but a value of {new_t_step} was assigned to it")
 
         self._t_step = new_t_step
 
     # ----
 
     # == Name ==
 
@@ -354,25 +812,23 @@
         """
 
         return self._name
 
     @name.setter
     def name(self, new_name: str) -> None:
         if not isinstance(new_name, str):
-            raise TypeError(
-                f"Property 'name' should be a string but an object of type '{type(new_name).__name__}' was assigned to it.")
+            raise TypeError(f"Property 'name' should be a string but an object of type '{type(new_name).__name__}' was assigned to it")
         if not new_name:
-            raise ValueError(
-                "An empty string cannot be assigned to the 'name' property.")
+            raise ValueError("An empty string cannot be assigned to the 'name' property")
 
-        if new_name in PWL. __dict_of_objects:
-            raise ValueError(f"Name '{new_name}' already in use.")
+        if new_name in PWL.__dict_of_objects.keys():
+            raise ValueError(f"Name '{new_name}' already in use")
 
-        PWL. __dict_of_objects.pop(self._name)
-        PWL. __dict_of_objects[new_name] = self
+        PWL.__dict_of_objects.pop(self._name)
+        PWL.__dict_of_objects[new_name] = self
         self._name = new_name
 
     # ----
 
     # == Verbose Flag ==
 
     @property
@@ -394,16 +850,15 @@
 
         return self._verbose
 
     @verbose.setter
     def verbose(self, new_verbose: bool) -> None:
 
         if not isinstance(new_verbose, bool):
-            raise TypeError(
-                f"Attribute 'verbose' should be a boolean but an object of type '{type(new_verbose).__name__}' was assigned to it.")
+            raise TypeError(f"Attribute 'verbose' should be a boolean but an object of type '{type(new_verbose).__name__}' was assigned to it")
         self._verbose = new_verbose
 
     # ----
 
     # == Plot Enable Flag ==
 
     @property
@@ -425,134 +880,176 @@
 
         ### See Also
 
         * [PWL Plotter](#pwl-plotter)
         """
 
         if (not _has_matplotlib) and self._verbose:
-            print(
-                "Optional features deactivated. Using the plot_flag does nothing in this case.")
+            print("Optional features deactivated. Using the plot_flag does nothing in this case")
 
         return self._plot_flag
 
     @plot_flag.setter
     def plot_flag(self, new_plot_flag: bool) -> None:
 
         if not isinstance(new_plot_flag, bool):
-            raise TypeError(
-                f"Attribute 'plot_flag' should be a boolean but an object of type '{type(new_plot_flag).__name__}' was assigned to it.")
+            raise TypeError(f"Attribute 'plot_flag' should be a boolean but an object of type '{type(new_plot_flag).__name__}' was assigned to it")
 
         if (not _has_matplotlib) and self._verbose:
-            print(
-                "Optional features deactivated. Using the plot_flag does nothing in this case.")
+            print("Optional features deactivated. Using the plot_flag does nothing in this case")
 
         self._plot_flag = new_plot_flag
 
     # ----
 
+    # == Initial Condition ==
+
+    def initial(self, x0: float = 0) -> "PWL":
+        """**`initial` method of `PWL` class**
+
+        ### Summary
+
+        Method that sets the initial condition for the `PWL` object.
+
+        ### Parameters
+
+        * `x0` (`float`, optional) : Initial condition for `t=0`.
+
+        ### Returns
+
+        * `PWL` : Returns the object itself.
+
+        ### Raises
+
+        * `TypeError` : Raised if `x0` is not a real number.increasing.
+        * `InitialConditionError` : Raised if the object already has initial conditions.
+        """
+
+        if not isinstance(x0, Real):
+            raise TypeError(f"Argument 'x0' should be a real number but has type '{type(x0).__name__}'")
+        if len(self) != 0:
+            raise InitialConditionError(f"PWL object already has initial condition of {self.x_list[0]}")
+
+        self._insert(0, x0)
+
+        return self
+
+    # ----
+
     # == Last Value Holder ==
 
-    def hold(self, duration: float) -> None:
+    def hold(self, duration: float) -> "PWL":
         """**`hold` method of `PWL` class**
 
         ### Summary
 
         Method that holds the last value from the previous event for a given duration.
 
         If the `PWL` object is empty, adds the point `(0, 0)` and holds that.
 
         ### Parameters
 
         * `duration` (`float`) : Duration to hold the last value for. Should be strictly positive.
 
+        ### Returns
+
+        * `PWL` : Returns the object itself.
+
         ### Raises
 
         * `TypeError` : Raised if `duration` is not a real number.
         * `ValueError` : Raised if `duration` is not strictly positive.
         * `PrecisionError` : Raised if computational noise causes the time coordinates to not be strictly increasing.
         """
 
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive but has value of {duration}")
 
         if self._verbose:
-            print(f"{self._name}: Adding hold with duration of {duration}.")
+            print(f"{self._name}: Adding hold with duration of {duration}")
 
         if len(self._t_list) == len(self._x_list) == 0:
             if self._verbose:
-                print("    Empty PWL object. Adding initial (0, 0) point.")
-            self._add(0, 0)
+                print("    Empty PWL object. Adding initial (0, 0) point")
+            self._insert(0, 0)
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
-        self._add(last_t+duration, last_x)
+        self._insert(last_t+duration, last_x)
+
+        return self
 
     # ----
 
     # == Linear Transition ==
 
-    def lin_transition(self, target: float, duration: float) -> None:
+    def lin_transition(self, target: float, duration: float) -> "PWL":
         """**`lin_transition` method of `PWL` class**
 
         ### Summary
 
         Method that generates a linear transition from the last value of the previous event to a given target with a given duration.
 
         If the `PWL` object is empty, adds the point `(0, 0)` and transitions from that.
 
         ### Arguments
 
         * `target` (`float`) : Value to transition to.
         * `duration` (`float`) : Duration of the transition. Should be strictly positive.
 
+         ### Returns
+
+        * `PWL` : Returns the object itself.
+
         ### Raises
 
         * `TypeError` : Raised if either `target` or duration` is not a real number.
         * `ValueError` : Raised if `duration` is not strictly positive.
         * `PrecisionError` : Raised if computational noise causes the time coordinates to not be strictly increasing.
         """
 
         if not isinstance(target, Real):
-            raise TypeError(
-                f"Argument 'target' should be a real number but has type '{type(target).__name__}'.")
+            raise TypeError(f"Argument 'target' should be a real number but has type '{type(target).__name__}'")
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive but has value of {duration}")
 
-        self._lin_transition(target, duration, 0)
+        self._nested_lin_transition(target, duration, 0)
+
+        return self
 
     # ----
 
     # == Rectangular Pulse ==
 
-    def rect_pulse(self, value: float, duration: float, t_step: Optional[float] = None) -> None:
+    def rect_pulse(self, value: float, duration: float, t_step: Optional[float] = None) -> "PWL":
         """**`rect_pulse` method of `PWL` class**
 
         ### Summary
 
         Method that generates a rectangular pulse with given amplitude and duration.
 
         If `duration` is less than or equal to `t_step` (`self.t_step` if `t_step` is not set), substitutes the pulse by a linear transition from the last value of the previous event to `value` with duration `t_step` (`self.t_step` if `t_step` is not set).
 
         ### Arguments
 
         * `value` (`float`) : Amplitude of the pulse.
         * `duration` (`float`) : Duration of the pulse. Should be strictly positive.
         * `t_step` (`float`, optional) : Transition time for the discontinuity. Should be strictly positive. If not set, uses `self.t_step`.
 
+         ### Returns
+
+        * `PWL` : Returns the object itself.
+
         ### Raises
 
         * `TypeError` : Raised if either `value`, duration` or `t_step` is not a real number.
         * `ValueError` : Raised if either `duration` or `t_step` is not strictly positive.
         * `PrecisionError` : Raised if computational noise causes the time coordinates to not be strictly increasing.
 
         ### See Also
@@ -560,54 +1057,50 @@
         * [Linear Transition](#linear-transition)
         """
 
         if t_step is None:
             t_step = self._t_step
 
         if not isinstance(value, Real):
-            raise TypeError(
-                f"Argument 'value' should be a real number but has type '{type(value).__name__}'.")
+            raise TypeError(f"Argument 'value' should be a real number but has type '{type(value).__name__}'")
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'")
         if not isinstance(t_step, Real):
-            raise TypeError(
-                f"Argument 't_step' should either be a real number but has type '{type(t_step).__name__}'.")
+            raise TypeError(f"Argument 't_step' should either be a real number but has type '{type(t_step).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive but has value of {duration}")
         if t_step <= 0:
-            raise ValueError(
-                f"Argument 't_step' should be strictly positive but has value of {t_step}.")
+            raise ValueError(f"Argument 't_step' should be strictly positive but has value of {t_step}")
 
         if self._verbose:
-            print(f"{self._name}: Adding rectangular pulse with value of {value}, duration of {duration} and time step of {t_step}.")
+            print(f"{self._name}: Adding rectangular pulse with value of {value}, duration of {duration} and time step of {t_step}")
 
         if duration <= t_step:
             if self._verbose:
-                print(
-                    f"{self._name}: Duration of {duration} is less than or equal to time step of {t_step}. Converting to linear transition.")
-            self._lin_transition(value, t_step, 1)
-            return
+                print(f"{self._name}: Duration of {duration} is less than or equal to time step of {t_step}. Converting to linear transition")
+            self._nested_lin_transition(value, t_step, 1)
+            return self
 
         if len(self._t_list) == len(self._x_list) == 0:
-            self._add(0, value)
+            self._insert(0, value)
             last_t = 0
         else:
             last_t = self._t_list[-1]
-            self._add(last_t+t_step, value)
+            self._insert(last_t+t_step, value)
 
-        self._add(last_t+duration, value)
+        self._insert(last_t+duration, value)
+
+        return self
 
     # ----
 
     # == Sawtooth Pulse ==
 
-    def sawtooth_pulse(self, start: float, end: float, duration: float, t_step: Optional[float] = None) -> None:
+    def sawtooth_pulse(self, start: float, end: float, duration: float, t_step: Optional[float] = None) -> "PWL":
         """**`sawtooth_pulse` method of `PWL` class**
 
         ### Summary
 
         Method that generates a sawtooth pulse with given starting and ending amplitudes and duration.
 
         If `duration` is less than or equal to `t_step` (`self.t_step` if `t_step` is not set), substitutes the pulse by a linear transition from the last value of the previous event to `end` with duration `t_step` (`self.t_step` if `t_step` is not set).
@@ -615,14 +1108,18 @@
         ### Arguments
 
         * `start` (`float`) : Amplitude at the start of the pulse.
         * `end` (`float`) : Amplitude at the end of the pulse.
         * `duration` (`float`) : Duration of the pulse. Should be strictly positive.
         * `t_step` (`float`, optional) : Transition time for the discontinuity. Should be strictly positive. If not set, uses `self.t_step`.
 
+         ### Returns
+
+        * `PWL` : Returns the object itself.
+
         ### Raises
 
         * `TypeError` : Raised if either `start`, `end`, duration` or `t_step` is not a real number.
         * `ValueError` : Raised if either `duration` or `t_step` is not strictly positive.
         * `PrecisionError` : Raised if computational noise causes the time coordinates to not be strictly increasing.
 
         ### See Also
@@ -630,57 +1127,52 @@
         * [Linear Transition](#linear-transition)
         """
 
         if t_step is None:
             t_step = self._t_step
 
         if not isinstance(start, Real):
-            raise TypeError(
-                f"Argument 'start' should be a real number but has type '{type(start).__name__}'.")
+            raise TypeError(f"Argument 'start' should be a real number but has type '{type(start).__name__}'")
         if not isinstance(end, Real):
-            raise TypeError(
-                f"Argument 'end' should be a real number but has type '{type(end).__name__}'.")
+            raise TypeError(f"Argument 'end' should be a real number but has type '{type(end).__name__}'")
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'")
         if not isinstance(t_step, Real):
-            raise TypeError(
-                f"Argument 't_step' should either be a real number but has type '{type(t_step).__name__}'.")
+            raise TypeError(f"Argument 't_step' should either be a real number but has type '{type(t_step).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive but has value of {duration}")
         if t_step <= 0:
-            raise ValueError(
-                f"Argument 't_step' should be strictly positive but has value of {t_step}.")
+            raise ValueError(f"Argument 't_step' should be strictly positive but has value of {t_step}")
 
         if self._verbose:
-            print(f"{self._name}: Adding sawtoth pulse from {start} to {end} with duration of {duration} and time step of {t_step}.")
+            print(f"{self._name}: Adding sawtoth pulse from {start} to {end} with duration of {duration} and time step of {t_step}")
 
         if duration <= t_step:
             if self._verbose:
-                print(
-                    f"{self._name}: Duration of {duration} is less than or equal to time step of {t_step}. Converting to linear transition.")
-            self._lin_transition(end, t_step, 1)
-            return
+                print(f"{self._name}: Duration of {duration} is less than or equal to time step of {t_step}. Converting to linear transition")
+            self._nested_lin_transition(end, t_step, 1)
+            return self
 
         if len(self._t_list) == len(self._x_list) == 0:
-            self._add(0, start)
+            self._insert(0, start)
             last_t = 0
         else:
             last_t = self._t_list[-1]
-            self._add(last_t+t_step, start)
+            self._insert(last_t+t_step, start)
+
+        self._insert(last_t+duration, end)
 
-        self._add(last_t+duration, end)
+        return self
 
     # ----
 
     # == Exponential Transition ==
 
-    def exp_transition(self, target: float, duration: float, tau: float, t_step: Optional[float] = None) -> None:
+    def exp_transition(self, target: float, duration: float, tau: float, t_step: Optional[float] = None) -> "PWL":
         """**`exp_transition` method of `PWL` class**
 
         ### Summary
 
         Method that generates an exponential transition from the last value of the previous event to a given target with a given duration.
 
         If the `PWL` object is empty, adds the point `(0, 0)` and transitions from that.
@@ -701,14 +1193,18 @@
         ### Arguments
 
         * `target` (`float`) : Value to transition to.
         * `duration` (`float`) : Duration of the transition. Should be strictly positive.
         * `tau` (`float`) : Time constant of the exponential. SHould be non zero.
         * `t_step` (`float`, optional) : Timestep between consecutive points inside the transition. Should be strictly positive. If not set, uses `self.t_step`.
 
+         ### Returns
+
+        * `PWL` : Returns the object itself.
+
         ### Raises
 
         * `TypeError` : Raised if either `target`, `duration`, tau` or `t_step` is not a real number.
         * `ValueError` : Raised if either `duration` or `t_step` is not strictly positive or `tau` is equal to zero.
         * `PrecisionError` : Raised if computational noise causes the time coordinates to not be strictly increasing.
 
         ### See Also
@@ -716,66 +1212,60 @@
         * [Linear Transition](#linear-transition)
         """
 
         if t_step is None:
             t_step = self._t_step
 
         if not isinstance(target, Real):
-            raise TypeError(
-                f"Argument 'target' should be a real number but has type '{type(target).__name__}'.")
+            raise TypeError(f"Argument 'target' should be a real number but has type '{type(target).__name__}'")
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'")
         if not isinstance(tau, Real):
-            raise TypeError(
-                f"Argument 'tau' should be a real number but has type '{type(tau).__name__}'.")
+            raise TypeError(f"Argument 'tau' should be a real number but has type '{type(tau).__name__}'")
         if not isinstance(t_step, Real):
-            raise TypeError(
-                f"Argument 't_step' should either be a real number but has type '{type(t_step).__name__}'.")
+            raise TypeError(f"Argument 't_step' should either be a real number but has type '{type(t_step).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive but has value of {duration}")
         if tau == 0:
-            raise ValueError("Argument 'tau' should be non zero.")
+            raise ValueError("Argument 'tau' should be non zero")
         if t_step <= 0:
-            raise ValueError(
-                f"Argument 't_step' should be strictly positive but has value of {t_step}.")
+            raise ValueError(f"Argument 't_step' should be strictly positive but has value of {t_step}")
 
         if self._verbose:
-            print(f"{self._name}: Adding exponential transition with target of {target}, time constant of {tau}, duration of {duration} and time step of {t_step}.")
+            print(f"{self._name}: Adding exponential transition with target of {target}, time constant of {tau}, duration of {duration} and time step of {t_step}")
 
         if duration <= t_step:
             if self._verbose:
-                print(
-                    f"    Duration of {duration} is less than or equal to time step of {t_step}. Converting to linear transition.")
-            self._lin_transition(target, t_step, 2)
-            return
+                print(f"    Duration of {duration} is less than or equal to time step of {t_step}. Converting to linear transition")
+            self._nested_lin_transition(target, t_step, 2)
+            return self
 
         if len(self._t_list) == len(self._x_list) == 0:
             if self._verbose:
-                print("    Empty PWL object. Adding initial (0, 0) point.")
-            self._add(0, 0)
+                print("    Empty PWL object. Adding initial (0, 0) point")
+            self._insert(0, 0)
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
-        f = _exp_transition_func(tau=tau, t1=last_t, t2=last_t +
-                                 duration, f1=last_x, f2=target)
+        f = exp_transition_func(tau=tau, t1=last_t, t2=last_t+duration, f1=last_x, f2=target)
 
         for t in np.arange(last_t+t_step, last_t+duration, t_step):
-            self._add(t, f(t))
+            self._insert(t, f(t))
+
+        self._insert(last_t+duration, target)
 
-        self._add(last_t+duration, target)
+        return self
 
     # ----
 
     # == Half Sine Transition ==
 
-    def sin_transition(self, target: float, duration: float, t_step: Optional[float] = None) -> None:
+    def sin_transition(self, target: float, duration: float, t_step: Optional[float] = None) -> "PWL":
         """**`sin_transition` method of `PWL` class**
 
         ### Summary
 
         Method that generates a half sine transition from the last value of the previous event to a given target with a given duration.
 
         If the `PWL` object is empty, adds the point `(0, 0)` and transitions from that.
@@ -796,14 +1286,18 @@
 
         ### Arguments
 
         * `target` (`float`) : Value to transition to.
         * `duration` (`float`) : Duration of the transition. Should be strictly positive.
         * `t_step` (`float`, optional) : Timestep between consecutive points inside the transition. Should be strictly positive. If not set, uses `self.t_step`.
 
+         ### Returns
+
+        * `PWL` : Returns the object itself.
+
         ### Raises
 
         * `TypeError` : Raised if either `target`, `duration` or `t_step` is not a real number.
         * `ValueError` : Raised if either `duration` or `t_step` is not strictly positive.
         * `PrecisionError` : Raised if computational noise causes the time coordinates to not be strictly increasing.
 
         ### See Also
@@ -811,61 +1305,57 @@
         * [Linear Transition](#linear-transition)
         """
 
         if t_step is None:
             t_step = self._t_step
 
         if not isinstance(target, Real):
-            raise TypeError(
-                f"Argument 'target' should be a real number but has type '{type(target).__name__}'.")
+            raise TypeError(f"Argument 'target' should be a real number but has type '{type(target).__name__}'")
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'")
         if not isinstance(t_step, Real):
-            raise TypeError(
-                f"Argument 't_step' should either be a real number but has type '{type(t_step).__name__}'.")
+            raise TypeError(f"Argument 't_step' should either be a real number but has type '{type(t_step).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive but has value of {duration}")
         if t_step <= 0:
-            raise ValueError(
-                f"Argument 't_step' should be strictly positive but has value of {t_step}.")
+            raise ValueError(f"Argument 't_step' should be strictly positive but has value of {t_step}")
 
         if self._verbose:
-            print(f"{self._name}: Adding sinusoidal transition with target of {target}, duration of {duration} and time step of {t_step}.")
+            print(f"{self._name}: Adding sinusoidal transition with target of {target}, duration of {duration} and time step of {t_step}")
 
         if duration <= t_step:
             if self._verbose:
-                print(
-                    f"    Duration of {duration} is less than or equal to time step of {t_step}. Converting to linear transition.")
-            self._lin_transition(target, t_step, n=2)
-            return
+                print(f"    Duration of {duration} is less than or equal to time step of {t_step}. Converting to linear transition")
+            self._nested_lin_transition(target, t_step, n=2)
+            return self
 
         if len(self._t_list) == len(self._x_list) == 0:
             if self._verbose:
-                print("    Empty PWL object. Adding initial (0, 0) point.")
-            self._add(0, 0)
+                print("    Empty PWL object. Adding initial (0, 0) point")
+            self._insert(0, 0)
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
-        f = _sin_transition_func(
+        f = sin_transition_func(
             t1=last_t, t2=last_t+duration, f1=last_x, f2=target)
 
         for t in np.arange(last_t+t_step, last_t+duration, t_step):
-            self._add(t, f(t))
+            self._insert(t, f(t))
+
+        self._insert(last_t+duration, target)
 
-        self._add(last_t+duration, target)
+        return self
 
     # ----
 
     # == Smoothstep Transition ==
 
-    def smoothstep_transition(self, target: float, duration: float, t_step: Optional[float] = None) -> None:
+    def smoothstep_transition(self, target: float, duration: float, t_step: Optional[float] = None) -> "PWL":
         """**`smoothstep_transition` method of `PWL` class**
 
         ### Summary
 
         Method that generates a smoothstep transition from the last value of the previous event to a given target with a given duration.
 
         If the `PWL` object is empty, adds the point `(0, 0)` and transitions from that.
@@ -884,14 +1374,18 @@
 
         ### Arguments
 
         * `target` (`float`) : Value to transition to.
         * `duration` (`float`) : Duration of the transition. Should be strictly positive.
         * `t_step` (`float`, optional) : Timestep between consecutive points inside the transition. Should be strictly positive. If not set, uses `self.t_step`.
 
+         ### Returns
+
+        * `PWL` : Returns the object itself.
+
         ### Raises
 
         * `TypeError` : Raised if either `target`, `duration` or `t_step` is not a real number.
         * `ValueError` : Raised if either `duration` or `t_step` is not strictly positive.
         * `PrecisionError` : Raised if computational noise causes the time coordinates to not be strictly increasing.
 
         ### See Also
@@ -899,59 +1393,55 @@
         * [Linear Transition](#linear-transition)
         """
 
         if t_step is None:
             t_step = self._t_step
 
         if not isinstance(target, Real):
-            raise TypeError(
-                f"Argument 'target' should be a real number but has type '{type(target).__name__}'.")
+            raise TypeError(f"Argument 'target' should be a real number but has type '{type(target).__name__}'")
         if not isinstance(duration, Real):
-            raise TypeError(
-                f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'.")
+            raise TypeError(f"Argument 'duration' should be a real number but has type '{type(duration).__name__}'")
         if not isinstance(t_step, Real):
-            raise TypeError(
-                f"Argument 't_step' should either be a real number but has type '{type(t_step).__name__}'.")
+            raise TypeError(f"Argument 't_step' should either be a real number but has type '{type(t_step).__name__}'")
 
         if duration <= 0:
-            raise ValueError(
-                f"Argument 'duration' should be strictly positive but has value of {duration}.")
+            raise ValueError(f"Argument 'duration' should be strictly positive but has value of {duration}")
         if t_step <= 0:
-            raise ValueError(
-                f"Argument 't_step' should be strictly positive but has value of {t_step}.")
+            raise ValueError(f"Argument 't_step' should be strictly positive but has value of {t_step}")
 
         if self._verbose:
-            print(f"{self._name}: Adding smoothstep transition with target of {target}, duration of {duration} and time step of {t_step}.")
+            print(f"{self._name}: Adding smoothstep transition with target of {target}, duration of {duration} and time step of {t_step}")
 
         if duration <= t_step:
             if self._verbose:
-                print(
-                    f"    Duration of {duration} is less than or equal to time step of {t_step}. Converting to linear transition.")
-            self._lin_transition(target, t_step, n=2)
-            return
+                print(f"    Duration of {duration} is less than or equal to time step of {t_step}. Converting to linear transition")
+            self._nested_lin_transition(target, t_step, n=2)
+            return self
 
         if len(self._t_list) == len(self._x_list) == 0:
             if self._verbose:
-                print("    Empty PWL object. Adding initial (0, 0) point.")
-            self._add(0, 0)
+                print("    Empty PWL object. Adding initial (0, 0) point")
+            self._insert(0, 0)
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
-        f = _smoothstep_transition_func(
+        f = smoothstep_transition_func(
             t1=last_t, t2=last_t+duration, f1=last_x, f2=target)
 
         for t in np.arange(last_t+t_step, last_t+duration, t_step):
-            self._add(t, f(t))
+            self._insert(t, f(t))
 
-        self._add(last_t+duration, target)
+        self._insert(last_t+duration, target)
+
+        return self
 
     # ----
 
-    # == PWL File Writer ==
+    # == File Writer ==
 
     def write(self, filename: Optional[str] = None, precision: int = 10) -> None:
         """**`write` method of `PWL` class**
 
         ### Summary
 
         Method that takes a `PWL` object and writes a PWL file with it's `(t, x)` coordinates in scientific notation.
@@ -970,26 +1460,23 @@
         * `PrecisionError` : Raised if `precision` is such that the rounding causes the time coordinates to not be strictly increasing.
         """
 
         if filename is None:
             filename = f'{self._name}.txt'
 
         if not isinstance(filename, str):
-            raise TypeError(
-                f"Argument 'filename' should be a string but has type '{type(filename).__name__}'.")
+            raise TypeError(f"Argument 'filename' should be a string but has type '{type(filename).__name__}'")
         if not isinstance(precision, int):
-            raise TypeError(
-                f"Argument 'precision' should be an integer but has type '{type(precision).__name__}'.")
+            raise TypeError(f"Argument 'precision' should be an integer but has type '{type(precision).__name__}'")
 
         if precision <= 0:
-            raise ValueError(
-                f"Argument 'precision' should be strictly positive but has value of {precision}.")
+            raise ValueError(f"Argument 'precision' should be strictly positive but has value of {precision}")
 
         if self._verbose:
-            print(f"{self._name}: Writing PWL file to {filename}.")
+            print(f"{self._name}: Writing PWL file to {filename}")
 
         t_list = self._t_list
         x_list = self._x_list
 
         with open(filename, "w") as file:
             ti_str = np.format_float_scientific(
                 t_list[0], precision-1, unique=False, sign=False)
@@ -999,67 +1486,95 @@
             last_t = ti_str
             for ti, xi in zip(t_list[1:], x_list[1:]):
                 ti_str = np.format_float_scientific(
                     ti, precision-1, unique=False, sign=False)
                 xi_str = np.format_float_scientific(
                     xi, precision-1, unique=False, sign=True)
                 if ti_str == last_t:
-                    raise PrecisionError(
-                        "The chosen precision level caused the written time coordinates to not be strictly increasing.")
+                    raise PrecisionError("The chosen precision level caused the written time coordinates to not be strictly increasing")
                 file.write(
                     f"{ti_str}    {xi_str}\n")
                 last_t = ti_str
 
     # ----
 
+    # == Object Copy ==
+
+    def copy(self, name: Optional[str] = None) -> "PWL":
+        """**`copy` class method of `PWL` class**
+
+        ### Summary
+
+        Method that creates a deep copy of a `PWL` object.
+
+        ### Arguments
+
+        * `name` (`str`, optional) : Name of the `PWL` object used for verbose output printing. Should not be empty. If not set, automatically generates a name based on already taken names. 
+
+        ### Returns
+
+        * `PWL`
+
+        ### Raises
+
+        * `TypeError` : Raised if `name` is not a string.
+        * `ValueError` : Raised if `name` is either empty or already taken.
+        """
+
+        new_pwl = PWL(t_step=self.t_step, name=name, verbose=self.verbose)
+
+        new_pwl._t_list = self.t_list
+        new_pwl._x_list = self.x_list
+
+        return new_pwl
+
+    # ----
+
     # == PWL Plotter ==
 
     @classmethod
     def plot(cls, merge: bool = False) -> None:
         """**`plot` class method of `PWL` class**
         *Optional feature: Requires matplotlib*
 
         ### Summary
 
         Class method that takes all instances of the `PWL` class with plot enable flag set to `True` and plots them on the same time axis.
 
         ### Arguments
 
-        * `merge` (`bool`, optional) : Flag indicating if all signals should be ploted on the same strip or separeted. If not set, defaults to False.
+        * `merge` (`bool`, optional) : Flag indicating if all signals should be ploted on the same strip or separeted. If not set, defaults to `False`.
 
         ### Raises
 
         * `TypeError` : Raised if `merge` is not a boolean.
         * `ImportError` : Raised if the matplotlib package is not installed.
 
         ### See Also
 
         * [Plot Enable Flag](#plot-enable-flag)
         """
 
         if not _has_matplotlib:
-            raise ImportError(
-                "Optional plotting features are deactivated. Install matplotlib to use.")
+            raise ImportError("Optional plotting features are deactivated. Install matplotlib to use")
 
         if not isinstance(merge, bool):
-            raise TypeError(
-                f"Argument 'merge' should be a boolean but has type '{type(merge).__name__}'.")
+            raise TypeError(f"Argument 'merge' should be a boolean but has type '{type(merge).__name__}'")
 
         dict_of_objects = {key: pwl for key,
                            pwl in cls.__dict_of_objects.items() if pwl.plot_flag}
 
         if not dict_of_objects:
             return None
 
         if merge:
             axs = plt.subplots(nrows=1, sharex=True, squeeze=False)[1]
             axs = np.repeat(axs, len(dict_of_objects))
         else:
-            axs = plt.subplots(nrows=len(dict_of_objects),
-                               sharex=True, squeeze=False)[1]
+            axs = plt.subplots(nrows=len(dict_of_objects), sharex=True, squeeze=False)[1]
             axs = axs.flatten()
         x_max: float = 0
 
         for key, ax in zip(dict_of_objects, axs):
             pwl = dict_of_objects[key]
             if not pwl._plot_flag:
                 continue
@@ -1069,174 +1584,105 @@
             label = pwl.name
             ax.plot(x_list, y_list)
             ax.set_ylabel(label)
 
         axs[0].set_xlim(xmin=0, xmax=x_max)
         plt.show()
 
-    # = Private Methods and Functions =
-
-    # From this point forward, all listed methods and functions are not intended to be used by the user. Brief descriptions will be provided, but documentation will be kept to a minimum.
-
     # ----
 
-    # == PWL Point Adder ==
-
-    def _add(self, t: float, x: float) -> None:
-        """**`_add` private method of `PWL` class**
-
-        Private method that adds a `(t, x)` point to a `PWL` object of any size.
-        """
-
+    def _insert(self, t: float, x: float) -> None:
         if len(self._t_list) >= 1 and t <= self._t_list[-1]:
-            raise PrecisionError(
-                f"Internal Python rounding caused the time coordinates to not be strictly increasing when adding points to {self._name}.")
+            raise PrecisionError(f"Internal Python rounding caused the time coordinates to not be strictly increasing when adding points to {self._name}")
 
         if len(self._t_list) == len(self._x_list) < 2:
             self._t_list.append(t)
             self._x_list.append(x)
         else:
             self._colinear_eliminator(x, t)
 
-    # ----
-
-    # == Colinear Points Eliminator ==
-
     def _colinear_eliminator(self, x: float, t: float) -> None:
-        """**`_colinear_eliminator` private method of `PWL` class**
-
-        Private method that adds a `(t, x)` point to a `PWL` object with 2 or more points without consecutive colinear points.
-        """
-
         t_n_1 = self._t_list[-1]
         t_n_2 = self._t_list[-2]
 
         x_n_1 = self._x_list[-1]
         x_n_2 = self._x_list[-2]
 
         last_m = (x_n_1 - x_n_2)/(t_n_1 - t_n_2)
         new_m = (x - x_n_1)/(t - t_n_1)
 
-        if last_m == new_m:
+        if is_within(last_m, new_m):
             self._t_list[-1] = t
             self._x_list[-1] = x
         else:
             self._t_list.append(t)
             self._x_list.append(x)
 
-    # ----
-
-    # == Nested Linear Transition ==
-
-    def _lin_transition(self, target: float, duration: float, n: int) -> None:
-        """**`_lin_transition` private method of `PWL` class**
-
-        Private method to generate a linear transition. The difference between this method and the [public linear transition](#linear-transition) method is that this method prints indented verbose output when called from within any of the public methods that revert to a linear transition in certain conditions.
-        """
-
+    def _nested_lin_transition(self, target: float, duration: float, n: int) -> None:
         if self._verbose:
             if n == 0:
-                print(
-                    f"{self._name}: Adding linear transition with target of {target} and duration of {duration}.")
+                print(f"{self._name}: Adding linear transition with target of {target} and duration of {duration}")
             else:
-                print(
-                    n*"    "+f"Adding linear transition with target of {target} and duration of {duration}.")
+                print(n*"    "+f"Adding linear transition with target of {target} and duration of {duration}")
 
         if len(self._t_list) == len(self._x_list) == 0:
             if self._verbose:
-                print((n+1)*"    "+"Empty PWL object. Adding initial (0, 0) point.")
-            self._add(0, 0)
+                print((n+1)*"    "+"Empty PWL object. Adding initial (0, 0) point")
+            self._insert(0, 0)
 
         last_t = self._t_list[-1]
-        self._add(last_t+duration, target)
-
-# ----
-
-# == Exponential Function Generator ==
+        self._insert(last_t+duration, target)
 
 
-def _exp_transition_func(tau: float, t1: float, f1: float, t2: float, f2: float) -> Callable[[float], float]:
-    """**`_exp_transition_func` private function**
-
-    Private function that generates an exponential function passing trough 2 fixed points.
-    """
-
-    A: float = (f1*np.exp(t1/tau) - f2*np.exp(t2/tau)) / \
-        (np.exp(t1/tau) - np.exp(t2/tau))
+def exp_transition_func(tau: float, t1: float, f1: float, t2: float, f2: float) -> Callable[[float], float]:
+    A: float = (f1*np.exp(t1/tau) - f2*np.exp(t2/tau)) / (np.exp(t1/tau) - np.exp(t2/tau))
     B: float = (f1 - f2)/(np.exp(-t1/tau) - np.exp(-t2/tau))
 
     def f(t: float) -> float:
         result: float = A + B*np.exp(-t/tau)
         return result
 
     return f
 
-# ----
-
-# == Sinusoidal Function Generator ==
-
-
-def _sin_transition_func(t1: float, f1: float, t2: float, f2: float) -> Callable[[float], float]:
-    """**`_sin_transition_func` private function**
-
-    Private function that generates a sinusoidal function passing trough 2 fixed points.
-    """
 
+def sin_transition_func(t1: float, f1: float, t2: float, f2: float) -> Callable[[float], float]:
     fm: float = (f1+f2)/2
     tm: float = (t1+t2)/2
     T: float = 2*(t2-t1)
     w: float = 2*np.pi/T
     phi: float = w*tm
     A: float = f2-fm
 
     def f(t: float) -> float:
         result: float = fm + A*np.sin(w*t - phi)
         return result
 
     return f
 
-# ----
-
-# == Smoothstep Function Generator ==
-
-
-def _smoothstep_transition_func(t1: float, f1: float, t2: float, f2: float) -> Callable[[float], float]:
-    """**`_smoothstep_transition_func` private function**
-
-    Private function that generates a smoothstep function passing trough 2 fixed points.
-    """
 
+def smoothstep_transition_func(t1: float, f1: float, t2: float, f2: float) -> Callable[[float], float]:
     Am = np.array([[1, t1, t1**2, t1**3],
                    [1, t2, t2**2, t2**3],
                    [0, 1, 2*t1, 3*t1**2],
                    [0, 1, 2*t2, 3*t2**2]])
     Bm = np.array([f1, f2, 0, 0])
     A, B, C, D = np.linalg.solve(Am, Bm)
 
     def f(t: float) -> float:
         result: float = A + B*t + C*t**2 + D*t**3
         return result
 
     return f
 
-# ----
 
+def is_within(x: float, y: float, tol: float = 0.01) -> float:
+    error = 0 if x == y else 2*abs(x-y)/(abs(x)+abs(y))
 
-if __name__ == "__main__":
-    pwl0 = PWL(0.001)
-    pwl1 = PWL(0.001)
+    return error <= tol
 
-    pwl0.hold(1)
-    pwl1.hold(1)
 
-    pwl0.sin_transition(1, 1)
-    pwl1.sin_transition(-1, 1)
-
-    pwl0.hold(1)
-    pwl1.hold(1)
-
-    pwl0.sin_transition(0, 1)
-
-    pwl1.plot_flag = False
+if __name__ == "__main__":
+    t = PWL(0.01, name="t").lin_transition(10, 10)
+    x = -(1/3)*(t**3)+5*(t**2)-15*t
+    x.name = "x"
 
-    PWL.plot(merge=False)
-    print(pwl0(1.5))
+    PWL.plot()
```

### Comparing `pwl_writer-1.1.3/pyproject.toml` & `pwl_writer-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "pwl_writer"
 authors = [{name = "Victor Sabiá P. Carpes", email = "victorscarpes@gmail.com"}]
 readme = "README.md"
 requires-python = ">=3.6.6"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
-dependencies = ["numpy"]
+dependencies = ["numpy >= 1.13"]
 
 [project.optional-dependencies]
 plot = ["matplotlib"]
 doc = ["pycco"]
 
 [project.urls]
 Documentation = "https://htmlpreview.github.io/?https://github.com/victorscarpes/pwl_writer/blob/main/docs/pwl_writer.html"
```

### Comparing `pwl_writer-1.1.3/PKG-INFO` & `pwl_writer-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pwl_writer
-Version: 1.1.3
+Version: 1.2.0
 Summary: Package to generate PWL files incrementally using little 'events' like rectangular pulses and exponential rising or falling edges.
 Author-email: "Victor Sabiá P. Carpes" <victorscarpes@gmail.com>
 Requires-Python: >=3.6.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: numpy
+Requires-Dist: numpy >= 1.13
 Requires-Dist: pycco ; extra == "doc"
 Requires-Dist: matplotlib ; extra == "plot"
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/victorscarpes/pwl_writer/blob/main/docs/pwl_writer.html
 Project-URL: Source, https://github.com/victorscarpes/pwl_writer
 Provides-Extra: doc
 Provides-Extra: plot
```

