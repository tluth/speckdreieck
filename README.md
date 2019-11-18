# speckdreieck

Speckdreieck is a small collection of utilities to help facilitate the creation of Speckle mesh objects from generic geometric data. 

This came about from wanting to upload building models in various unsupported file types to speckle streams. The issue that kept coming up was that planar surfaces are usually described as a list of vertices ordered anti-clockwise around the perimeter of the surface. However, to make a speckle mesh object we need to specify the order in which these vertices are triangulated. 

The [implementation](https://github.com/joshuaskelly/earcut-python) of the earcut algorithm used for triangulating surfaces was created by [joshuaskelly](https://github.com/joshuaskelly). Thanks :) 

### Installation

Install and update using pip:

```sh
$ pip install speckdreieck
```

### Usage

```python 
my_surface = ["a bunch of verts"]
speckle_mesh = create_ya_thing(my_surface)
send_it_up 

```

License
----

MIT

**Free Software, Hell Yeah!**
