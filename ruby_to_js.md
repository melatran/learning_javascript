# Making the Switch From Ruby to JavaScript

## Syntax
**Ruby Method**
```
def speak
  puts "Hello!"
end
```

**JS Method**
```
function speak(){
  return "Hello!"
}
```

**Objects**
- Ruby `.class` to figure what the element is
- JS `typeof` to figure what the element is

**To Integers**
- Ruby `.to_i`
- JS requires a `parseInt()`

**Incrementing Shortcut**
- Ruby `x += 1`
- JS `x++`

**When do I use brackets and parenthesis in JS?**
- parenthesis `()` are used for function calls, to surround conditional statements, or grouping to enforce Order of Operations

```
function myFunc() {
  if (condition 1) {

  }
  if ((1 + 2) * 3) {
    //different from (1 + 2 * 3)
  }
}
```

- braces `{}` are used during declarion of object literals or to enclose blocks of code

```
var objLit = {
  a: "I am an Object Literal"
};
```

**Arrays**
JavaScript:
```
const pets = ['MoMo', 'Milo', 'Chloe']
function addPet(name) {
  pets.push(name)
}
```

Ruby:
```
pets = ['MoMo', 'Milo', 'Chloe']

def add_pet(name)
  pets << name
end
```

**Variables**
- both languages arrays indexes start at [0]

Ruby: store variables using `=`

```
dog = "Momo"
dog = {name: "MoMo", age: 5, personality: "brat"}
```

JS: `const`, `var`, or `let`

```
const dog = "MoMo"
```

**Methods**
Ruby: use keywords `def` and `end`
JS: function { } where the curly braces serve as the def and end

**Iterations**
Ruby:

```
players = {
  name: 'James',
  age: 8
},
{
  name: 'Lucifer',
  age: 9
}

def iterate
  players.each {|player| player.name}
end
```

JS:

```
function findMatching(drivers, string){
  return drivers.filter(function (name) {
    return (name.toLowerCase() === string.toLowerCase())
  });
}
```

**Object Oriented Programming**
Ruby:

```
class Pet
  attr_accessor :name, :age

  def initialize(name, age)
    @name = name
    @age = age
  end

  def bark(phrase)
    puts "{#phrase}
  end
end
```

JS:

```
function User (name, email) {
  this.name = name;
  this.email = email;

  this.sayHello = function(){
    returns `Hello, my name is ${this.name}`
  };
}
```
