#YUI-Benchmark

These files demonstrate how you can write BenchmarkJS tests and compare performance across different YUI versions. This is done by using Ryan Grove's (rgrove) `multi.js` module for YUI, which creates an iFrame and exposes a YUI instance.

##Files

* `event-custom-benchmark.js`: Just a sample file with some benchmarkJS tests.
* `index.html`: This is what your main test HTML page should look like. Pulls down all the relevant modules + BenchmarkJS
* `multi.js`: Module written by Ryan Grove that lets you dump a version of YUI inside an iFrame on the page.

##Instructions

To integrate Benchmark tests into your component with the ability to compare performance across different YUI version, I recommend the following steps:

1. Take what's in `index.html` but change the `multi.js` path from '<script src="multi.js"></script>' to 'https://raw.github.com/tilomitra/yui-benchmark/master/multi.js' so you don't have to download `multi.js` into your project. (Optionally, we could keep multi.js in `yui3/src/common/`).
2. You'll probably need to change the paths to the other modules so they reflect your project directory structure.