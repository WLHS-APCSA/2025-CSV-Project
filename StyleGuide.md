# Java Style Guide (based on Google's)

## 1. Naming Conventions
Follow these rules to ensure your code matches official Java standards:

* **Classes:** Use `UpperCamelCase` (e.g., `AthleteProfile`, `DataManager`). Classes are **nouns**.
* **Methods:** Use `lowerCamelCase` (e.g., `calculateMean()`, `getName()`). Methods are **verbs**.
* **Variables:** Use `lowerCamelCase` (e.g., `goldMedals`, `tempList`). Avoid single letters like `x` or `g`.
* **Constants:** Use `UPPER_SNAKE_CASE` (e.g., `GOLD_VALUE`, `MAX_ROWS`) for `static final` variables.

## 2. Formatting & Whitespace
* **Indentation:** Use **4 spaces** per indent level. Do not use Tabs.
* **Braces:** Use "Egyptian Brackets"—the opening brace `{` stays on the same line as the code.
```java
if (score > 10) {
    System.out.println("High Score!");
}
```
* **Column Limit** Keep lines under 100 characters. Wrap long lines to the next line and indent.

## 3. JavaDocs
```markdown
## 3. Documentation (JavaDocs)
Every class and non-trivial method must have a JavaDoc comment block.

* **Class Headers:** Place above the class declaration.
* **Method Headers:** Place above the method to explain `@param` (parameters) and `@return`.

**Example:**
```java
/**
 * Calculates the weighted score based on medal types.
 * @param gold the number of gold medals won
 * @return the total calculated points
 */
public int calculateWeight(int gold) {
    // logic
}
```
## 4. Programming Best Practices
* **Avoid Magic Numbers:** Use named constants like `final int GOLD_POINTS = 3;` instead of raw numbers like `3`.
* **One Variable per Line:** Do not combine declarations (e.g., no `int x, y;`).
* **The "Vertical Rule":** Use blank lines to separate logical "paragraphs" of code within a method.
