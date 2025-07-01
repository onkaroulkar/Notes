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
2.  Use Enums Instead of Repeating State Checks
❌ Not DRY:
if (type.equals("CAR")) { ... }
else if (type.equals("TRUCK")) { ... }
else if (type.equals("BIKE")) { ... }

✅ DRY Version:
enum VehicleType { CAR, TRUCK, BIKE }

VehicleType type = VehicleType.CAR;

switch (type) {
    case CAR: ...
    case TRUCK: ...
    case BIKE: ...
}

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
✅ 6. Templates and Annotations (Spring / Java EE)
In frameworks like Spring, DRY applies at a high level using annotations and templates.

❌ Not DRY (boilerplate everywhere):
@RequestMapping(value = "/user", method = RequestMethod.GET)
@ResponseBody
public User getUser() { ... }

✅ DRY with simplification:
@GetMapping("/user")
public User getUser() { ... }

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
🔸 When NOT to Use DRY (Important!)
Sometimes duplication is better than the wrong abstraction. This is called:

Avoid premature DRY:
If two methods look similar but serve very different purposes, don’t force them into one method.
Don’t DRY too early — duplicate until patterns are clear.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
🔸 DRY in Testing
Even in test code, DRY applies.
❌ Not DRY:
@Test
public void testAddition() {
    Calculator c = new Calculator();
    assertEquals(5, c.add(2, 3));
}

@Test
public void testSubtraction() {
    Calculator c = new Calculator();
    assertEquals(1, c.subtract(3, 2));
}

✅ DRY with setup:
Calculator c;

@BeforeEach
public void setup() {
    c = new Calculator();
}

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
