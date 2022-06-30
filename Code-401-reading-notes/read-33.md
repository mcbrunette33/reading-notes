## Read 33

- The @hasOne and @hasMany directives do not support referencing a model which then references the initial model via @hasOne or @hasMany if DataStore is enabled.

- Under the hood, @hasMany configures a secondary index on the related table to enable you to query the related model from the source model.

-  actions represented as callbacks tend to be either scattered across the code or deeply nested inside each other. 

- Java 8 introduced the CompletableFuture class. Along with the Future interface, it also implemented the CompletionStage interface. 

- CompletableFuture is at the same time a building block and a framework, with about 50 different methods for composing, combining, and executing asynchronous computation steps and handling errors.

- If we already know the result of a computation, we can use the static completedFuture method with an argument that represents a result of this computation.

- Static methods runAsync and supplyAsync allow us to create a CompletableFuture instance out of Runnable and Supplier functional types correspondingly.

- Both Runnable and Supplier are functional interfaces that allow passing their instances as lambda expressions thanks to the new Java 8 feature.

- The Runnable interface is the same old interface that is used in threads and it does not allow to return a value.

- The Supplier interface is a generic functional interface with a single method that has no arguments and returns a value of a parameterized type.

