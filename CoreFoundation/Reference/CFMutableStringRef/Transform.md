```
Boolean CFStringTransform ( CFMutableStringRef string, CFRange *range, CFStringRef transform, Boolean reverse );
```

The transformation represented by transform is applied to the given range of string, modifying it in place. Only the specified range is modified, but the transform may look at portions of the string outside that range for context. Reasons that the transform may be unsuccessful include an invalid transform identifier, and attempting to reverse an irreversible transform.



kCFStringTransformStripCombiningMarks
The identifier of a transform to strip combining marks (accents or diacritics).

kCFStringTransformToLatin
The identifier of a transform to transliterate all text possible to Latin script. Ideographs are transliterated as Mandarin Chinese.


kCFStringTransformFullwidthHalfwidth
The identifier of a reversible transform to convert full-width characters to their half-width equivalents.


kCFStringTransformLatinKatakana
The identifier of a reversible transform to transliterate text to Katakana from Latin.


kCFStringTransformLatinHiragana
The identifier of a reversible transform to transliterate text to Hiragana from Latin.


kCFStringTransformHiraganaKatakana
The identifier of a reversible transform to transliterate text to Katakana from Hiragana.


kCFStringTransformMandarinLatin
The identifier of a transform to transliterate text to Latin from ideographs interpreted as Mandarin Chinese. This transform is not reversible.


kCFStringTransformLatinHangul
The identifier of a reversible transform to transliterate text to Hangul from Latin.


kCFStringTransformLatinArabic
The identifier of a reversible transform to transliterate text to Arabic from Latin.


kCFStringTransformLatinHebrew
The identifier of a reversible transform to transliterate text to Hebrew from Latin.


kCFStringTransformLatinThai
The identifier of a reversible transform to transliterate text to Thai from Latin.


kCFStringTransformLatinCyrillic
The identifier of a reversible transform to transliterate text to Cyrillic from Latin.


kCFStringTransformLatinGreek
The identifier of a reversible transform to transliterate text to Greek from Latin.


kCFStringTransformToXMLHex
The identifier of a reversible transform to transliterate characters other than printable ASCII to XML/HTML numeric entities.


kCFStringTransformToUnicodeName
The identifier of a reversible transform to transliterate characters other than printable ASCII (minus braces) to their Unicode character name in braces.

Examples include {AIRPLANE} and {GREEK CAPITAL LETTER PSI}.


kCFStringTransformStripDiacritics
The identifier of a transform to remove diacritic markings.
