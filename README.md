🔷 What is the DRY Principle?
DRY stands for Don't Repeat Yourself.
It was introduced in the book "The Pragmatic Programmer" by Andy Hunt and Dave Thomas, and it states:

🔷 DRY — The Core Idea
The DRY principle aims to reduce repetition of code, logic, or knowledge across your system. If a piece of logic, rule, or data structure is duplicated in multiple places:
It becomes harder to maintain
Increases the chance of bugs
Leads to inconsistencies

Makes scaling the system harder
DRY is not just about writing less code — it's about writing better-structured code that’s easier to manage and change.
----------------------------------------------------------------------------------------------------------------------------------------------------------------------

🔷 Understanding “Repetition” in Depth

There are different kinds of repetition:
1. 🔸 Code Repetition
Same block of code exists in multiple places.

🧱 Example (Anti-DRY):
int area1 = length1 * width1;
int area2 = length2 * width2;

✅ DRY version:
int calculateArea(int length, int width) {
    return length * width;
}
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
2. 🔸 Logic Repetition
Same business logic is repeated — not necessarily the same code.

🧱 Example:
// Check if a user is an adult
if (age >= 18) { ... }
// Later
if (person.getAge() >= 18) { ... }


