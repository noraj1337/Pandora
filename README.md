# Pandora (BETA)

**Export Maltego Graphs to JSON format**

This means you can import them into Splunk, ElasticSearch or anything else that accepts JSON.

## Installation

```
$ git clone https://github.com/SneakersInc/Pandora.git && cd Pandora
$ pip install -r requirements.txt
```

## Command Line Export

To run a simple export you can use the command line as below:

```
$ ./pandora.py ExampleGraph.mtgx
```

This will save the new json file to `output/ExampleGraph.json`.

## Web Interface

You can also use the web interface to export and view the output. To start the web server just run:

```
$ ./webserver.py
```

This will start a small Flask web server on port 5000.

This is just the beginning of the project so more updates will come.

## Python version

Pandora works only with Python 2 (not compatible with Python 3 yet).

So if your OS has `python3` as default `python` you will need to run `pip2` and `python2`.

Examples:
+ `$ pip2 install -r requirements.txt` for the installation
+ `$ python2 ./pandora.py ExampleGraph.mtgx` to convert mtgx to json
