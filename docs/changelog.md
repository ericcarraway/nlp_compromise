Uses semvar, with occasional releases to npm and bower.

here, 'Major' is considered an api change, while 'Minor' is considered a performance change.

### v.3  &nbsp;  **(Breaking)**
* 3.0.2 - Statement & Question classes
* v3.0.0 - Feb 2016
  * split ngram, locale, and syllables into plugins in seperate repo

### v.2
* v2.0.0 - Nov 2015 &nbsp;  **(Breaking)**
  * es6 classes, babel building
  * better test coverage
  * ngram uses term tokenization, so that 'Tony Hawk' us one term, and not two
  * more organized pos rules
  * Pos tagging is done implicitly now once nlp.Text is run
  * Entity spotting is split into .people(), .place(), .organisations()
  * unicode normalisation is killed
  * opaque two-letter tags are gone
  * plugin support
  * passive tense detection
  * lexicon can be augmented third-party
  * date parsing results are different

### v.1
* v1.1.0 - May 2015
smarter handling of ambiguous contractions ("he's" -> ["he is", "he has"])

* v1.0.0 - May 2015
added name genders and beginning of co-reference resolution ('Tony' -> 'he') API.
small breaking change on ```Noun.is_plural``` and ```Noun.is_entity```, affording significant pos() speedup. Bumped Major version for these changes.

### v.0

* v0.5.2 - May 2015
Phrasal verbs ('step up'), firstnames and .people()

* v0.4.0 - May 2015
Major file-size reduction through refactoring

* v0.3.0 - Jan 2015
New NER choosing algorithm, better capitalisation logic, consolidated tests

* v0.2.0 - Nov 2014
Sentence class methods, client-side demos