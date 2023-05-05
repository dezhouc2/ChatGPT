# ChatGPT
  
  * ask-response principle:
    - Querying
      - extract keywords from query and match these keywords with corresponding nodes,pass nodes into response module
    
    - Indexing
      - split a text document into small chunks and index each small chunks respectively
      
      - each small chunk is regarded as a node
      
      - node1 -> node2 -> node3 (a sequence of indexes regards as a complete document as response passing into response module)
    
    - Response Module
      - definition: a class that input a set of nodes and output a response

      - Create and refine
        - definition: a way of generating a response

        - info in first node + query = initial answer; pass this initial answer + second query + info in second node as input = second better answer; so on and on
