# Lyric Makers by creating PowerPoint Slides

The purpose of these scripts is to reduce the amount of time spent copy pasting 
lyrics into slides that can later be used as translation guides or for lyrics 
videos (what I used it for). Where the lyrics will be printed for the slide is
dependent on the script you use. The main one, lyric_maker, has it in the bottom
third so that you can add an image on the top to indicate who is singing or some
art or whatever.

Here is an example of what would be created
![Image of lyric example](https://i.ytimg.com/vi/o0ftlJfcVxU/maxresdefault.jpg)


## USAGE

python lyric_maker.py <firstlyric.txt> <secondlyric.txt> <thirdlyric.txt>

Yes you have to write python if you don't have the correct initialization, download
whatever python is updated, just not 2.7. google it.

This script was designed to be used with "hangul" or korean lyrics as the first
text, romanization as the second text file, and english translations as the third
text file. These three txt files MUST be the same length and even blank lines are
counted. Each line corresponds to the same lyric. 

You can drag and drop the file into your terminal or run time rather than having to 
change directories. Note that the OUTPUT file will be exported based on what is 
written inside the script. To change the output to a specific folder, go into the script
and edit line 60, where you put the correct output folder.

Example: prs.save('/Users/loser/Downloads/done_slides.pptx')

Feel free to add an output folder function if you so desire, I would do it but I'm too
lazy to have to add another argument...

##Types of lyric makers

There are a large variety that have a certain number of files or argument necessary.
 
lyric_maker: has three inputs for (hangul/korean, romanization, and translation)
these are centered in the bottom third. 
lyric_maker_aesthetic: has three inputs, centered in the middle. 
lyric_maker_english: has two inputs (english lyric on top, translation on the bottom),
centered for lower third
lyric_maker_japan: has four inputs (japanese lyric, romanization, eng trans, kor trans):
centered for lower third
lyric_maker_sadballad: had three inputs (kor, rom, trans) but it is centered where the
last file (in this case the english trans) is on top for peak aesthetic. the words are
WHITE but you can change that in the script (lines with RGB color, look up the color you
want and replace the three values) 
lyric_maker_solo: three inputs but right aligned, this was used to add the image of
the singer or whatever on the left side of the slide. 
lyric_maker_solo_english: two inputs, right aligned format
lyric_maker_solo_only_eng: just one input, right aligned format
