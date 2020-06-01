# JavaScript Object Graphs with Python

This Python module serializes and deserializes cyclic object graphs in the [JSOG format](https://github.com/simoneggler/jsog-python).

## Source code

The fork history:
(https://github.com/simoneggler/jsog-python) 
-> (https://github.com/jsog/jsog-python) 
-> (https://github.com/markrowsoft/jsog-python) .

## Download

pyjsog - comming soon

## Usage

This code mimics the standard *json* python package:

    from jsog3 import jsog

	string = jsog.dumps(cyclicGraph);
	cyclicGraph = jsog.loads(string);

It can be used to convert between object graphs directly:

    from jsog3 import jsog

	jsogStructure = jsog.encode(cyclicGraph);	// has { '@ref': 'ID' } links instead of cycles
	cyclicGraph = jsog.decode(jsogStructure);

## Authors

* Jeff Schnitzer (jeff@infohazard.org)
* Simon Eggler (simon.eggler@gmx.net)

## License

This software is provided under the [MIT license](http://opensource.org/licenses/MIT)
