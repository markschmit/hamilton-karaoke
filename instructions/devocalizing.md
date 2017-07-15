# Devocalizing the Songs

To have the best karaoke experience one needs tracks without lyrics.  There are a couple approaches one can take.

## The simplest approach: use the Hamilton Instrumentals!

It's now possible to download the official Hamilton Instrumentals.  You can buy them in MP3 form [directly from Amazon](https://smile.amazon.com/Hamilton-Instrumentals-Original-Broadway-Cast/dp/B073GMNBSB).

## An alternative: de-vocalizing with Audacity

Broadway shows generally involve a lot more singing than just the main voices.  Unfortunately the instrumentals strip *all* of the voices.  There is software that can support removing most of the main vocals while still leaving non-major vocals (e.g. the ensemble bits) intact.  

### Using Audacity

Use [Audacity]()'s built-in [vocal-remover plugin](http://manual.audacityteam.org/man/vocal_remover.html).  This works by removing any audio that's identical on both stereo channels.  This *usually* eliminates most of the vocals, though some songs with many parts have non-centered parts that aren't eliminated at all.  (E.g. in Alexander Hamilton both Washington's and Eliza's parts are unaffected.)

This approach also has the downside of removing all other centered parts.  Often this includes drums and bass, but sometimes it can include even more.  Yorktown is particularly bad - it loses almost all of its record-scratching/etc.

### Bulk Application

Audacity allows one to apply the same 'chain' of effects to a whole directory at once.

Here's how to bulk remove-vocals:
1. Put all of your audio files in one directory, e.g. 'hamilton-karaoke/wav'
1. Open up Audacity
1. Create the chain:
  1. Go to 'File', 'Edit Chains'.
  1. Click 'Add'.  Name it 'RemoveVocalsAndSaveWav' and click OK.
  1. Click "Insert" and select VocalRemover.  Adjust params if desired.  Click OK.
  1. Click "Insert" and select ExportWAV.  Click OK.
  1. Click OK on the Edit Chains box.
1. Apply the chain to the directory
  1. Go to 'File', 'Apply Chain'.
  1. Click 'Apply to Files...'
  1. Browse to the original 'wav' directory and select files to devocalize.  Click 'Open'.
  1. The devocalized versions should be produced to a 'stripped' subdirectory of the original directory.

### Other approaches

There are probably more sophisticated approaches.  Contributions in this area are extremely welcome!
