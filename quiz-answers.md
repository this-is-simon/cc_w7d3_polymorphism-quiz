# cc_w7d3_polymorphism-quiz

Polymorphism
What does the word 'polymorphism' mean?
Polymorphism means that objects of a certain class can potentially be treated as objects of another class.

What does it mean when we apply polymorphism to OO design? Give a simple Java example.
It means that we can in effect group together objects of different classes into one super class, or give them shared behaviours based on an interface.
For example we may have several classes for different devices that can be connected to a Computer superclass, like a Printer and a Scanner. If we implement a shared interface IConnectables we can then refer to our Printer and Scanner object as "connectables" and create an array list within Computer of connectable objects.

What can we use to implement polymorphism in Java?
We can use superclasses and interfaces.

How many 'forms' can an object take when using polymorphism?
I think it can in theory take an unlimited number of forms.

Give an example of when you could use polymorphism.
If we had a Cafe superclass with subclasses for various sub classes of cups and glasses, we could group them by their shared behaviour and refer to them as "drinkingReceptacles" using an interface, IDrinkable. In our Cafe class we could have a hash map of drinkingReceptacles which groups all the cups and glasses together, for example when loading a Dishwasher class.

Composition
What do we mean by 'composition' in reference to object-oriented programming?
We mean the designing the architecture of various modules within a programme so that the programme can run in a way that makes sense. We would focus on being able to group certain behaviours and characteristics without repeating ourselves more than necessary, and having as many different moving parts as we need to not be overly dependent on other parts. For example if we were composing a car we would be sure to have a body, wheels and a steering wheel; we want both the wheels and the steering wheel to be able to share a 'turn' behaviour, but we don't want the programme to be written in such a way that when we change a wheel the steering wheel also changes.

When would you use composition? Provide a simple example in Java.
If you were creating a Library project, you could begin with a super class of Reading Materials and another super class of People. People might be divided into Borrowers and Staff and would all have shared characteristics such as having a name and being able to borrow a book. In the sub class of Staff, staff would have a method to be able to borrow a book for a longer length of time than a Borrower. Reading Materials could be split into Magazines, Books and Reference Materials, and Magazines and Books could share an interface of Borrawable but Reference Materials would not.

What is/are the advantage(s) of using composition?
Composition allows you to plan and design your programme so that you don't back yourself into a corner.

What happens to the behaviours when the object composed of them is destroyed?
If the behaviours belong to the object then the behaviours will also cease to exist, but if the behaviours belong to a superclass or interface then they will continue to live within the system.
