# callsheet-localizations
Localization Files for [Callsheet](https://apps.apple.com/us/app/callsheet-find-cast-crew/id1672356376).

## Basics

This repository contains a series of [string catalog](https://developer.apple.com/documentation/xcode/localizing-and-varying-text-with-a-string-catalog) files. They contain a series of translatable snippets, and, eventually, their translations.

The easiest way to open and modify these files &mdash; other than using [Xcode](https://developer.apple.com/xcode/) &mdash; is to use the free macOS app [Loca Studio](https://www.cunningo.com/locastudio/index.html).

## Using Loca Studio

Generally speaking, you can look at the `ID` column, and provide a translation in the `Target` column. However, there are some special cases:

### Plurality

For some items, like age, will occasionally have a singular and a plural form. Look at the ages shown here:

<img width="380" alt="Screenshot 2024-05-10 at 8 27 46 PM" src="https://github.com/cliss/callsheet-localizations/assets/282460/419dcd21-d3f4-44ec-8d47-87fffc36c3ef">

This isn't _super_ obvious in Loca Studio:

<img width="410" alt="Screenshot 2024-05-10 at 8 24 59 PM" src="https://github.com/cliss/callsheet-localizations/assets/282460/af01548a-6f2a-4b2d-aa5d-3139ba935370">

Note that the `Source` column kind of hints at what's going on here, but the `ID` column shows `plural-one` for the singular version and `plural-other` for the plural version. Fill each in as appropriate, please.

## Submission Flow

I've never done this before, so I'm working this out as we go, as well. But here's my vision for how I hope this will work:

1. [Fork this repository](https://github.com/cliss/callsheet-localizations/fork)
2. Perform whatever translations you want
    * Please don't feel obligated to do the whole document! Any little bit helps!
3. Create a pull request to this repository
4. I'll review, and, short of a major issue, accept the PR
5. We both get to enjoy Callsheet being in one more language!
6. If you happen to be an [ATP](https://atp.fm/) listener, and if you _do_ complete an entire language's localization, let me know, and maybe an ATP sticker will get mailed to you. 😏

## What if my language isn't here?

Reach out (see below) and I'll be happy to add it!

## Questions?

Please [say something on Mastodon](https://mastodon.social/@caseyliss) or [contact me](https://www.caseyliss.com/contact).

