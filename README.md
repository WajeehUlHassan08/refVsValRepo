# refVsValRepo


Basic Intro 

Everytime we create an app, class, controller etc. it uses some of iPhone memory

Problems faced:

App much memory used:
- App uses too much of phone’s memory

e.g. a 2000 records loaded in an array, so it adds up to the memory. As a result, our app may crash and unexpected results can be encountered

- Orphans: 
Another problem is adding something to the memory and it never gets removed


- Missing:
You assign something to memory and then it unexpectedly got removed from the memory and when we reference it again or try to get value again, our app crashes because it doesn’t exist in memory anymore

We do memory handling in two ways

1- Value type
2- Reference type 

Value types can be things like String, Int, struct, enum, Bool, Array, Dictionary and how those things live in memory and how they get shared in memory is different from reference types. With value types, each instance holds on to its value,  and If you use it somewhere else, it makes a copy of that value and passes it around your application. Value types has no address in memory. In short, value types create copy. 

- Comparing instance data with == makes sense
- You want copies to have independent state
- The data will be used in code across multiple threads

Where as

Reference types are just single instance of an object and if you want to pass it around your application, instead of making a copy of it and passing it around, only one copy exist and instead you are just passing a pointer or a reference back to the single copy of your class. In short, there can be only one
- Subclasses of NSObject must be class types
- Comparing instance identity with === makes sense
- You want to create shared, mutable state





Flowchart for Reference vs Value type
![RefvsValFlowchart](/RefvsValFlowchart.png)
