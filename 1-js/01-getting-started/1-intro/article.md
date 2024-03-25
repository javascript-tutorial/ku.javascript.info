# پێشەکییەک لە جاڤاسکڕێپت

با بزانین چی تایبەتیکی هەیە جاڤاسکڕێپت، دەتوانین چی بەدەست بهێنین لەگەڵیدا، و چ تەکنەلۆژیایەکی دیکە بە باشی کار دەکەن لەگەڵی.

## جاڤاسکڕێپت چییە؟

*جاڤاسکڕێپت* لە سەرەتادا بۆ "بە زیندوویکردنی لاپەڕەکانی وێب" دروستکرا.

بەرنامەکانی ئەم زمانە پێیان دەوترێت *scripts*. دەتوانرێت لە HTML ی پەڕەیکی وێب بنووسرێن و بە بارکردنی لاپەڕەکە بە شێوەیەکی ئۆتۆماتیکی کاربکەن.
سکریپتەکان وەک دەقی سادە دابین دەکرێن و جێبەجێ دەکرێن.

پێویستیان بە ئامادەکاری تایبەت یان کۆکردنەوە نییە بۆ ئەوەی کاربکەن.

لەم لایەنەدا جاڤاسکڕێپت زۆر جیاوازە لە زمانێکی تر بە ناوی [جاڤا](https://ckb.wikipedia.org/wiki/%D8%AC%D8%A7%DA%A4%D8%A7_(%D8%B2%D9%85%D8%A7%D9%86%DB%8C_%D8%A8%DB%95%D8%B1%D9%86%D8%A7%D9%85%DB%95%D8%B3%D8%A7%D8%B2%DB%8C))


```smart header="بۆچی پێی دەوترێت <u>جاڤا؟</u>script>"
کاتێک جاڤاسکڕێپت دروستکرا، سەرەتا ناوێکی دیکەی هەبوو: "Livescript".بەڵام جاڤا لەو کاتەدا زۆر بەناوبانگ بوو، بۆیە بڕیاردرا کە جێگیرکردنی زمانێکی نوێ وەک "برایەکی بچووکتر"ی جاڤا یارمەتیدەر بێت.

بەڵام لەگەڵ پەرەسەندندا، جاڤاسکڕێپت بوو بە زمانێکی تەواو سەربەخۆ کە تایبەتمەندی خۆی هەبوو و بوو بە [ئێکماسکڕێپت](https://en.wikipedia.org/wiki/ECMAScript)،وە ئێستا بە هیچ شێوەیەک پەیوەندی بە جاڤاوە نییە.
```

ئەمڕۆ، جاڤاسکڕێپت دەتوانێت نەک تەنها لە وێبگەڕەکەدا کار بکات، بەڵکو لەسەر سێرڤەر، یان لە ڕاستیدا لەسەر هەر ئامێرێک کە بەرنامەیەکی تایبەتی هەبێت بە ناوی [JavaScript engine](https://en.wikipedia.org/wiki/JavaScript_engine).

وێبگەڕەکە بزوێنەرێکی جێگیرکراوی هەیە، هەندێک جار پێی دەوترێت "ئامێری مەجازی جاڤاسکڕێپت".

بزوێنەرە جیاوازەکان "کۆدناوی(codenames)" جیاوازیان هەیە. بۆ نموونە:


- [ڤی ٨](https://en.wikipedia.org/wiki/V8_(JavaScript_engine)) -- لە کرۆم و ئۆپێرا و ئێدج.
- [ئێسپایدرمانکی](https://en.wikipedia.org/wiki/SpiderMonkey) -- لە فایرفاکس.
-   کۆدناوی دیکەش هەن وەک "چاکرا" بۆ IE ،  "جاڤاسکڕێپت کۆر"، "نیترۆ" و "SquirreLish" بۆ سەفاری و هتد.

-   باشە ئەو کۆدناوەکانی سەرەوە لەبیرمان بمێنێ چونکە لە بابەتەکانی گەشەپێدەران لە ئینتەرنێتدا بەکاردێت.ئێمەش بەکاریان دەهێنین. بۆ نموونە,ئەگەر "تایبەتمەندییەک X لەلایەن V8 پشتگیری بکرێت" ، پاشان ئەگەری زۆرە لە کرۆم و ئۆپێرا و ئێدجدا کار بکات


```smart header="بزوێنەرەکان چۆن کاردەکەن؟"

بزوێنەرەکان ئاڵۆزن. بەڵام بنەماکان ئاسانن.

1. بزوێنەرەکە (ئەگەر وێبگەڕێک بێت بزوێنەرەکە لە نێوخۆی جێگیربووە) سکریپتەکە دەخوێنێتەوە ("وە شیکاری دەکات").
2. پاشان سکریپتەکە دەگۆڕێت بۆ کۆدی ماشین ("کامپایڵکردن").
3. و پاشان کۆدی ماشین زۆر بە خێرایی کاردەکات.

بزوێنەرەکە لە هەر هەنگاوێکدا هەوڵ ئەدات پرۆسەکە باشتر و خێراتر بکات. تەنانەت کاتێ کە ئێسکرێپتەکە کامپایڵ بووە بزوێنەرەکە کارکردنی ئێسکڕێپتەکە ئەگرێتە ژێرچاودێری ، ئەو زانیاریانە کە لە ڕێگای ئێسکڕێپت ئێمە تێن وە ئەچنیش شی دەکاتەوە ، وە بەپێی ئەم زانیاریەنە کە لە ڕێگای چاودێریکردن وە شی کردنەوەی دیتاکانی هات و چوو کراوەی ئێسکرێپتەکە کۆیکردەسەو کۆدی ماشینەکە باشتر و گونجاوتر دەکات بەپشتبەستن بەو زانیاریەکانی خۆی
```

## جاڤاسکڕێپت لە ناو وێبگەڕە چی دەتوانێ بکات؟

جاڤاسکڕێپتی مۆدێرن زمانێکی بەرنامەسازی "ئەمنە". دەستگەیشتن بە ئاستی نزم بۆ بیرگە یان CPU نادات چونکە لە سەرەتادا بۆ ئەو وێبگەڕانە دروستکراوە کە پێویستیان پێی نییە.

تواناکانی جاڤاسکڕێپت تا ڕادەیەکی زۆر پشت بەو ژینگەیە دەبەستێت کە تێیدا کاردەکات.[Node.js](https://ckb.wikipedia.org/wiki/%D9%86%DB%86%D8%AF_%D8%AC%DB%95%DB%8C_%D8%A6%DB%8E%D8%B3) پشتگیری لەو فانکشنەنە دەکات کە ڕێگە بە جاڤاسکڕێپت دەدەن فایلە دڵخوازەکان بخوێنێتەوە/بینووسێت، داواکاری تۆڕەکان دروست بکات و هتد.

جاڤاسکڕێپت لە وێبگەڕەکەدا دەتوانێت هەموو ئەرکەکانی دەستکاریکردنی لاپەڕەکانی وێب، وەڵام دانەوەی داواکاریەکانی بەکارهێنەر و سێرڤەری وێب ئەنجام بدات.



بۆ نموونە جاڤاسکڕێپت لەناو وێبگەڕەکەدا توانای هەیە:

- ئێچ تی ئێم ئێڵ یان HTML ی نوێ زیاد بکە بۆ لاپەڕەکە، ناوەڕۆکەکان وە ستایلەکان بگۆڕێت.
- کاردانەوە بەرامبەر بە کردارەکانی بەکارهێنەر بێت، کرتە لە ماوس کردن، جوڵانەوەی ماوس، فشار دان دوکمەکانی کیبۆرد، بۆ هەموو ئەمانە دەتوانن کاردانەوەیکی تایبەت ئامادە وە جێبەجێکەن
- ناردنی داواکاری لە ڕێگەی تۆڕەوە بۆ سێرڤەرە دوورەکان، دانلود و ئاپلۆد فایلەکان (کە پێی دەوترێت [AJAX](https://en.wikipedia.org/wiki/Ajax_(programming)). و تەکنەلۆژیای [COMET](https://en.wikipedia.org/wiki/Comet_(programming))

- کووکی وەرگرتن و ڕێکخستن، پرسیار لە سەردانکەرەکانی ماڵپەڕەکە بکە، نامەکان پیشان بدە.
- داتاکانی لایەنی کلاینت ("Local Storage") پاشەکەوت بکە.

## جاڤاسکڕێپت لە وێبگەڕەکانە ناتوانێت چی بکات؟

تواناکانی جاڤاسکڕێپت لە وێبگەڕەکاندا سنووردارە بۆ پاراستنی سەلامەتی بەکارهێنەر. ئامانج لێی ڕێگریکردنە لە دەستگەیشتن بە زانیارییە تایبەتەکان یان زیانگەیاندن بە زانیارییەکانی بەکارهێنەر.

نموونەی ئەم سنووردارکردنانە بریتین لە:

- جاڤاسکڕێپت لە وێب پەڕێکدا لەوانەیە فایلە ئارەزوومەندانە لەسەر هارد دیسکەکە بخوێنێتەوە/بنووسێت، کۆپییان بکات، یان بەرنامەکان ئێجرابکات. دەستڕاگەیشتنێکی ڕاستەوخۆی بە کارەکانی سیستەمی کارپێکردن نییە.

    وێبگەڕە مۆدێرنەکان ڕێگەی پێدەدەن کار لەگەڵ فایلەکاندا بکات، بەڵام دەستڕاگەیشتن سنووردارە و تەنها لەو کاتەدا دابین دەکرێت کە بەکارهێنەر هەندێک کردار ئەنجام بدات، وەک "خستنەناو" فایلێک بۆ ناو پەنجەرەی وێبگەڕەکە یان هەڵبژاردنی لە ڕێگەی تاگی `<input>` .

    ڕێگا هەیە بۆ کارلێککردن لەگەڵ کامێرا/مایکرۆفۆن و ئامێرەکانی تر، بەڵام پێویستیان بە مۆڵەتی بەکارهێنەری ڕوون هەیە. کەواتە لاپەڕەیەک کە جاڤاسکڕێپتی هەبێت ڕەنگە بە نهێنی کامێرای وێب چالاک نەکات و دەوروبەرەکەی نەبینێت و زانیاری بۆ [NSA](https://ckb.wikipedia.org/wiki/%D8%AF%DB%95%D8%B2%DA%AF%D8%A7%DB%8C_%D8%A6%D8%A7%D8%B3%D8%A7%DB%8C%D8%B4%DB%8C_%D9%86%DB%95%D8%AA%DB%95%D9%88%DB%95%DB%8C%DB%8C) نەنێرێت.

  
- تاب/پەنجەرە جیاوازەکان بەزۆری ئاگاداری یەکتر نین. هەندێک جار ئاگادار یەک ئەوەن، بۆ نموونە کاتێک پەنجەرەیەک جاڤاسکڕێپت بەکاردەهێنێت بۆ کردنەوەی پەنجەرەیەکی تر. بەڵام تەنانەت لەم حاڵەتەشدا، جاڤاسکڕێپت لە لاپەڕەیەکەوە ڕەنگە نەتوانێت دەستی بگات بە لاپەڕەیەکی تر ئەگەر لە سایتی جیاوازەوە بێت (لە دۆمەین، پرۆتۆکۆڵ، یان دەروازەیەکی جیاوازەوە).

    ئەمەش پێی دەوترێت "Same Origin Policy".بۆ چارەسەرکردنی، *هەردوو لاپەڕەکە* دەبێت ڕازی بن لەسەر ئاڵوگۆڕی داتا، و دەبێت کۆدی تایبەتی جاڤاسکڕێپتیان تێدابێت کە مامەڵە لەگەڵ پەنجەرەکان یا تەبەکان بکات. لە فێرکاریدا باسی ئەم بابەتە دەکەین.
  

    این محدودیت مجدداً برای ایمنی کاربر است. لاپەڕەیەک لە `http://anysite.com` کە بەکارهێنەر کردوویەتیەوە نابێت بۆ نموونە بچێتە ناو تابێکی تری وێبگەڕ بە ئادرسی  `http://gmail.com` و لەوێوە زانیاری بدزێت.

 
- جاڤاسکڕێپت دەتوانێت بە ئاسانی لە ڕێگەی تۆڕەوە پەیوەندی لەگەڵ ئەو سێرڤەرە بکات کە لاپەڕەی ئێستا لێیەوە هاتووە.بەڵام توانای وەرگرتنی زانیاری لە سایت/دۆمەینەکانی ترەوە پەککەوتووە.هەرچەندە دەکرێت، بەڵام پێویستی بە ڕێککەوتنی ڕوون هەیە (بە سەردێڕی HTTP ) لە لایەنی دوورەوە. جارێکی تریش ئەمە سنووردارکردنی ئەمنە بۆ بەکارهێنەرەکان.

![](limitations.svg)


ئەگەر جاڤاسکڕێپت لە دەرەوەی وێبگەڕ بەکاربهێنرێت، بۆ نموونە لەسەر سێرڤەر، هیچ سنووردارکردنێکی لەو جۆرە نییە.هەروەها وێبگەڕە مۆدێرنەکان ڕێگە بە plugins/extensions دەدەن کە ڕەنگە داوای مۆڵەتی درێژتر وە سەختر بکەن.

## What makes JavaScript unique?

There are at least *three* great things about JavaScript:

```compare
+ Full integration with HTML/CSS.
+ Simple things are done simply.
+ Supported by all major browsers and enabled by default.
```
JavaScript is the only browser technology that combines these three things.

That's what makes JavaScript unique. That's why it's the most widespread tool for creating browser interfaces.

That said, JavaScript can be used to create servers, mobile applications, etc.

## Languages "over" JavaScript

The syntax of JavaScript does not suit everyone's needs. Different people want different features.

That's to be expected, because projects and requirements are different for everyone.

So, recently a plethora of new languages appeared, which are *transpiled* (converted) to JavaScript before they run in the browser.

Modern tools make the transpilation very fast and transparent, actually allowing developers to code in another language and auto-converting it "under the hood".

Examples of such languages:

- [CoffeeScript](https://coffeescript.org/) is "syntactic sugar" for JavaScript. It introduces shorter syntax, allowing us to write clearer and more precise code. Usually, Ruby devs like it.
- [TypeScript](https://www.typescriptlang.org/) is concentrated on adding "strict data typing" to simplify the development and support of complex systems. It is developed by Microsoft.
- [Flow](https://flow.org/) also adds data typing, but in a different way. Developed by Facebook.
- [Dart](https://www.dartlang.org/) is a standalone language that has its own engine that runs in non-browser environments (like mobile apps), but also can be transpiled to JavaScript. Developed by Google.
- [Brython](https://brython.info/) is a Python transpiler to JavaScript that enables the writing of applications in pure Python without JavaScript.
- [Kotlin](https://kotlinlang.org/docs/reference/js-overview.html) is a modern, concise and safe programming language that can target the browser or Node.

There are more. Of course, even if we use one of these transpiled languages, we should also know JavaScript to really understand what we're doing.

## Summary

- JavaScript was initially created as a browser-only language, but it is now used in many other environments as well.
- Today, JavaScript has a unique position as the most widely-adopted browser language, fully integrated with HTML/CSS.
- There are many languages that get "transpiled" to JavaScript and provide certain features. It is recommended to take a look at them, at least briefly, after mastering JavaScript.
