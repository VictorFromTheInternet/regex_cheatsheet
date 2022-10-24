# Table of contents
* [Resources](#resources--tutorials)
* [Examples & Most Common](#examples-and-most-common)
   * [Phone Number matching](#phone-number-matching)
* [Meta Characters](#meta-characters)
   * [Resources](#single-characters)
   * [Quantifiers](#quantifiers)
   * [Position](#position)
   * [Character Classes](#character-classes)
   * [Groups](#groups)

<br>
<br>

# Resources & tutorials:
* [The coding train - programming w text](https://youtube.com/playlist?list=PLRqwX-V7Uu6YEypLuls7iidwHMdCM6o2w)
* [Regex 101 - Testing environment](https://regex101.com/)

<br>
<br>

# Examples and Most Common
#### Phone Number Matching
> \\(?\d{3}[-.)]\s?\d{3}[-.]\d{4}
> > \\(? ... literal '(' optionally <br>
> > \d{3} ... 3 digits <br>
> > [-.) ] ... either a - . ) <br>
> > \s? ... blank space optionally
> > \d{3} ... 3 digits <br>
> > [-. ] ... either a - .  <br>
> > \d{4} ... 4 digits <br>
> > > (###) ###-#### <br>
> > > (###)###-#### <br>
> > > ###-###-### <br>
> > > ###.###.#### <br>

#### Email Matching
> regex here

#### Password validation
> regex here

<br>
<br>
<br>

## Meta characters:
### Single characters
character |  definition
:----------:|:-------------:
   \w   |  any letter (letters and numbers) 
   \d   |  any digit
   \s   | any whitespace
   .    |  any character
   \    | escape sequence (to match special char literally)
 
 Notes:
 - the '\' character is also used for escape sequences 
   - (lets you type special characters in the rule) 
   - Ex: \w\w\w\w\*  ... matches ... text*
   - Ex: \.\w\w\w  ... mactches ... '.com' '.org' '.net'
 
<br>
<br>
<br>
 
### Quantifiers
character |  definition  
:----------:|:-------------:
   \*    |  0 or more times 
   \+    |  1 or more
   \?    |  0 or 1 time (Optional)
 {min, max}    |  min times, max times
  { n }  |  n amount of times

Notes:
- Quantifiers are applied to preceding characters/expressions. 
   - Ex: \w{4}  ... matches ... 'word'
   - Ex: colou?rs?  ... matches ... 'color' 'colour' and 'colours
 
<br>
<br>
<br>
 
### Position
character |  definition  
:----------:|:-------------:
   ^    |  beginning
   $     |  end
   \b    |  word boundary

Notes:
- \b\w{4,6}\b ... matches ... 'word' 'words' 'worlds'

<br>
<br>
<br>

### Character Classes
character |  definition  
:----------:|:-------------:
   [ ... ]  | matches a character within the specified class
   [ A-Z ]  | all uppercase letters
   [ a-z ]  | all lowercase letters
   
   
Notes:
   - Ex: user [abc] ... matches ... 'user a' 'user b' 'user c'
   - Ex: 

<br>
<br>
<br>

### Groups
character |  definition  
:----------:|:-------------:

