---
layout: post
title:  "Dictionary C# API"
date:   2017-08-20 00:00:00 +0100
categories: Release
---

Today I am releasing C# 37 Languages Online Free[Dictionary API V1.0](https://github.com/AndMu/Wikiled.Dictionary)

![Nuget](https://img.shields.io/nuget/v/Wikiled.Dictionary.svg)

.NET Standard 1.1

Supports translation from/to English and any of below languages:

* Arabic
* Croatian
* Czech
* Dutch
* Danish
* Esperanto
* Estonian
* Finnish
* French
* German
* Greek
* Hebrew
* Italian
* JapaneseKanaRomaji
* JapaneseKanjiKana
* JapaneseKanjiRomaji
* JapaneseRomajiKanji
* Latin
* Latvian
* Lithuanian
* Norwegian
* Persian
* PersianFarsi
* Polish
* Portuguese
* Romanian
* Russian
* Serbian
* SimpleChinese
* Slovak
* Spanish
* Swedish
* Thai
* Turkish
* Ukrainian
* Yiddish


Samle code:
```C#
	DictionaryManagerFactory factory = new DictionaryManagerFactory();	
	var manager = factory.Construct();
	var request = new TranslationRequest
	{
		From = Language.English,
		To = Language.German,
		Word = "Love"
	};
	var result = await manager.Translate(request, CancellationToken.None);		
```
