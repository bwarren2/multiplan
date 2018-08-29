# Multiplan Creation and Use

---

#### Wants

* Allow default and specialized programs for students that are associated (Math vs Math for Astronauts)
* Assignments are managed automatically or outside EAB (scalability)

---

#### Sample flow

![Foo](img/mockup.jpg)

(This is why I am a server dev.)

---

#### How the data structures work right now

![Foo](img/current.jpg)

---

#### Option 1: assign multiple templates to a program

![Foo](img/templating.jpg)

---

#### Upsides

* Intuitive to traverse the relationships as you drill down in the content admin
* Matches how we think of "specializations within a program"

#### Challenges

* Credits are currently marked at the ProgramDefinition level.  Different slot sets could have different credits.
* Migration of code.  How much of our existing codebase codifies the table hierarchy as-is?

---

#### Inferences

* Our current construction of a ProgramDefinition is the natural container for "a thing with program slots"


---

#### Option 2: assign programs to a category

![Foo](img/categorization.jpg)

---

#### Upsides

* Adds new structure rather than changing existing structure

#### Challenges

* Less intuitive.  In order to say "things that are like this", you need to go thing -> category -> things in category

---

#### Sample update flow

![Foo](img/state_diagram.jpg)




