# LAB-8 (STL)

Write a program that does the following:
* Reads a phrase / sentence from a text file into a **std::string** object
* Split the phrase in words. Consider that the following characters are separators (space, comma, question and exclamation mark, point). Words may be separated by multiple spaces. Use only methods available in the **std::string** class for this task
* Create a **std::map** object that counts how many times each word is encountered. Don't take word casing into consideration (case-insensitive).
* Use a **std::priority_queue** to sort each word using the number of times it was found. if two words have the same number of appearance in the phrase, they will be sorted lexicographically.
* Print the words after they are sorted

**Example:**
* Let's assume that we have a file that contains the following phrase: "***I bought an apple. Then I eat an apple. Apple is my favorite.***"
* First we create a MAP with the following items:
    ```
    {
        "i" : 2,
        "bought" : 1,
        "an" : 2,
        "apple" : 3,
        "then" : 1,
        "eat" : 1,
        "is" : 1,
        "my" : 1,
        "favorite" : 1
    }
    ```
* Then we sort these words based on the amount of time we found them and lexycographically
* Finally - we will print the following
  * ```apple => 3```
  * ```an => 2```
  * ```i => 2```
  * ```bought => 1```
  * ```eat => 1```
  * ```favorite => 1```
  * ```is => 1```
  * ```my => 1```
  * ```then => 1```