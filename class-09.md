## Instance methods
* Instances of Models are documents. Documents have many of their own built-in instance methods. We may also define our own custom document instance methods.
* Overwriting a default mongoose document method may lead to unpredictable results. See this for more details.
* Do not declare methods using ES6 arrow functions (=>). Arrow functions explicitly prevent binding this, so your method will not have access to the document and the above examples will not work.
## Static methods
### You can also add static functions to your model. There are two equivalent ways to add a static
* Add a function property to schema.statics
* Call the Schema#static() function
* Do not declare statics using ES6 arrow functions (=>). Arrow functions explicitly prevent binding this, so the above examples will not work because of the value of this.