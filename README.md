State is a behavioral design pattern that lets an object alter its behavior when its internal state changes. It appears as if the object changed its class.

The State pattern is closely related to the concept of a Finite-State Machine

The main idea is that, at any given moment, there’s a finite number of states which a program can be in. Within any unique state, the program behaves differently, and the program can be switched from one state to another instantaneously. However, depending on a current state, the program may or may not switch to certain other states. These switching rules, called transitions, are also finite and predetermined.

A behavior is defined on a state object that is responsible for running some handler when the overall state transitions to its own state. The interface that these state objects operate on is called the Context.

The way this pattern works in practice is that by delegating the work of certain actions to the state objects that represent a piece of the state, the action that represents the piece of the state is responsible for updating it from their handling of that state.

The most important problem this pattern solves is when your state becomes large and there are many cases. It becomes hard to debug issues when our application's state can change in many ways especially when our application becomes enormous.