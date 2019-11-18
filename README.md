# speckdreieck

Speckdreieck is a small collection of utilities to help facilitate the creation of [Speckle](https://speckle.systems/) mesh objects from generic geometric data. 

This came about from wanting to upload building models in various unsupported file types to speckle streams. The issue that kept coming up was that planar surfaces are usually described as a list of vertices ordered anti-clockwise around the perimeter of the surface. However, to make a speckle mesh object we need to specify the order in which these vertices are triangulated. 

The of the earcut algorithm used for triangulating surfaces was created by [joshuaskelly](https://github.com/joshuaskelly). Thanks :) 

### Installation

Install and update using pip:

```sh
$ pip install speckdreieck
```

### Usage

```python 
my_surface = ["a bunch of verts"]
properties = {}
mesh = parse_vertices(my_surface, properties)
new_stream("hestia.speckle.works", "My Stream", "A stream containing a surface")

```

License
----

MIT

**Free Software, Hell Yeah!**
