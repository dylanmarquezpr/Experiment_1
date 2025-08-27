**Experiment 1 - Introduction to Python Programming**

**Name: Dylan Rvy A. Marquez**
**Section: 2ECE-B**
**Date: 08/25/2025**

**OVERVIEW**

The task basically covers the basics of Python programming through three problems: arranging letters alphabetically, replacing words with emoticons, and unpacking list elements. These serve as practice for handling strings, dictionaries, and lists, while also applying Python’s built-in functions in solving simple tasks.

**1. ALPHABET SOUP PROBLEM**

The Alphabet Soup Problem is designed to practice string manipulation. The task is to create a function that arranges the letters of a word in alphabetical order. The program defines a function called alphabet_soup(word), which accepts a word as input. Inside the function, the sorted() function is applied to break the word into characters and arrange them alphabetically. Since the result of sorted() is a list, the ''.join() method is then used to combine the characters back into a single string.

**PROCEDURE :**

1. Define the function alphabet_soup(word).
   
` def alphabet_soup(word): #DEFINE DUNCTION `

2. Use sorted() to arrange the characters in alphabetical order. Apply ''.join() to reassemble the characters into a string.

`return '' .join(sorted(word)) #SORT LETTERS`

3. Accept user input using input().

`word = input("Type a word: ") #USER INPUT `

7. Pass the input word to the function and print the result.

`print(alphabet_soup(word))`

**OUTPUT :**

<img width="273" height="43" alt="Screenshot 2025-08-27 215035" src="https://github.com/user-attachments/assets/c144cf50-eb88-4db9-8125-b957a1890412" />



For example, when the user types SirNikkoLobos, the program outputs the same letters in alphabetical order. This shows how simple built-in functions can make text manipulation efficient and very straightforward in Python.

**2. EMOTICON PROBLEM**

The Emoticon Problem demonstrates the use of dictionaries and string replacement. A dictionary named emoticons is created, where each keyword such as "smile", "grin", "sad", and "mad" is mapped to its corresponding emoticon. A function called emote(sentence) is then defined to take a sentence as input. The program loops through the dictionary and uses the .replace() method to substitute every occurrence of the keywords with their emoticon equivalents.

**PROCEDURE :**

1. Create a dictionary mapping words to emoticons. Define the function emote(sentence) to process the text and use a for-loop to check each word in the dictionary.

```
def emote(sentence):
    emoticons = {      #DICTIONARY MAPPING FROM KEYWORD
        "smile": ":)",
        "grin": ":D",
        "sad": ":((",
        "mad": ">:("
    }
    for word, emo in emoticons.items():
```

2. Replace the words in the sentence with their corresponding emoticons using .replace(). Return and print the modified sentence.

```
sentence = sentence.replace(word, emo) # REPLACE EVERY OCCURENCE OF 'WORD' WITH ITS EMOTICON
    return sentence
print(emote("Make me smile!"))
print(emote("I am mad."))
print(emote("She gave me a grin."))
print(emote("Engineering makes me sad."))

```

**OUTPUT :** 

<img width="236" height="89" alt="Screenshot 2025-08-27 215055" src="https://github.com/user-attachments/assets/f24cd37d-3fdb-44fc-926d-84142ff90456" />



For instance, the input sentence “Make me smile!” becomes “Make me :)!” while “I am mad.” becomes “I am >:(.” Similarly, “She gave me a grin.” is transformed into “She gave me a :D.” and “Engineering makes me sad.” becomes “Engineering makes me :((.” This demonstrates how Python dictionaries can act as lookup tables and how text can be modified dynamically using string methods.

**3. UNPACKING LIST PROBLEM**

The Unpacking List Problem focuses on separating the first, middle, and last elements of a list. A predefined list is given as [1, 2, 3, 4, 5, 6]. The goal is to assign the first element to first, the last element to last, and the remaining elements in between to middle. This is accomplished using list methods. The .pop(0) method removes and returns the first element, which is then stored in the variable first. The .pop(-1) method removes and returns the last element, which is stored in the variable last. The elements left in the list represent the middle section, which is stored in the variable middle.

**PROCEDURE :** 

1. Define a list with values [1, 2, 3, 4, 5, 6].

`lst = [1, 2, 3, 4, 5, 6] #CREATE LIST`

2.. Use .pop(0) to extract the first element.

`first = lst.pop(0)   #REMOVE AND RETURN FIRST ELEMENT`

3. Use .pop(-1) to extract the last element.

`last = lst.pop(-1)   #REMOVE AND RETURN LAST ELEMENT`

4. Assign the remaining values to middle.

`middle = lst         #REMAINING LIST`

5. Print the three variables to display the results.
    
```
print("first:", first)
print("middle:", middle)
print("last:", last)
```

**OUTPUT :**

<img width="190" height="66" alt="Screenshot 2025-08-27 215203" src="https://github.com/user-attachments/assets/664fc724-5a27-4480-ba0f-45b4b9816e1f" />



The program takes the list [1, 2, 3, 4, 5, 6] and divides it into three parts. The first element, which is 1, is removed and stored in the variable first, while the last element, 6, is removed and stored in the variable last. The elements left in the list, [2, 3, 4, 5], are stored in the variable middle. When printed, the program clearly shows the separation of the list as first: 1, middle: [2, 3, 4, 5], and last: 6.
