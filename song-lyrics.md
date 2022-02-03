---
title: Songs
description: 
published: true
date: 2022-02-03T10:07:48.437Z
tags: 
editor: markdown
dateCreated: 2021-06-12T12:41:38.182Z
---

# Song Translations

## Kaf

-   [魔女 | majo | Witch](/song-lyrics/majo)
-   [雛鳥 | Hina Dori | Baby Bird](/song-lyrics/baby-bird)
-   [痛みを | Itami Wo | Through the Pain](/song-lyrics/through-the-pain)
-   [花女 | Hanna Onna | Flower Girl](/song-lyrics/flower-girl)

## RIM

-   [法螺話 | Tall Story](/song-lyrics/tall-story)
-   [胎児に月はキスをしない | The Moon Not Kiss the Foetation](/song-lyrics/the-moon-not-kiss-the-foetation)

### NEW ROMANCER

RIM's 1st album, released on 21 Jul 2021.

1.  ピロウトーク | Pillow Talk
2.  [ラヴソング | Love Song](/song-lyrics/love-song)
3.  [さみしいひと | Lonely Person](/song-lyrics/lonely-person)
4.  [宿木 | Mistletoe](/song-lyrics/mistletoe)
5.  [いたいよ | It Hurts](/song-lyrics/it-hurts)
6.  甘美な無法 | Luscious Lawless
7.  食虫植物 | Carnivorous Plant
8.  胎児に月はキスをしない | The Moon Not Kiss the Foetation
9.  [NEUROMANCE](/song-lyrics/neuromance)
10.  ユーエンミー | You and Me
11.  クライベイビー | Cry Baby
12.  [魔的 feat. 花譜 | Magical feat. Kaf](/song-lyrics/magical)
13.  [やさしくしないで | Don't be Kind to Me](/song-lyrics/dont-be-kind-to-me)
14.  十九月 | 19 - Month

## koko

-   [この世界に口づけを | To Kiss This World](/song-lyrics/to-kiss-this-world)

# Editor Notes

## Style Guide

Note: these are guides, not strict rules. This is a wiki, just throw stuff up here and I'll format it later, maybe when I have time.

I'm still experiementing with different stuff, and don't have time to follow all these strictly either. These are just reminders.

### Metadata

The title should be the translated english song name.

The subtitle should have the original japanese song name, romanji translation of the song name, and vocalist. These are helpful when people are searching, which'll only show the title and subtitle of a page.

The location (aka link) to the page should be same as the title, but formatted into all lowercase, and use hyphens for spaces. For example, "/to-kiss-this-world" for "To Kiss This World".

Probably should tag a page with the vocalist, maybe genre? we'll have to decide what tags are needed later.

#### CSS: Lyrics Table Style

We're using css to remove horizontal line breaks between rows in the lyrics tables, and to reduce padding (spacing) between rows.

Custom CSS for a page can be edited at: edit a page -> blue "Page" action top right -> "Styles tab

Whe creating a page, copy from an already styled page and place in the new page. [Here's one styled page](/song-lyrics/to-kiss-this-world).

### Introduction

A song page should have an introduction section, that has the following:

-   Initial release date and format (MV or album)
-   Link to: where to stream (youtube, spotify), to buy (store)
-   Versions (variations) of the song, if any
-   producers: writing, arranging, composing, mixing
-   maybe include other musicians (guitar / drums etc.)
-   illustrator / animator (for MV)

The introduction section to a song does not need a header.

## Ruby Annotation

We can typeset furigana, or hiragana annotations on top of kanjis, by using the [ruby annotations](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ruby). The standard `<ruby>` HTML tag is implemented in all major browsers.

##### Tabs {.tabset}

###### code

```
<ruby>痛<rt>いた</rt>みを</ruby>
```

###### rendered

痛いたみを

### Problem: Markdown Support

We have to write the raw ruby HTML tags inside markdown. There is no builtin support for generating ruby HTML tags from markdown. (Wiki.js takes markdown code, generates HTML code, then displays it.)

The biggest reason of using markdown editor instead of HTML is that it's cleaner. Markdown is less verbose, easier to write, look at, and edit. Not having a clean way to write ruby annotations in markdown undermines this.

If we're to implement ruby support in markdown, we first need to find a library, if we don't want to decide on the syntax and write code ourselves. There are a few libraries, one candidate might be [markdown-it-ruby](https://github.com/n-inja/markdown-it-ruby). And to actually use the library, we'll need to create a Pull Request on [Wiki.js](https://github.com/Requarks/wiki), or fork it and implement ourselves. See [this PR](https://github.com/Requarks/wiki/pull/2126/files) for reference.

But that's a lot of work, so we can just simply write less ruby annotations and call it a day, but:

### Problem: When to Use

Ruby annotations are helpful for people learning japanese, especially on difficult kanjis (溢?), and on uncommon readings (愛 as いと instaed of あい?).

Having annotations on all kanjis can be helpful to beginners (me), but too many annotations might be distracting, and ruby annotations are annoying to write and edit.

I'm not sure whrere's the balance on when to use ruby annotations, or maybe just not use annotations at all because it's too much work.

## Tabs

I wasn't sure if we want to present the english lyrics only (copy-paste-done), or want to make a jp-en side-by-side thing. So I tried both and placed them in tags to compare. But the tabs thing looks good too so we're keeping the tabs now.

Reference: https://docs.requarks.io/en/editors/markdown#content-tabs