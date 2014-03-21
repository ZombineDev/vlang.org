<h2>Language Features</h2>

<p>On the contrary with the state of art verification languages which has decade old root, Vlang has been developed recently and thus it understand modern verification and simulation needs better. Vlang offers features which caters the need of a futuristic verification suit and test bench development. Inheriting clean and well designed syntax &amp; semantics, advanced object orientation, multicore programming features from D AND by implementing verification features &amp; UVM, Vlang brings in great value for any design verification engineer. A list of important features of Vlang has been enumerated as follows:</p>

<ol>
<li><h3>Multicore Support</h3>

<p>With the increase in number of cores, speed of each core is no more increasing. In future there will be more and more cores possibly each of them with reduced speed. And with this your old good reuse model is no more scalable with your favorite simulator. Vlang provides and supports multiple levels of multicore concurrency to address the growing trend of multicore system usability. </p>

<ul>
<li><strong>User Level Concurrency:</strong> Vlang offers temporal language concurrency as offered by other verification languages. Processes, fork-join, events et al. are the part of this category. </li>
<li><strong>Hierarchical Concurrency:</strong> Vlang offers hierarchical concurrency in which execution of different RootEntry are computed using parallel computing resulting faster simulation. By the virtue of this capability of Vlang, user can create as many simulator he/she wishes. </li>
<li><strong>Language Level Concurrency:</strong> D offers powerful features on multicore concurrent computation which will benefit the development of test benches. Computationally heavy portion of the test bench and models can be made multi-threaded for faster execution. </li>
</ul></li>
<li><h3>Compatibility with other Languages</h3>

<p>Vlang is highly compatible with other languages commonly used in simulation and verification process.</p>

<ul>
<li><strong>C/C++/SystemC:</strong> D is <a href="http://en.wikipedia.org/wiki/Application_binary_interface">ABI compatible</a> with <a href="http://dlang.org/abi.html">C/C++</a>. By the virtue of this Vlang is interoperable with C/C++/SystemC and Vlang with C/C++/SystemC will create one single executable after linking.</li>
<li><strong>Verilog/SystemVerilog:</strong> Vlang implements <a href="http://en.wikipedia.org/wiki/Verilog_Procedural_Interface">VPI</a> interface of Verilog Standard and hence Verilog models can be integrated seamlessly with Vlang.</li>
<li><strong>VHDL:</strong> Vlang implements <a href="http://www.eda.org/VIUF_proc/Fall96/DUNLOP96A.PDF">VHPI</a> interface of VHDL Standard and hence VHDL models can be integrated seamlessly with Vlang. </li>
<li><strong>MATLAB:</strong> Golden models written in <a href="http://en.wikipedia.org/wiki/MATLAB">MATLAB</a> can be seamlessly integrated with Vlang through matlab-mex interfaces.</li>
</ul></li>
<li><h3>Constrained Randomization and Other Features</h3>

<p>Vlang implements a very powerful and sophisticated <a href="http://en.wikipedia.org/wiki/Binary_decision_diagram">BDD</a> based Constrained Randomization engine. Commonly encountered features of other verification languages like pre randomization, post randomization, random arrays et. al. are supported. The lightweight nature of Vlang implementation make the constrained randomization process lightning fast. Other important verification features like processes, routines, fork-join, events &amp; notifications, ports &amp; channels, lightweight data-types (added to D's rich native data-types), hierarchical test benches et. al. comes naturally with Vlang.</p></li>
<li><h3>UVM Implementation</h3>

<p>Vlang implements a word-to-word translation of SystemVerilog <a href="http://en.wikipedia.org/wiki/Universal_Verification_Methodology">UVM</a> version 1.1d in order to provide an access to existing use models. The UVM port of Vlang is completely concurrent to provide lightning fast simulation speed. Vlang aspires to augment the UVM implementation with Standard Template Models (STM) in future.</p></li>
<li><h3>Efficiency</h3>

<p>Vlang takes the advantage of D compiler's lightning fast compilation feature. The test bench compiles and elaborates in seconds for complex test benches. This leads to a drastic reduction in verification time in comparison to the verification time lost on compilation &amp; elaboration with state of the art verification languages. Lightweight nature of Vlang makes simulation task lightning fast when it is compared to other languages.</p></li>
<li><h3>Opensource License</h3>

<p>The core language part of Vlang (known as ESDL) is released under Boost Software License and the UVM part of Vlang is released under Apache 2.0 License. This means the source code is available with you and you can modify and distribute it without have to share the source code. The licensing strategy of Vlang is academia fiendly and industry productive. The open source nature of Vlang  is an outlook of developers through which the aspiration is to promote further verification language research.</p></li>
</ol>

<h2>Adopting Vlang</h2>

<p>Vlang has been designed for easy adoption. The language features are standard with extension in power towards every direction, brings in a value as modern verification language. Following points give a brief overview on adoption friendly nature of Vlang:</p>

<ol>
<li>A short learning curve for C++/SystemC/SystemVerilog programmers. Competent programmers should be able to understand the entire language without great effort.</li>
<li>No need of memory management, garbage collector is built into the language.</li>
<li>Unit testing is built into the language.</li>
<li>When necessary, down and dirty to the metal coding should be supported. This mean easy maintanence and no coding guilelines needed.</li>
<li>Vlang is pointer-less! You do not need to use any pointer in Vlang unless you really need it. </li>
<li>Extremely fast during compilation and simulation – No waste of time during elaboration.</li>
<li>Easy or no training for begineers.</li>
<li>Very powerful object orientation, supporting generic programming, which means more robust models possibly and hence no or trivial adoption neede for models across different test suit.</li>
</ol>

<p>Vlang is open source which means your internal design verification team can build a superset on the top of it. The Boost License allows you to share binary-only version to your customer. If you are a heavy UVM user, Vlang provides a word-to-word translated SV UVM which is multicore enabled resulting in a much more faster speed in comparison to SV UVM. The constrained random solver in Vlang instantiates many copies of BDD runnng on seperate threads making it lightening fast. The open source nature of Vlang encourages it to be researched in academia and used in industrial productivity environment as well. In near future, models and methodologies written on Vlang will be scalable with the increase in number of processor cores due to Vlang's concurrency feature. D compiler takes care of performance enhancement of dirty codes and hence no need of code review/management and coding guidelines.</p>

<h2>Vlang and You</h2>
