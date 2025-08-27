<img width="273" height="43" alt="Screenshot 2025-08-27 215035" src="https://github.com/user-attachments/assets/89dc15c9-78a3-4e26-90ca-936fadcceb55" />Experiment 1 - Introduction to Python Programming

Name: Dylan Rvy A. Marquez
Section: 2ECE-B
Date: 08/25/2025

OVERVIEW

The task basically covers the basics of Python programming through three problems: arranging letters alphabetically, replacing words with emoticons, and unpacking list elements. These serve as practice for handling strings, dictionaries, and lists, while also applying Python’s built-in functions in solving simple tasks.

1. ALPHABET SOUP PROBLEM

The Alphabet Soup Problem is designed to practice string manipulation. The task is to create a function that arranges the letters of a word in alphabetical order. The program defines a function called alphabet_soup(word), which accepts a word as input. Inside the function, the sorted() function is applied to break the word into characters and arrange them alphabetically. Since the result of sorted() is a list, the ''.join() method is then used to combine the characters back into a single string.

PROCEDURE : 

1. Define the function alphabet_soup(word).
   

` def alphabet_soup(word): #DEFINE DUNCTION `

2. Use sorted() to arrange the characters in alphabetical order.

3. Apply ''.join() to reassemble the characters into a string.

`return '' .join(sorted(word)) #SORT LETTERS`

5. Accept user input using input().

`word = input("Type a word: ") #USER INPUT `

7. Pass the input word to the function and print the result.

`print(alphabet_soup(word))`

OUTPUT :

For example, when the user types SirNikkoLobos, the program outputs the same letters in alphabetical order. This shows how simple built-in functions can make text manipulation efficient and very straightforward in Python.

2. EMOTICON PROBLEM

The Emoticon Problem demonstrates the use of dictionaries and string replacement. A dictionary named emoticons is created, where each keyword such as "smile", "grin", "sad", and "mad" is mapped to its corresponding emoticon. A function called emote(sentence) is then defined to take a sentence as input. The program loops through the dictionary and uses the .replace() method to substitute every occurrence of the keywords with their emoticon equivalents.

PROCEDURE :

1. Create a dictionary mapping words to emoticons.
2. Define the function emote(sentence) to process the text.
3. Use a for-loop to check each word in the dictionary.

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

5. Replace the words in the sentence with their corresponding emoticons using .replace().
6. Return and print the modified sentence.

```
sentence = sentence.replace(word, emo) # REPLACE EVERY OCCURENCE OF 'WORD' WITH ITS EMOTICON
    return sentence
print(emote("Make me smile!"))
print(emote("I am mad."))
print(emote("She gave me a grin."))
print(emote("Engineering makes me sad."))

```

OUTPUT : 

<img width="273" height="43" alt="Screenshot 2025-08-27 215035" src="https://github.com/user-attachments/assets/7bc6590b-2d3b-40af-b207-c179a8e44528" />


For instance, the input sentence “Make me smile!” becomes “Make me :)!” while “I am mad.” becomes “I am >:(.” Similarly, “She gave me a grin.” is transformed into “She gave me a :D.” and “Engineering makes me sad.” becomes “Engineering makes me :((.” This demonstrates how Python dictionaries can act as lookup tables and how text can be modified dynamically using string methods.

3. UNPACKING LIST PROBLEM

The Unpacking List Problem focuses on separating the first, middle, and last elements of a list. A predefined list is given as [1, 2, 3, 4, 5, 6]. The goal is to assign the first element to first, the last element to last, and the remaining elements in between to middle. This is accomplished using list methods. The .pop(0) method removes and returns the first element, which is then stored in the variable first. The .pop(-1) method removes and returns the last element, which is stored in the variable last. The elements left in the list represent the middle section, which is stored in the variable middle.

PROCEDURE : 

1. Define a list with values [1, 2, 3, 4, 5, 6].

`lst = [1, 2, 3, 4, 5, 6] #CREATE LIST`

3. Use .pop(0) to extract the first element.

`first = lst.pop(0)   #REMOVE AND RETURN FIRST ELEMENT`

5. Use .pop(-1) to extract the last element.

`last = lst.pop(-1)   #REMOVE AND RETURN LAST ELEMENT`

7. Assign the remaining values to middle.

`middle = lst         #REMAINING LIST`

9. Print the three variables to display the results.
    
```
print("first:", first)
print("middle:", middle)
print("last:", last)
```

OUTPUT :

first: 1  
middle: [2, 3, 4, 5]  
last: 6  

