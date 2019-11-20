# Clean Code: Smells and Heuristics

Taken from Uncle Bob's Clean Code.

## Comments

C1: Inappropriate Information Reserve comments for technical notes referring to code and design.  
C2: Obsolete Comment Update or delete obsolete comments.  
C3: Redundant Comment A redundant comment describes something able to sufficiently describe itself.  
C4: Poorly Written Comment Comments should be brief, concise, correctly spelled.  
C5: Commented-Out Code Ghost code. Delete it.

## Environment

E1: Build Requires More Than One Step Builds should require one command to check out and one command to run.  
E2: Tests Require More Than One Step Tests should be run with one button click through an IDE, or else with one command.

## Functions

F1: Too Many Arguments Functions should have no arguments, then one, then two, then three. No more than three.  
F2: Output Arguments Arguments are inputs, not outputs. If somethings state must be changed, let it be the state of the called object.  
F3: Flag Arguments Eliminate boolean arguments.  
F4: Dead Function Discard uncalled methods. This is dead code.

## General

G1: Multiple Languages in One Source File Minimize the number of languages in a source file. Ideally, only one.  
G2: Obvious Behavior is Unimplemented The result of a function or class should not be a surprise.  
G3: Incorrect Behavior at the Boundaries Write tests for every boundary condition.  
G4: Overridden Safeties Overriding safeties and exerting manual control leads to code melt down.  
G5: Duplication Practice abstraction on duplicate code. Replace repetitive functions with polymorphism.  
G6: Code at Wrong Level of Abstraction Make sure abstracted code is separated into different containers.  
G7: Base Classes Depending on Their Derivatives Practice modularity.  
G8: Too Much Information Do a lot with a little. Limit the amount of things going on in a class or functions.  
G9: Dead Code Delete unexecuted code.  
G10: Vertical Separation Define variables and functions close to where they are called.  
G11: Inconsistency Choose a convention, and follow it. Remember no surprises.  
G12: Clutter Dead code.  
G13: Artificial Coupling Favor code that is clear, rather than convenient. Do not group code that favors mental mapping over clearness.  
G14: Feature Envy Methods of one class should not be interested with the methods of another class.  
G15: Selector Arguments Do not flaunt false arguments at the end of functions.  
G16: Obscured Intent Code should not be magic or obscure.  
G17: Misplaced Responsibility Use clear function name as waypoints for where to place your code.  
G18: Inappropriate Static Make your functions nonstatic.  
G19: Use Explanatory Variables Make explanatory variables, and lots of them.  
G20: Function Names Should Say What They Do ...  
G21: Understand the Algorithm Understand how a function works. Passing tests is not enough. Refactoring a function can lead to a better understanding of it.  
G22: Make Logical Dependencies Physical Understand what your code is doing.  
G23: Prefer Polymorphism to If/Else or Switch/Case Avoid the brute force of switch/case.  
G24: Follow Standard Conventions It doesn't matter what your teams convention is. Just that you have on and everyone follows it.  
G25: Replace Magic Numbers with Named Constants Stop spelling out numbers.  
G26: Be Precise Don't be lazy. Think of possible results, then cover and test them.  
G27: Structure Over Convention Design decisions should have a structure rather than a dogma.  
G28: Encapsulate Conditionals Make your conditionals more precise.  
G29: Avoid Negative Conditionals Negative conditionals take more brain power to understand than a positive.  
G30: Functions Should Do One Thing  
G31: Hidden Temporal Couplings Use arguents that make temporal coupling explicit.  
G32: Don’t Be Arbitrary Your code's sturcture should communicate the reason for its structure.  
G33: Encapsulate Boundary Conditions Avoid leaking +1's and -1's into your code.  
G34: Functions Should Descend Only One Level of Abstraction The toughest heuristic to follow. One level of abstraction below the function's described operation can help clarify your code.  
G35: Keep Configurable Data at High Levels High level constants are easy to change.  
G36: Avoid Transitive Navigation Write shy code. Modules should only know about their neighbors, not their neighbor's neighbors.

## Names

N1: Choose Descriptive Names Choose names that are descriptive and relevant.  
N2: Choose Names at the Appropriate Level of Abstraction Think of names that are still clear to the user when used in different programs.  
N3: Use Standard Nomenclature Where Possible Use names that express their task.  
N4: Unambiguous Names Favor clearness over curtness. A long, expressive name is better than a short, dull one.  
N5: Use Long Names for Long Scopes A name's length should relate to its scope.  
N6: Avoid Encodings No not encode names with type or scope information.  
N7: Names Should Describe Side-Effects Consider the side-effects of your function, and include that in its name.

## Tests

T1: Insufficient Tests Test everything that can possibly break  
T2: Use a Coverage Tool! Use your IDE as a coverage tool.  
T3: Don’t Skip Trivial Tests ...  
T4: An Ignored Test is a Question about an Ambiguity If your test is ignored, the code is brought into question.  
T5: Test Boundary Conditions The middle is usually covered. Remember the boundaries.  
T6: Exhaustively Test Near Bugs Bugs are rarely alone. When you find one, look nearby for another.  
T7: Patterns of Failure Are Revealing Test cases ordered well will reveal patterns of faiure.  
T8: Test Coverage Patterns Can Be Revealing Similarly, look at the code that is or is not passed in a failure.  
T9: Tests Should Be Fast Slow tests won't get run.
