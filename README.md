[![NPM](https://nodei.co/npm/@bonnie/class.png?downloads=true)](https://nodei.co/npm/@bonnie/class/)

a super small javascript Inheritance framework 

<pre>
  var Vehicle = Class.Create({
    init: function(wheels) {
      this.wheels = wheels;
    }
  });

  var Truck = Vehicle.Extend({
    init: function(hp, wheels) {
      this._super(wheels);
      this.horsepower = hp;
    },
    printInfo: function() {
      console.log('I am a truck and I have ' + this.wheels +
        ' wheels and ' + this.horsepower + ' hp.');
    }
  });
  
  var t = new Truck(350, 4);
  t.printInfo();
</pre>
