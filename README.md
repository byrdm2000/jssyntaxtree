# jsSyntaxTree
_jsSyntaxTree_ is a web application that creates syntax tree graphs 
from phrases entered in labelled bracket notation. jsSyntaxTree 
generated graphs can be used in linguistic homework, assignments 
and other documents.

See the LICENSE file for license information.

## Changes from upstream
The changes I (byrdm2000) made to this project was adding an option to remove connections from the part-of-speech tag to the label, as the syntax class I am taking (24.902 at MIT) requires syntax trees to be drawn without a connector to leaves, unless a triangle is drawn instead.

## Building and Running
jsSyntaxTree can be built with Docker like so:
```
$ docker build -t jssyntaxtree .
```
and then ran with Docker:
```
$ docker run -dp <port>:80 jssyntaxtree
```

For example, if you want to host it on port 3000, you would run 
```
$ docker run -dp 3000:80 jssyntaxtree
```

The web application will then be available at http://localhost:3000 (or whatever port you choose).

## Support, Questions etc.
If you encounter any bugs or problems, please file a bug report or contact the developers
on the upstream jsSyntaxTree project page:
http://github.com/int2str/jssyntaxtree
