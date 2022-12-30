# UnityVectorSwizzle
Vector swizzle extension class for Unity engine.
# What is swizzling
Swizzling is the ability to compose vectors by arbitrarily rearranging and combining components of other vectors.
https://en.wikipedia.org/wiki/Swizzling_(computer_graphics)
# How to use
You can compose arbitrarily rearranging any components of vector you want.<br>And you can even compose "0" and "1" as well.

## Examples
Vector2 to Vector2
```
Vector2 v = new Vector3(x, y)._x0(); // v = (x, 0)
Vector2 v = new Vector3(x, y)._yy(); // v = (y, y)
```
Vector3 to Vector3
```
Vector3 v = new Vector3(x, y, z)._x1z(); // v = (x, 1, z)
Vector3 v = new Vector3(x, y, z)._xxx(); // v = (x, x, x)
```
Vector3 to Vector2
```
Vector2 v = new Vector3(x, y, z)._0y(); // v = (0, y)
Vector2 v = new Vector3(x, y, z)._xz(); // v = (x, z)
```
Vector2 to Vector3
```
Vector3 v = new Vector2(x, y)._x1y(); // v = (x, 1, y)
Vector3 v = new Vector2(x, y)._xxx(); // v = (x, x, x)
```
You can also swizzle vector4 as well.
# Support Type
- Vector2
- Vector3
- Vector4
- Vector2Int
- Vector3Int
- Quaternion
