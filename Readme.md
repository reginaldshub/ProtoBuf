# Protocol Buffers:

> “Protocol Buffers are a way of encoding structured data in an efficient yet extensible format.”

Google developed Protocol Buffers for use in their internal services. It is a binary encoding format that allows you to specify a schema for your data using a specification language, like so:

```message Person {
  required int32 id = 1;
  required string name = 2;
  optional string email = 3;
}
```
> “New fields could be easily introduced, and intermediate servers that didn’t need to inspect the data could simply parse it and pass through the data without needing to know about all the fields.”

### Why Protocol Buffers?

* Schemas Are Awesome
* Backward Compatibility For Free
* Less Boilerplate Code
* Validations and Extensibility
* Easy Language Interoperability

### When to use JSON?
* You need or want data to be human readable
* Data from the service is directly consumed by a web browser
* Your server side application is written in JavaScript
* You aren’t prepared to tie the data model to a schema
* You don’t have the bandwidth to add another tool to your arsenal
* The operational burden of running a different kind of network service is too great


## Running the code:

### Installation 
> Node.js

```npm install protobufjs [--save --save-prefix=~]
```
```html 
var protobuf = require("protobufjs");
```

> Browsers

```<script src="//cdn.rawgit.com/dcodeIO/protobuf.js/6.X.X/dist/protobuf.js"></script>
<script src="//cdn.rawgit.com/dcodeIO/protobuf.js/6.X.X/dist/protobuf.min.js"></script>
```


