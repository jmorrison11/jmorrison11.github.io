<!-- layout: page
title: "melodymaker"
permalink: /melodymaker/ -->

# Melody Maker
I used the IDE Netbeans to create this project. There is nothing visually unique about it like most of my other projects but it does play music. Refer to repository below.
I'm going to describe below the methods and what they do. There are a couple that need some sork still but the majority of it works just as it should and shows an
understanding of stacks and queues. 

- public Melody(Queue<Note> song)
    -Initializes your melody to store the passed in Queue of Notes. 
  
- public double getTotalDuration()
  - Returns the total length of the song in seconds. If the song includes a repeated section the length should include that repeated section twice. 
  
- public String toString()
  - This one doesn't return the information formatted at all. I only have it printing out the inital queue. 
  - Returns a String containing information about each note. Each note should be on its own line and output using its toString method. 
  
- public void changeTempo(double tempo)
  - Changes the tempo of each note to be tempo percent of what it formerly was. Passing a tempo of 1.0 will make the tempo stay the same.  
  tempo of 2.0 will make each note twice as long. tempo of 0.5 will make each note half as long. 
  
- public void reverse()
  - I do not have this method working properly as of now. 
  - Reverses the order of notes in the song, so that future calls to the play methods will play the notes in the opposite of the order they were 
  in before reverse was called.  For example, a song containing notes A, F, G, then B would become B, G, F, A.
  
- public void append(Melody other)
  - I do not have this method working properly as of now. 
  - Adds all notes from the given other song to the end of this song. 
  For example, if this song is A,F,G,B and the other song is F, C, D, the method should change this song to be A, F, G, B, F, C, D. 
  The other song should be unchanged after the call.
  
- public void play()
  - Play the song by calling each note's play method. 
  The notes should be played from the beginning of the queue to the end unless there are notes that are marked as being the beginning or end of a repeated section. 
  When the first note that is a beginning or end of a repeated section is found it creates a second queue. 
  It gets notes from the original queue until it sees another marked as being the beginning or end of a repeat. 
  As it gets these notes it will play them and then place them back in both queues. 
  Once you hit a second mark at the beginning or end of a repeat it should play everything in the secondary queue and then return to playing from the main queue. 
  It should be possible to call this method multiple times and get the same result.

##### [the repository](https://github.com/jmorrison11/MelodyMaker) 
###### [back to home](jmorrison11.github.io)
###### [back to project list](https://jmorrison11.github.io/projects)
