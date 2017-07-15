# How to lay out lyrics

1. Create a lyrics/ subdirectory in the given song directory.
2. Copy lyrics from appropriate Genius.com page into a 'genius.txt' file
3. Do page layout: open the lyrics in KBS and start dividing into pages.  Save as 'paginated.txt'.
  - Put parallel verses on the same pages. 
  - Don't include chorus lines that simply back up a primary singer. 
  - Include only chrous lines that are at least partially broadly sung (e.g. you'd sing it when singing the song in the shower)
  - Don't include character cues after the first unless the color alone will be insufficient (e.g. distinguishing COMPANY from MALE ENSEMBLE while reusing color or an occasional joint-cue).  This requires thinking about how many colors will be necessary for the song.

4. Syllabalize the text, putting slashes between syllables in words:
  - http://juiciobrennan.com/syllables/ might be helpful, but you need to replace hyphens with slashes, remove slashes from character cues, and fix the words that aren't found (e.g. contracted forms like "drippin'").  Save as 'syllables.txt'.

5. Create a 'sync' version that has no parallel vocals and no character cues but maintains the page separations.  This is the version that we'll use to do the initial syncing, after which we'll restore the other lyrics.  Save as 'sync.txt'.


## Tips

- You want to be able to have lines disappear one-by-one so the next set of lines can start appearing.  The lyrics are often too fast to clear an entire screen at once.

## Example: The Schuyler Sisters

### [genius.txt](../05-TheSchuylerSisters/lyrics/genius.txt)

This is copied pretty directly from [the genius.com page](https://genius.com/Lin-manuel-miranda-the-schuyler-sisters-lyrics).
<pre>
[ANGELICA AND MALE ENSEMBLE]
Look around, look around-

[ELIZA]
Angelica, remind me what we’re looking for…

[ALL MEN]
She’s lookin’ for me!

[ANGELICA]
Eliza, I’m lookin’ for a mind at work
I’m lookin’ for a mind at work!
I’m lookin’ for a mind at work!
Whooaaaaa!

[ELIZA/ANGELICA/PEGGY]
Whooaaaaa!
Work!	[COMPANY]
Work, work!

Work, work!
Work, work!




Work!
</pre>

### [paginated.txt](../05-TheSchuylerSisters/lyrics/paginated.txt)

Now we're relying on color to carry a lot of information.  Note how principal + ensemble lines are split into separate parallel lines (of different colors) and most cues are removed (because at this point in the song we'll use colors as cues).
<pre>
Look around, look around-
[ALL MEN]
Look around, look around-
Angelica, remind me what
we’re looking for-
She’s lookin’ for me!

Eliza, I’m lookin’ for a mind at work,
Work, work!
I’m lookin’ for a mind at work!
Work, work!
I’m lookin’ for a mind at work!
Work, work!

Whooaaaaa!
 [SS] Whooaaaaa!
 [SS] Work!
[CHORUS] Work!
</pre>

### [syllables.txt](../05-TheSchuylerSisters/lyrics/syllables.txt)
Pretty much identical, except with syllables split up.

<pre>
Look a/round, look a/round-
[ALL MEN]
Look a/round, look a/round-
An/gel/i/ca, re/mind me what
we’re look/ing for
She’s look/in’ for me!

E/li/za, I’m look/in’ for a mind at work,
Work, work!
I’m look/in’ for a mind at work!
Work, work!
I’m look/in’ for a mind at work!
Work, work!

Whooaaaaa!
Whooaaaaa!
Work!
Work!
</pre>

### [sync.txt](../05-TheSchuylerSisters/lyrics/sync.txt)
Same as above with parallel lyrics ("Look around, look around") and character cues ("[ALL MEN]") stripped out.
<pre>
Look a/round, look a/round-
An/gel/i/ca, re/mind me what
we’re look/ing for
She’s look/in’ for me!

E/li/za, I’m look/in’ for a mind at
Work, work!
I’m look/in’ for a mind at
Work, work!
I’m look/in’ for a mind at
Work, work!

Whooaaaaa!
Whooaaaaa!
Work!
</pre>
