Sanscript.js
=============================

## Introduction

Sanscript is a transliteration library for Indian languages. It supports the most popular Indian scripts and several different romanization schemes. Although Sanscript focuses on Sanskrit transliteration, it has partial support for other languages and is easy to extend.

## Setup
The package is officially distributed at npm [here](https://www.npmjs.com/package/@sanskrit-coders/sanscript), whereas a variant due to Vikram Iyer is separately available [here](https://www.npmjs.com/package/sanscript). So one can use commands such as:

- `npm install @sanskrit-coders/sanscript`
- `yarn add @sanskrit-coders/sanscript`

## Usage

Sanscript is simple to use:

```js
var output = Sanscript.t(input, from, to);
```

Here, `from` and `to` are the names of different **schemes**. In Sanscript, the word "scheme" refers to both scripts and romanizations. These schemes are of two types:

1. **Brahmic** schemes, which are *abugidas*. All Indian scripts are Brahmic schemes.
2. **Roman** schemes, which are *alphabets*. All romanizations are Roman schemes.

By default, Sanscript supports the following Brahmic schemes:

ahom, assamese, avestan, balinese, bengali, bhaisuki, brahmi, brahmi_tamil, burmese, chakma, cham, cyrillic, devanagari, dogra, gondi_gunjala, gondi_masaram, grantha, grantha_pandya, gujarati, gurmukhi, hk, iast, itrans, itrans_dravidian, javanese, kannada, khamti_shan, kharoshti, khmer, khom_thai, khudawadi, kolkata, lao, lao_pali, lepcha, limbu, mahajani, malayalam, manipuri, marchen, modi, mon, mro, multani, newa, ol_chiki, oriya, persian_old, phags_pa, ranjana, rejang, rohingya, sanskritOCR, shan, sharada, siddham, sinhala, slp1, sora_sompeng, sundanese, syloti_nagari, tagalog, tagbanwa, tai_laing, takri, tamil, tamil_extended, tamil_superscripted, telugu, thai, tibetan, tirhuta_maithili, urdu, vattelutu, velthuis, wancho, warang_citi, wx, zanbazar_square

of which the following are Roman schemes:

* `hk` (Harvard-Kyoto)
* `iast` (International Alphabet of Sanskrit Transliteration)
* `itrans` (ITRANS)
* `itrans_dravidian` (ITRANS with support for Dravidian short "e" and "o")
* `kolkata` (National Library at Kolkata)
* `slp1` (Sanskrit Library Phonetic Basic)
* `velthuis` (Velthuis)
* `wx` (WX)
* `cyrillic`

### IAST Simplified
I have included a simplified IAST scheme that can be used to edit Sanskrit documents using ASCII characters available on a standard keyboard. This fork of Sanscript.js is available from http://github.com/trivedigaurav/sanscript.js/.

<table>
  <tr>
   <td>Vowels
   </td>
   <td>

<table>
  <tr>
   <td rowspan="2" >अ
<p>
<strong>a</strong>
   </td>
   <td rowspan="2" >आ
<p>
<strong>-a</strong>
   </td>
   <td rowspan="2" >इ
<p>
<strong>i</strong>
   </td>
   <td rowspan="2" >ई 
<p>
<strong>-i</strong>
   </td>
   <td rowspan="2" >उ
<p>
<strong>u</strong>
   </td>
   <td rowspan="2" >ऊ 
<p>
<strong>-u</strong>
   </td>
   <td rowspan="2" >ऋ
<p>
<strong>r.</strong>
   </td>
   <td rowspan="2" >ॠ
<p>
<strong>-r.</strong>
   </td>
   <td rowspan="2" >ऌ
<p>
<strong>l.</strong>
   </td>
   <td rowspan="2" >ॡ
<p>
<strong>-l.</strong>
   </td>
   <td rowspan="2" >ए
<p>
<strong>e</strong>
   </td>
   <td rowspan="2" >ऐ
<p>
<strong>ai</strong>
   </td>
   <td rowspan="2" >ओ
<p>
<strong>o</strong>
   </td>
   <td rowspan="2" >औ
<p>
<strong>au</strong>
   </td>
   <td rowspan="2" >ं
<p>
<strong>m.</strong>
   </td>
   <td rowspan="2" >ः
<p>
<strong>h.</strong>
   </td>
  </tr>
  <tr>
  </tr>
</table>


   </td>
  </tr>
  <tr>
   <td>Consonants

   </td>
   <td>

<table>
  <tr>
   <td rowspan="2" >क
<p>
<strong>ka</strong>
   </td>
   <td rowspan="2" >ख
<p>
<strong>kha</strong>
   </td>
   <td rowspan="2" >ग
<p>
<strong>ga</strong>
   </td>
   <td rowspan="2" >घ
<p>
<strong>gha</strong>
   </td>
   <td rowspan="2" >ङ
<p>
<strong>.na</strong>
   </td>
  </tr>
  <tr>
  </tr>
  <tr>
   <td rowspan="2" >च
<p>
<strong>ca</strong>
   </td>
   <td rowspan="2" >छ
<p>
<strong>cha</strong>
   </td>
   <td rowspan="2" >ज
<p>
<strong>ja</strong>
   </td>
   <td rowspan="2" >झ
<p>
<strong>jha</strong>
   </td>
   <td rowspan="2" >ञ
<p>
<strong>~na</strong>
   </td>
  </tr>
  <tr>
  </tr>
  <tr>
   <td rowspan="2" >ट
<p>
<strong>t.a</strong>
   </td>
   <td rowspan="2" >ठ
<p>
<strong>t.ha</strong>
   </td>
   <td rowspan="2" >ड
<p>
<strong>d.a</strong>
   </td>
   <td rowspan="2" >ढ
<p>
<strong>d.ha </strong>
   </td>
   <td rowspan="2" >ण
<p>
<strong>n.a</strong>
   </td>
  </tr>
  <tr>
  </tr>
  <tr>
   <td rowspan="2" >त
<p>
<strong>ta </strong>
   </td>
   <td rowspan="2" >थ
<p>
<strong>tha</strong>
   </td>
   <td rowspan="2" >द
<p>
<strong>da</strong>
   </td>
   <td rowspan="2" >ध
<p>
<strong>dha</strong>
   </td>
   <td rowspan="2" >न
<p>
<strong>na</strong>
   </td>
  </tr>
  <tr>
  </tr>
  <tr>
   <td rowspan="2" >प
<p>
<strong>pa</strong>
   </td>
   <td rowspan="2" >फ
<p>
<strong>pha</strong>
   </td>
   <td rowspan="2" >ब
<p>
<strong>ba</strong>
   </td>
   <td rowspan="2" >भ
<p>
<strong>bha</strong>
   </td>
   <td rowspan="2" >म
<p>
<strong>ma</strong>
   </td>
  </tr>
  <tr>
  </tr>
  <tr>
   <td rowspan="2" >श
<p>
<strong>‘sa</strong>
   </td>
   <td rowspan="2" >ष
<p>
<strong>s.a</strong>
   </td>
   <td rowspan="2" >स
<p>
<strong>sa</strong>
   </td>
   <td rowspan="2" >ह
<p>
<strong>ha</strong>
   </td>
   <td rowspan="2" > ळ
<p>
<strong>~la</strong>
   </td>
  </tr>
  <tr>
  </tr>
  <tr>
   <td rowspan="2" >य
<p>
<strong>ya</strong>
   </td>
   <td rowspan="2" >र
<p>
<strong>ra</strong>
   </td>
   <td rowspan="2" >ल
<p>
<strong>la</strong>
   </td>
   <td rowspan="2" >व
<p>
<strong>va</strong>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>
   </td>
  </tr>
</table>


   </td>
  </tr>
  <tr>
   <td>Vowel Marks (examples)

   </td>
   <td>

<table>
  <tr>
   <td rowspan="2" >क्
<p>
<strong>k</strong>
   </td>
   <td rowspan="2" >खा
<p>
<strong>kh-a</strong>
   </td>
   <td rowspan="2" >गि
<p>
<strong>gi</strong>
   </td>
   <td rowspan="2" >घी
<p>
<strong>dh-i</strong>
   </td>
   <td rowspan="2" >ङु
<p>
<strong>.nu</strong>
   </td>
  </tr>
  <tr>
  </tr>
  <tr>
   <td rowspan="2" >चू
<p>
<strong>c-u</strong>
   </td>
   <td rowspan="2" >छृ
<p>
<strong>chr.</strong>
   </td>
   <td rowspan="2" >जॄ
<p>
<strong>j-r.</strong>
   </td>
   <td rowspan="2" >झॢ
<p>
<strong>jhl.</strong>
   </td>
   <td rowspan="2" >ञॣ
<p>
<strong>~n-l.</strong>
   </td>
  </tr>
  <tr>
  </tr>
  <tr>
   <td rowspan="2" >टे
<p>
<strong>t.e</strong>
   </td>
   <td rowspan="2" >ठै
<p>
<strong>t.hai</strong>
   </td>
   <td rowspan="2" >डो
<p>
<strong>d.o</strong>
   </td>
   <td rowspan="2" >डौ
<p>
<strong>d.au</strong>
   </td>
   <td rowspan="2" >थ्
<p>
<strong>tha</strong>
   </td>
  </tr>
  <tr>
  </tr>
  <tr>
   <td rowspan="2" >णं
<p>
<strong>n.am</strong>
   </td>
   <td rowspan="2" >तः
<p>
<strong>tah.</strong>
   </td>
   <td rowspan="2" >क्ष
<p>
<strong>ks.a</strong>
   </td>
   <td rowspan="2" >त्र
<p>
<strong>tra</strong>
   </td>
   <td rowspan="2" >ज्ञ
<p>
<strong>j~na</strong>
   </td>
  </tr>
  <tr>
  </tr>
</table>


   </td>
  </tr>
  <tr>
   <td>Symbols

   </td>
   <td>

<table>
  <tr>
   <td rowspan="2" >ऽ
<p>
<strong>'</strong>
   </td>
   <td rowspan="2" >।
<p>
<strong>|</strong>
   </td>
   <td rowspan="2" >।।
<p>
<strong>||</strong>
   </td>
   <td rowspan="2" >०
<p>
<strong>0</strong>
   </td>
   <td rowspan="2" >१
<p>
<strong>1</strong>
   </td>
   <td rowspan="2" >२
<p>
<strong>2</strong>
   </td>
   <td rowspan="2" >३
<p>
<strong>3</strong>
   </td>
   <td rowspan="2" >४
<p>
<strong>4</strong>
   </td>
   <td rowspan="2" >५
<p>
<strong>5</strong>
   </td>
   <td rowspan="2" >६
<p>
<strong>6</strong>
   </td>
   <td rowspan="2" >७
<p>
<strong>7</strong>
   </td>
   <td rowspan="2" >८
<p>
<strong>8</strong>
   </td>
   <td rowspan="2" >९
<p>
<strong>9</strong>
   </td>
  </tr>
  <tr>
  </tr>
</table>


   </td>
  </tr>
</table>

### Example Phrases

*IAST Simplified:*    nar-ah. gacchanti |

*IAST:*               narāḥ gacchanti.

*ITRANS:*             narAH gachChanti.

*Devanagari:*         नराः गच्छन्ति ।

#### Vedic Accents

*IAST Simplified:*    a\_gnim-i\!~le pu\_rohi\!tam. ya\!j~nasya\! de\_vamr.\_tvija\!m

*IAST:*               a॒gnimī॑ḻe pu॒rohi॑taṃ ya॑jñasya॑ de॒vamṛ॒tvija॑m

*ITRANS:*             a\_gnimI\'Le pu\_rohi\'taM ya\'j~nasya\' de\_vamRRi\_tvija\'m

*Devanagari:*         अ॒ग्निमी॑ळे पु॒रोहि॑तं य॑ज्ञस्य॑ दे॒वमृ॒त्विज॑म्

### Disabling transliteration
When Sanscript sees the token `##`, it toggles the transliteration state:

```js
Sanscript.t('ga##Na##pa##te', 'hk', 'devanagari'); // गNaपte
Sanscript.t('ध##र्म##क्षेत्रे', 'devanagari', 'hk'); // dhaर्मkSetre
```

When Sanscript sees the token `\`, it disables transliteration on the character that immediately follows. `\` is used for ITRANS compatibility; we recommend always using `##` instead.

```js
Sanscript.t('a \\a', 'itrans', 'devanagari'); // अ a
Sanscript.t('\\##aham', 'itrans', 'devanagari'); // ##अहम्
```

### Transliterating to lossy schemes
A **lossy** scheme does not have the letters needed to support lossless translation. For example, Bengali is a lossy scheme because it uses `ব` for both `ba` and `va`. In future releases, Sanscript might let you choose how to handle lossiness. For the time being, it makes some fairly bad hard-coded assumptions. Corrections and advice are always welcome.

### Transliteration options
You can tweak the transliteration function by passing an `options` object:

```html
<script src="node_modules/@sanskrit-coders/sanscript/sanscript.js"></script>
<script>
  var output = Sanscript.t(input, from, to, options);
</script>
```

`options` maps options to values. Currently, these options are supported:

* `skip_sgml` - If true, transliterate SGML tags as if they were ordinary words (`<b>iti</b>` → `<ब्>इति</ब्>`). Defaults to `false`.
* `syncope` - If true, use Hindi-style transliteration (`ajay` → `अजय`). In linguistics, this behavior is known as [schwa syncope](http://en.wikipedia.org/wiki/Schwa_deletion_in_Indo-Aryan_languages). Defaults to `false`.

## Contributing

### Installing dependencies

Run either:

- `npm install`
- `yarn`

### Adding new schemes

Adding a new scheme is simple:

```js
Sanscript.addBrahmicScheme(schemeName, schemeData);
Sanscript.addRomanScheme(schemeName, schemeData);
```

For help in creating `schemeData`, see the comments on the `addBrahmicScheme` and `addRomanScheme` functions.

### Testing

We use `qunit` for testing.
After installing dependencies, you can either:

* run `npm run test` to run tests from the command line
* open [test/index.html](test/index.html) to run tests in the browser

### Publishing to npm

```shell
npm publish --access public
```
