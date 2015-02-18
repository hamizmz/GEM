# GEMs
Graham's Easy Models

## Create your model!
  
    function Person() {
      var secret = 'I still pick my nose and I am 26 years old.'; // just a private variable
      this.prenom = 'Graham';
      this.nom = 'Robertson';
      this.surnom = 'Ham';
      this.age = 26;
      
      // Extend a Gem!
      this.extend = Gem;
      this.extend();
    };

## Create an instance!
    var graham = new Person();

## Listen to events!!
    graham.subscribe('age', function(val) {
      alert('Wow! ' + graham.prenom + ' a ' + val + ' ans là.  Très cool!');
    });

## Change values that trigger events!
    graham.age = 27; // Not until September 14th, 2015 though...

## And that's all!
Have fun :)
