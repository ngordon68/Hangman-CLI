# Hangman CLI

# 01 OverView
An CLI application of the classic game Hangman. Hangman is a game where the player is given a random word and the player has to guess the word within a limited number of attempts. 

# 02 Objectives 
 Dive into the essentials of Swift programming by creating a classic Hangman game that runs directly in the command line. This project is a hands-on way to solidify my understanding of Swift's core concepts while having fun with an interactive coding challenge

# 03 Skills
Loops, Arrays, Functions, Optionals, Structs, Enums, User Experience, User testing

# 04 UML Diagram

![Group](https://github.com/user-attachments/assets/c259659c-5505-42d1-b930-08e84665dace)

   
# 05 Technical Walkthrough   
The Hangman CLI was a great refresher to practiced my Swift fundamentals. I loved the game as a child and it was a perfect opportunity to recreate the game in the command line interface. One of my obstacles was that I was running to an issue with the user guessing correctly with a letter and having that letter geenerate in the correct space for the word. I intially tried to loop through the characters within the string but I was having issues with this approach. My solution was to take the user input and convert that into an array where each letter has it own index. If the user guessed a letter correctly, there will be a loop to check where the word has the guessed input and take the index to placed correctly. 

Here below is the code used to help placed the letter by the index position
```
fileprivate func placeLetter(_ userInput: String) {
    print("You have guessed \(userInput) which is correct!")
    for index in currentWordInArray.indices {
        if currentWordInArray[index] == userInput {
            guessedWordArray[index] = userInput
            guessedWord = guessedWordArray.joined()
            
        }
    }
}
```
    
    
# 06 Video Demo
Below is a video walkthrough Hangman in the command line interface

https://github.com/user-attachments/assets/1d0c2443-b01b-41f7-ae56-d5ad53ccb0f4






