# spring-boot-cheat-sheet

## Building RESTful web services:

1. Add maven dependency to pom.xml: spring-boot-starter-web
2. **Annotations(@):**

a) RestController: define RESTful web services. Serves Json, XML or custom response.

b) Request Mapping: define Request URI to access REST endpoints.The default request method is GET.

        @RequestMapping(value="/products") 
        public ResponseEntity<Object> getProducts() { }
        
c)@RequestBody annotation is used to define the request body content type.

      public ResponseEntity<Object> createProduct(@RequestBody Product product) { }
d)@PathVariable annotation is used to define the custom or dynamic request URI. The 
Path variable in request URI is defined as curly braces {}.

        public ResponseEntity<Object> updateProduct(@PathVariable("id") String id) { }
e)@RequestParam annotation is used to read the request parameters from the Request URL.By default,it is a required parameter.

    public ResponseEntity<Object> getProduct(@RequestParam(value="name", 
    required=false, defaultValue="honey") String name) { 
    }
    
 3.** Method and API**
 
  a) GET API: 
  b) POST:
  c) PUT:
  d) DELETE: 
