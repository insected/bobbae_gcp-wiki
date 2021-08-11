[JSONPath](https://goessner.net/articles/JsonPath/) is a query language for [JSON](https://www.json.org/json-en.html), similar to [XPath](https://en.wikipedia.org/wiki/XPath) for [XML](https://en.wikipedia.org/wiki/XML).

JSONPath expressions always refer to a JSON structure in the same way as XPath expression are used in combination with an XML document. Since a JSON structure is usually anonymous and doesn't necessarily have a "root member object" JSONPath assumes the abstract name $ assigned to the outer level object.

JSONPath expressions can use the dot–notation

$.store.book[0].title

or the bracket–notation

$['store']['book'][0]['title']

for input pathes. Internal or output pathes will always be converted to the more general bracket–notation.

JSONPath allows the wildcard symbol * for member names and array indices. It borrows the descendant operator '..' from E4X and the array slice syntax proposal [start:end:step] from ECMASCRIPT 4.

Expressions of the underlying scripting language (<expr>) can be used as an alternative to explicit names or indices as in

$.store.book[(@.length-1)].title

using the symbol '@' for the current object. Filter expressions are supported via the syntax ?(<boolean expr>) as in

$.store.book[?(@.price < 10)].title

## Example

Given JSON structure:

```
{ "store": {
    "book": [ 
      { "category": "reference",
        "author": "Nigel Rees",
        "title": "Sayings of the Century",
        "price": 8.95
      },
      { "category": "fiction",
        "author": "Evelyn Waugh",
        "title": "Sword of Honour",
        "price": 12.99
      },
      { "category": "fiction",
        "author": "Herman Melville",
        "title": "Moby Dick",
        "isbn": "0-553-21311-3",
        "price": 8.99
      },
      { "category": "fiction",
        "author": "J. R. R. Tolkien",
        "title": "The Lord of the Rings",
        "isbn": "0-395-19395-8",
        "price": 22.99
      }
    ],
    "bicycle": {
      "color": "red",
      "price": 19.95
    }
  }
}
```


| XPath	| JSONPath	| Result |
|---------|--------------|--------|
|/store/book/author|	$.store.book[*].author	|the authors of all books in the store|
|//author	|$..author|	all authors|
|/store/*	|$.store.*	|all things in store, which are some books and a red bicycle.|
|/store//price|	$.store..price	|the price of everything in the store.|
|//book[3]|	$..book[2]	|the third book|
|//book[last()]|	$..book[(@.length-1)] or  $..book[-1:]	|the last book in order.|
|//book[position()<3]|	$..book[0,1] or $..book[:2]	|the first two books|
|//book[isbn]	|$..book[?(@.isbn)]|	filter all books with isbn number|
|//book[price<10]	|$..book[?(@.price<10)]	|filter all books cheapier than 10|
|//*	|$..*	|all Elements in XML document. All members of JSON structure.|


# jq

[jq](https://stedolan.github.io/jq/) is like sed for JSON data - you can use it to slice and filter and map and transform structured data with the same ease that sed, awk, grep and friends let you play with text.

The syntax used by `jq` is not JSONPath.  It is a custom syntax.  https://stedolan.github.io/jq/manual/

jq, while being more powerful than JSONPath, nevertheless enables one to write queries that are usually as simple as, and sometimes even simpler than, the corresponding JSONPath queries.  

For example, the XPath expression:
```
/store/book[1]/title
```
would look like this in JSONPath:
```
$.store.book[0].title
```
and like this in [JSON Pointer](https://tools.ietf.org/html/rfc6901):
```
/store/book/0/title
```
and like this in jq:
```
.store.book[0].title
```
One important point about jq here is that jq is stream-oriented: the jq expression shown above can be run not just against a single object, but also against a stream of objects.  

In general, given a stream of JSON entities as input, jq will produce a stream of outputs. The input entities may be any mix of any JSON types, not just objects or arrays.

https://github.com/stedolan/jq/wiki/For-JSONPath-users



# jp

[jp](https://github.com/bobbae/jp) is a program that can be used to grok json at the command line via path expressions. 

