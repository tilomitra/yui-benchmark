#YUI-Benchmark

These files demonstrate how you can write BenchmarkJS tests and compare performance across different YUI versions. This is done by using Ryan Grove's (rgrove) `multi.js` module for YUI, which creates an iFrame and exposes a YUI instance.

##Files

* `event-custom-benchmark.js`: Just a sample file with some benchmarkJS tests.
* `index.html`: This is what your main test HTML page should look like. Pulls down all the relevant modules + BenchmarkJS
* `multi.js`: Module written by Ryan Grove that lets you dump a version of YUI inside an iFrame on the page.

##Instructions

To integrate Benchmark tests into your component with the ability to compare performance across different YUI version, I recommend the following steps:

* Using the `index.html` in the repo as a template. Note that you'll need to change some paths in the file for it to work with your directory structure.
* Using the `event-custom-benchmark.js` file as a template for writing performance tests.
* Pulling in `multi.js` into `yui3/src/common/` and referencing it from there.
