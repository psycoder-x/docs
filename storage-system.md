
# Storage System

Psycoder-x Storage System (PXSS) is a method that defines how
to name and sort files and directories on your hard drive, cloud
storage, flash drive, etc. The purpose of PXSS is to provide a
way to organize things on the same or different storages.

No matter what storage you use. If there is a way to manage files
and directories, you can use this storage system.

## Storage tree

In general, the root directory is divided into six pillars,
with some pillars containing main filters.

The following table shows the storage structure:

| Pillars: | prj | psp | srt | tmp | use | was |
|-|-|-|-|-|-|-|
| Main filters: | lib pic run snd txt vid | | | | lib pic run snd txt vid | lib pic run snd txt vid |

## Filter

Filter is a directory that defines what can be stored in it.
Predefined filter is a filter defined in this document.
Main filter is a predefined filter that is stored directly in the pillar.
Such main filters exists: lib, pic, run, snd, txt, vid. 

### run

The filter that contains programs, games, and any other runnable things.
Specifically, executables, scripts, examples, documentation,
and files that cannot be separated from its executable. 

### lib

The filter that contains static libraries, dynamic libraries,
include files, documentation, and examples.

### pic

The filter that contains static graphics: pictures, photos,
images, art, textures, diagrams, etc.

### snd

The filter that contains anything to listen to (sounds, music, noises, etc).
This filter may contain graphics such as album art or similar.

### txt

The filter that contains files for humans to read: documents,
tables, text, presentations, documentation, books, etc.
May contain graphical elements but as long as the text remains the main part.

### vid

The filter that contains videos, movies, animations, etc.
With or without a sound channel.

## Pillar

Pillar is a directory defined in this document
that defines what you can or should do with its contents.
Such pillars exists: prj, psp, srt, tmp, use, was.

### tmp

The pillar for temporary files that you delete after use.
For example, to test something, you create a temporary project and delete it when you're done.
This pillar has no filters because you don't need to sort the things to be deleted.

### srt

The pillar for files that you intend to sort later.
If you do not have time to determine where to save the file, this pillar is for you.
This pillar has no filters because it exists to avoid filters.

### was

The pillar for things you no longer intend to use or change.
Don't call it "read only" rather "story storage".
This is the best place for storing public files.
This pillar contains the main filters.
Any subdirectory except the main filters can be saved as an archive file (most likely zip).

### use

The pillar for things that can be used every day.
This pillar contains the main filters.   

### prj

The pillar for your projects, things you're working on.
This pillar contains the main filters, but they don't work as expected.
In this pillar you filter things not by project files, but by files that are the result of projects.
For example, the code is a text, but it falls under the "run" filter
because the result of compiling that code is an executable file.
A project may contain any number of subprojects.
Sometimes it's just a sub-project (mod, asset, documentation, etc.) without any parent project files,
in which case the parent project directory needs to be created just to contain those sub-projects.

### psp

The pillar for some platform-specific directories and files.
In many cases these things cannot be moved, but if you want to and can do so, move them to this pillar.

## Directory and file names

In this chapter implied directories and files you can rename without losing your posabilities.

Avoid uppercase (capital letters). Take care of your Shift and Caps Lock keys.

Avoid spaces. This allows you to write the path without double quotes.
Use minus instead. Or use underscore if minus is not allowed.

Avoid plurals in directory names, as any directory always contains multiple items.
There is no reason to keep the plural form.
However, in file names, the plural form makes sense,
but in many cases, may be replaced with "list", "set", "array", etc.
And it is much easier to search for files whose name contains the word "list"
instead of the letter "s" (or some unpredictable English plural form yet).

Use short forms in names if the meaning can be understood from the context
or if the full form is described elsewhere (for example, in this document).
Avoid uncommon acronyms.

## Version Control System

Directories and files used in any version control system should be ignored,
as these things can be anywhere and cannot be moved.

## Relation Problem

Sometimes it is not possible to separate two or more definitely different things
because these things are related to each other.
As a result, they cannot be placed in any filter.
To solve this problem you need to:
 1. Create a directory for all related things.
 2. Move all related things into the created directory.
 3. Find the main file among the related files. It describes relations or is directly related to all other files.
 4. Put the resulting directory in the filter according to the main file.

## Definition Problem

Sometimes it is not possible to separate two or more things 
because it is difficult to define their differences.
If this happens, things should not be separated.

## Sub-directories

The contents of any directory can be separated between sub-directories
as long as these subdirectories avoid the definition problem.
