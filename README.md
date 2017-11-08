# cereal-inline
This simple script allows to serialize values into/from JSON/XML/... archives 
without need to create enclosing parent node. 

Usage is simple:
```
using namespace cereal;

JSONInputArchive archive(stream);

MySerializable s;
load_inline(archive, s);
```

Note that this script doesn't work with versioned containers.
