# GhostWordGame

Here is a fully functional android app which I made in Google Applied CS with android program. 
Ghost is a word game in which players take turns adding individual letters to a growing word fragment, trying not to be the one to complete a valid word. 
Each fragment must be the beginning of an actual word, and, for our purposes, we will consider 4 to be the minimum word length. 
The player who completes a word or creates a fragment that is not the prefix of a word loses the round.

#Rules of Game

So on player 1's turn, they can:

challenge player 2's word if they think player 2 has formed a valid word of at least 4 letters.
If the fragment is a word, then player 1 wins; if the fragment is not a word, then player 2 wins.
challenge player 2's word if they think that no word can be formed with the current fragment. 
Then, player 2 must provide a valid word starting with the current fragment or lose.
add a letter to move the fragment towards a valid word. 
attempt to bluff player 2 by adding a letter that doesn't move the fragment towards a valid word.

#Screens

![Alt text](https://lh4.googleusercontent.com/-WaELE3qq66ZwPSX5Jo-tU6GoMfNSdhXBQxw-YjVV9c0Y4Q0xq4GhZllyCh2_kY8CosE54XE=w1366-h638 "Optional title2")

#Modes
Mode 1 - Uses SimpleDictionary Class <br />
Mode 2 - Uses FastDictionary Class [Improved version of game which uses trie data structure to store our dictionary] </br >
Just to test both modes of game, change "GhostDictionary dictionary = new FastDictionary(inputStream);" OR "GhostDictionary dictionary = new SimpleDictionary(inputStream);" in onCreate() method of GhostActivity.java <br />
GhostDictionary is an interface, not a class. This is the shared interface for SimpleDictionary and FastDictionary. This shared interface makes it easy to swap between the two kinds of dictionaries in the activity.

#Data Structures 

Binary search <br />
ArrayList <br />
Trie 

#License

Copyright 2016 Akshay Jain

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
