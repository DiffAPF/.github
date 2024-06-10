<div align="center">
<h1>Differentiable All-pole Filters for Time-varying Audio Systems</h1>

<p>
    <a href="https://yoyololicon.github.io/" target=”_blank”>Chin-Yun Yu</a>,
    <a href="https://christhetr.ee/" target=”_blank”>Christopher Mitcheltree</a>,
    <a href="https://www.linkedin.com/in/alistair-carson-a6178919a/" target=”_blank”>Alistair Carson</a>,
    <a href="https://www.acoustics.ed.ac.uk/group-members/dr-stefan-bilbao/" target=”_blank”>Stefan Bilbao</a>,
    <a href="https://www.eecs.qmul.ac.uk/~josh/" target=”_blank”>Joshua D. Reiss</a>, and
    <a href="https://www.eecs.qmul.ac.uk/~gyorgyf/about.html" target=”_blank”>György Fazekas</a>
</p>

[![arXiv](https://img.shields.io/badge/arXiv-2404.07970-b31b1b.svg)](https://arxiv.org/abs/2404.07970)
[![Listening Samples](https://img.shields.io/badge/%F0%9F%94%8A%F0%9F%8E%B6-Listening_Samples-blue)](https://diffapf.github.io/web/)
[![Plugins](https://img.shields.io/badge/neutone-Plugins-blue)](https://diffapf.github.io/web/index.html#plugins)
[![License](https://img.shields.io/badge/License-MPL%202.0-orange)](https://www.mozilla.org/en-US/MPL/2.0/FAQ/)
</div>

<h2>Abstract</h2>
<p>
Infinite impulse response filters are an essential building block of many time-varying audio systems, such as audio effects and synthesisers.
However, their recursive structure impedes end-to-end training of these systems using automatic differentiation.
Although non-recursive filter approximations like frequency sampling and frame-based processing have been proposed and widely used in previous works, they are approximations and cannot accurately reflect the gradient of the original system.
We alleviate this difficulty by re-expressing a time-varying all-pole filter to backpropagate the gradients through itself, so the filter implementation is not bound to the technical limitations of automatic differentiation frameworks.
This implementation can be employed within any audio system containing filters with poles for efficient gradient evaluation.
We demonstrate its training efficiency and expressive capabilities for modelling real-world dynamic audio systems on a phaser, time-varying subtractive synthesiser, and feed-forward compressor.
We make our code available and provide the trained audio effect and synth models in a VST plugin.
</p>

<hr>
<h2>Citation</h2>

Accepted to the 27th International Conference on Digital Audio Effects (DAFx24), Guildford, United Kingdom, 3 - 7 September 2024.

<pre><code>@inproceedings{ycy2024diffapf,
    title={Differentiable All-pole Filters for Time-varying Audio Systems},
    author={Chin-Yun Yu and Christopher Mitcheltree and Alistair Carson and Stefan Bilbao and Joshua D. Reiss and György Fazekas},
    booktitle={International Conference on Digital Audio Effects (DAFx)},
    year={2024}
}
</code></pre>
