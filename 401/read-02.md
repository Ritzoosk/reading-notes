# Node Ecosystem, TDD


### Describe (in plain English) what Array.map() does

- array.map CREATES a NEW array containing all the results of the appilcable function
- [array.map](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map) 


### Describe (in plain English) what Array.reduce() does


- array.reduce reduces an array into a single output 
- [array.reduce](https://www.javascripttutorial.net/javascript-array-reduce/) 


### Provide code snippets showing how to use superagent() to fetch data from a URL and log the result With normal Promise .then() syntax Again with async / await syntax


#### .then
- "function newSearch(req, res){
  console.log('newSearch', req.body);
  try{
    superagent.get(`https://www.googleapis.com/books/v1/volumes?q=in${req.body.selection}:${req.body.userInput}& limit=10`)
    .then(bookData => {
  
      //console.log("bookData", bookData.body);
      
      const bookCameBack = bookData.body.items.map(outputPrep);
      function outputPrep(info){
        return new Bookbuild(info)
      }
      res.render('pages/searches/show', {bookFront : bookCameBack})
    });
    } catch(error){
      res.render('pages/error.ejs', {errorThatComesBack : error})
  }
  
}"
- my book app

### async / await

- "const foo = async function() {
  // the function containing this code would 
  try {
    let res = await request.executeQuery(params);
    if (_inFlightQueryMetadata) {
      _inFlightQueryMetadata.abort();
    }
    _inFlightQueryMetadata = request.queryMetadata(res.queryId);
    res = await _inFlightQueryMetadata;
    if (res.metadata.something) {
      res = await request.optionalThirdStep(res.metadata);
      // do something with third step res
    } else {
      // do something with second step res
    }
  } catch (err) {
    // handle the error (we can handle all errors for all requests in this one handler if we choose)
    return;
  }
};" - https://www.honeycomb.io/blog/es7-await-async-and-superagent/


### Explain promises as though you were mentoring a Code 301 level student Are all callback functions considered to be Asynchronous? Why or Why Not?

- a promise is an object that will get assign later. It will then exist in one of 3 states 
  - fulfilled
  - rejected
  - pending
- Depends what is being promised. when the promise involves external resources it will be asynchronos.