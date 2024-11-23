A tensor is a generalization of vectors and matrices to potentially higher dimentions. They are the main object passed in the program. It store it in the graphs.

They are charaterized by:
- a datatype(float32, int32, string, ...)
- a shape(the dimension of data)

They could have some degrees or ranks (the dimensions):
- 0 (also known as **scalar**, is one value) es: `"test"`
- 1 (is a vector of values) es: `["test", "test2"]` 
- N (is a vector of N-1 vectors) es: `[["test", "test2"], ["hello", "ciao"]]`