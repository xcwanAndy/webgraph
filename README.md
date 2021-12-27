Welcome to WebGraph!
--------------------

[WebGraph](http://webgraph.di.unimi.it/) is a framework for graph
compression aimed at studying web graphs. It provides simple ways to
manage very large graphs, exploiting modern compression techniques.

This version of WebGraph is limited to graphs with at most 2^31 nodes. For
larger graphs, have a look at the [big
version](https://github.com/vigna/webgraph-big).

Building
--------

You need [Ant](https://ant.apache.org/) and [Ivy](https://ant.apache.org/ivy/).
Then, run `ant ivy-setupjars jar`.

seba (<mailto:sebastiano.vigna@unimi.it>)

Setup Deps
--------

```
# copy webgraph-deps to $DEPS
cd ~ && rm -rf deps && mkdir deps
cp webgraph/jars/compile/*.jar ~/deps

# copy webgraph to $DEPS
cp webgraph/webgraph-3.6.10.jar ~/deps
```

Run Program
--------
```
java -cp "~deps/*" it.unimi.dsi.webgraph.BVGraph -o -O -L ~/uk-2007-01
```
