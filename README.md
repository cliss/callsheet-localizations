# callsheet-localizations
Localization Files for [Callsheet](https://apps.apple.com/us/app/callsheet-find-cast-crew/id1672356376).

There are two sections:

* [`CallsheetLocalizations`](https://github.com/cliss/callsheet-localizations/tree/main/CallsheetLocalizations), which has all the text used inside the app.
* [`AppStore`](https://github.com/cliss/callsheet-localizations/tree/main/AppStore), which has the description and promotional text used [in the App Store](https://apps.apple.com/us/app/callsheet-find-cast-crew/id1672356376)

## Current Status

As of [77578a6](https://github.com/cliss/callsheet-localizations/commit/77578a6a04166c771e598b8f642974c68c93ebfa):

| Language        | % Complete  | [App Store][as] | Authors                           |
| :-------------- | :---------- | :-------------- | :-------------------------------- |
| English ([Modern](https://en.wikipedia.org/wiki/United_States)) | N/A         | ✔️              | [cliss](https://github.com/cliss) |
| English ([Traditional](https://en.wikipedia.org/wiki/United_Kingdom)) | N/A         | ✔️              | [cliss](https://github.com/cliss) |
| English ([Simplified](https://en.wikipedia.org/wiki/Australia)) | N/A         | ✔️              | [cliss](https://github.com/cliss) |
| Dutch           | 100% :tada: | ✔️              | [Deddiekoel](https://github.com/deddiekoel), [icod](https://github.com/icod) |
| French (🇫🇷)     | 100% :tada: |                 | [EricEEEEE](https://github.com/EricEEEEE), [samthegeek](https://github.com/samthegeek), [DonSqueak](https://github.com/donsqueak), [sayrer](https://github.com/sayrer) |
| French (🇨🇦)     | 100% :tada: |                 | [EricEEEEE](https://github.com/EricEEEEE), [samthegeek](https://github.com/samthegeek), [DonSqueak](https://github.com/donsqueak) |
| German          | 100% :tada: | ✔️              | [DonSqueak](https://github.com/donsqueak), [technocidal](https://github.com/technocidal), [fweber-de](https://github.com/fweber-de) |
| Hebrew          | 100% :tada: | ✔️              | [orisraeli](https://github.com/orisraeli) |
| Italian         | 100% :tada: | ✔️              | [cdf1982](https://github.com/cdf1982) |
| Norwegian (Bokmål) | 100% :tada: | ✔️              | [lognseth](https://github.com/lognseth) |
| Portuguese (🇵🇹) | 100% :tada: | ✔️              | [apfernandes](https://github.com/apfernandes), [sayrer](https://github.com/sayrer) |
| Russian         | 100% :tada: | ✔️              | [gkeep](https://github.com/gkeep), ChatGPT-4.o |
| Spanish (🇲🇽)    | 100% :tada: |                 | [ccavazos](https://github.com/ccavazos), [sayrer](https://github.com/sayrer) |
| Spanish (🇪🇸)    | 100% :tada: | ✔️              | [unaiherran](https://github.com/unaiherran) |
| Spanish (🌎)    | 100% :tada: |           | [ccavazos](https://github.com/ccavazos) |
| Swedish         | 100% :tada: | ✔️              | [sebdanielsson](https://github.com/sebdanielsson) |
| Ukrainian       | 100% :tada: | ✔️              | [zemlanin](https://github.com/zemlanin), [buzbohdan](https://github.com/buzbohdan) |
| Polish          | 100% :tada: |                 | [spitfire](https://github.com/spitfire), [DonSqueak](https://github.com/donsqueak) |
| Portuguese (🇧🇷) | 73%         |                 | [insidegui](https://github.com/insidegui) |
| Japanese        | 58%         |                 | [kenroy](https://github.com/kenroy), [jaddkeita](https://github.com/jaddkeita) |
| Korean          | 46%         |                 | [EdogawaKun](https://github.com/EdogawaKun)
| Danish          | 5%          |                 | [hanse00](https://github.com/hanse00) |

[as]: https://github.com/cliss/callsheet-localizations/tree/main/AppStore

## Basics

This repository contains a series of [string catalog](https://developer.apple.com/documentation/xcode/localizing-and-varying-text-with-a-string-catalog) files. They contain a series of translatable snippets, and, eventually, their translations.

I am not concerned with word-for-word, direct translations. **I'd vastly prefer translations that capture the _spirit_ and _tone_ of what's being said &mdash; and Callsheet in general &mdash; even if that means rephrasing what I've written, using locally-appropriate idioms, etc.** Please have fun with this, and make choices that are appropriate for the audience that speaks your language.

The easiest way to open and modify these files &mdash; other than using [Xcode](https://developer.apple.com/xcode/) &mdash; is to use the free macOS app [Loca Studio](https://www.cunningo.com/locastudio/index.html).

Be careful with Loca Studio though! Save your work often!

## Using Loca Studio

Generally speaking, you can look at the `ID` column, and provide a translation in the `Target` column. However, there are some special cases:

### Plurality

For some items, like age, will occasionally have a singular and a plural form. Look at the ages shown here:

<img width="380" alt="Screenshot 2024-05-10 at 8 27 46 PM" src="https://github.com/cliss/callsheet-localizations/assets/282460/419dcd21-d3f4-44ec-8d47-87fffc36c3ef">

This isn't _super_ obvious in Loca Studio:

<img width="410" alt="Screenshot 2024-05-10 at 8 24 59 PM" src="https://github.com/cliss/callsheet-localizations/assets/282460/af01548a-6f2a-4b2d-aa5d-3139ba935370">

Note that the `Source` column kind of hints at what's going on here, but the `ID` column shows `plural.one` for the singular version and `plural.other` for the plural version. Fill each in as appropriate, please.

[Language Plural Rules](https://www.unicode.org/cldr/charts/45/supplemental/language_plural_rules.html)

Some languages have more complicated pluralization rules than English speakers are used to. Words can be pluralized in ways that English speakers would recognize from [ordinal numerals](https://en.wikipedia.org/wiki/Ordinal_numeral), like 20th, 21st, 22nd, 23rd. You can look these up in the rules table above.

As an example, these are the rules for Polish:

| Pluralization  | English    | Polish       | Numbers |
| :------------- | :--------- | :----------- | :------ |
| one            | 1 month    | 1 miesiąc    | 1 |
| few            | 2 months   | 2 miesiące   | 2-4, 22-24, 32-34, 42-44, 52-54, 62, 102, 1002, … |
| many           | 5 months   | 5 miesięcy   | 0, 5-19, 100, 1000, 10000, 100000, 1000000, … |
| other          | 1.5 months | 1,5 miesiąca | 0.0-1.5, 10.0, 100.0, 1000.0, 10000.0, 100000.0, 1000000.0, … |

## Gender

English doesn't have very many gendered nouns, but it does have a few relevant to Callsheet. The words "actor" and "actress" are a good example.

However, other languages have a lot more words that can vary this way. Here is an example problem using the term "Director of Photography" in French:

| Pronoun | English                  | French |
| :------ | :----------------------- | :----- |
| She/her | Director of Photography: | Directrice de la Photographie: |
| He/him  | Director of Photography: | Directeur de la Photographie: |

Here, the problem is that the gender of a person is ambiguous in translation to French. The origin data is in English, so it can be best to avoid this ambiguity by rephrasing.

| English            | French |
| :----------------- | :----- |
| Cinematography by: | Cinématographie par: |

Uses of [grammatical gender](https://blog.duolingo.com/what-is-grammatical-gender/) are fine. The trailing parts of the first example say "de la Photographie". That's in the feminine for both, because "photographie" has that grammatical gender.

Other languages have [even more of these](https://blog.duolingo.com/german-gender-der-die-das/).

**In general, where it's appropriate and doesn't sound clunky, please use your language's equivalent of "they"/"them" or a genderless word. If not possible, not appropriate, or it just sounds super funky, please choose a sensible default.**

## Submission Flow

I've never done this before, so I'm working this out as we go, as well. But here's my vision for how I hope this will work:

1. [Fork this repository](https://github.com/cliss/callsheet-localizations/fork)
2. Perform whatever translations you want
    * Please don't feel obligated to do the whole document! Any little bit helps!
3. Create a pull request to this repository
4. I'll review, and, short of a major issue, accept the PR
5. We both get to enjoy Callsheet being in one more language!
6. If you happen to be an [ATP](https://atp.fm/) listener, and if you _do_ complete an entire language's localization, let me know, and maybe an ATP sticker will get mailed to you. 😏

## Wait, there are forks other than cutlery and roads?

I'm guessing you're not experienced with Github. No problem! Reach out (see below) and we'll see if there's an alternative approach we can use. 😊

## What if my language isn't here?

Reach out (see below) and I'll be happy to add it!

## Questions?

Please [say something on Mastodon](https://mastodon.social/@caseyliss) or [contact me](https://www.caseyliss.com/contact).
