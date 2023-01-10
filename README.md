# RusTextMorpher v1.2

 An engine to obscure and depersonalize user's text for russian and english languages with advanced obfuscations.
 Скрипт для офбускации и деперсонализации пользовательского текста.

 An engine let to configure obfuscation methods and return a similararity bitween original and obscured text.
 Позволяет гибко настраивать методы обфускации и возвращает результат в виде процента похожести оригинального и обфусцированного текста.

### Features :
- Automatic text language detection
- obscure by replacing Latin characters with cyrillic and reverse
- obscure of uincode characters with analogues of characters in the text in random order
- obscure of random substitution of characters for lower and upper case.
- obscure of the passage of random errors in words.
- obscure of sequential text division in random places.
- obscure of special characters to analogues.

### Возможности:
- Автоматическое определение языка текста
- Обфускация с помощью замены латинских символов на кирильские и обратно 
- Обфускация юинкодными символами аналогами символов в тексте в случайном порядке
- Обфускация путем случайной замены символов на нижний и верхний регистр.
- Обфускация путем помещения случайных ошибок в словах.
- Обфускация путем разбития текста в случайных местах.
- Обфускация спец символов на аналоги.

### Config
* shuffle_uniqcode = True
* shuffle_wnlines = True
* shuffle_uppercase = True
* shuffle_errors = True
* shuffle_translit = True

### TODO:
- Add replacements with words alternatives.

### Examples:

/============ Original text: =================

It may be audacious even to attempt a definition of his greatness, but it is not so difficult to describe the gifts that enabled him to create imaginative visions of pathos and mirth that, whether read or witnessed in the theatre, fill the mind and linger there. He is a writer of great intellectual rapidity, perceptiveness, and poetic power. 

/=============================================
Original Language detection:  en
/============ Obfuscated text: ===============

iТ may be audaсiоUs even То aтТEmрТ a definiТiОn оf his greaтness, buТ iТ iS nоТ Sо
DIffiсulТ То DesсRibe Тhe gifТs ТHaТ enabled him То сreaТe imAginaТive vIsIоNs оf
рaТHОS and mirтh ТhaТ, whEТher read оO WiтnEsseD In тhe ТheaТrP, fiLl Тhe mINd And
linger Тhere. HE is a wRIТer Af GrEAТ iNТelleстual raрidiТy, рerсEрТiveneSs, and
рОEтiс роweR.
/=============================================
Obscured Language detection:  en
Similararity: 0.22674418604651161
/=============================================

...

/============ Obfuscated text: ===============

It măy uę ăudăciōus Ęvęn Tō ĂtTęmpt ă dęFinitiōn ōf his gręătnęos, But it is Nōt sō difficult Tō
dęscribę Thę gifts thăt ęnăBlĘd Him tō cręătę imăgiNătiVę viSiōns ōF păthōs ĂnD Mirth thăt, whęthĘr
rĘăd ōr witnęssĘd In thę tHęătrę, filL thę mind ĂNd Lingęr thĘrę; Нę is ă writęr ōf Gręăt
inTęllęcTuăl răpOditY, pęrcęPtivęnęsS, ănd pōĘtic pōwęr;
/=============================================
Obscured Language detection:  en
Similararity: 0.0377906976744186
/=============================================

...

/============ Original text: =================

Суперхит-инструкция к простой жизни: сказать «нет», когда нужно, сделать из неудач мост к переменам или радоваться, с легкостью решая любые проблемы.
Нескучная философия: офисный работник, погрязший в рутине, забредает в кафе «Почему». Здесь он находит новый смысл жизни и осознает свои желания.

/=============================================
Original Language detection:  ru
============ Obfuscated text: ===============

SupeRhit-instrUktsija k pRosToj zhizNi: Skazat' «net», koGda nuzhno, sdelat' iz neuDaCh Most k
PerEmEnam iLA radovFt'sja, s leGKost'ju rEshaja ljubyeSPRoblemy. neskuchnaja filOsofija: ofisnYj
raBotnik, poGRjAzshij v Rutine, zABrEdaeT V Kafe «Pochemu». ZdEs' On nahodit novyj smysl zHizni i
osoznaEt svoi zhElAnija.
/=============================================
Obscured Language detection:  sl
similararity: 0.05245901639344262
/=============================================
...
/============ Obfuscated text: ===============

СуПерxит-инсТрУкция к прoсТoй жизни: сказатЬ «нЕт», кOгда НУжнO, сделАТЬ ИT нzУДаЧ мoст к
переменам Или раДOваться, с легкoстью РЕШая любые прoблЕмы. неСкучная филoсoфия: Oфисный
рАбoтник, пoVрязшиЙ в РУтине, ЗабреДаеТ в кафЕ «пoчему». здесЬ oн наxoдит нOвыЙ смысл жизНи и
oсOзнает сВoи жеЛания.
/=============================================
Obscured Language detection:  ru
Similararity: 0.3147208121827411
/=============================================

....

Diff details:

    Delete "I" from position 0
    Delete "t" from position 1
    Add "i" to position 2
    Add "Т" to position 3
    Delete "c" from position 16
    Add "с" to position 17
    Delete "o" from position 19
    Delete "u" from position 20
    Add "о" to position 21
    Add "U" to position 22
    Delete "t" from position 30
    Delete "o" from position 31
    Add "Т" to position 32
    Add "о" to position 33
    Delete "t" from position 36
    Delete "t" from position 37
    Delete "e" from position 38
    Add "т" to position 39
    Add "Т" to position 40
    Add "E" to position 41
    Delete "p" from position 43
    Delete "t" from position 44
    Add "р" to position 45
    Add "Т" to position 46
    Delete "t" from position 56
    Add "Т" to position 57
    Delete "o" from position 59
    Add "О" to position 60
    Delete "o" from position 63
    Add "о" to position 64
    Delete "t" from position 75
    Add "т" to position 76
    Delete "t" from position 85
    Add "Т" to position 86
    Delete "t" from position 89
    Add "Т" to position 90
    Delete "s" from position 93
    Add "S" to position 94
    Delete "o" from position 97
    Delete "t" from position 98
    Add "о" to position 99
    Add "Т" to position 100
    Delete "s" from position 102
    Delete "o" from position 103
    Delete " " from position 104
    Delete "d" from position 105
    Delete "i" from position 106
    Add "S" to position 107
    Add "о" to position 108
    Add "
    " to position 109
    Add "D" to position 110
    Add "I" to position 111
    Delete "c" from position 115
    Add "с" to position 116
    Delete "t" from position 119
    Add "Т" to position 120
    Delete "t" from position 122
    Delete "o" from position 123
    Add "Т" to position 124
    Add "о" to position 125
    Delete "d" from position 127
    Add "D" to position 128
    Delete "c" from position 131
    Delete "r" from position 132
    Add "с" to position 133
    Add "R" to position 134
    Delete "t" from position 139
    Add "Т" to position 140
    Delete "t" from position 147
    Add "Т" to position 148
    Delete "t" from position 151
    Delete "h" from position 152
    Add "Т" to position 153
    Add "H" to position 154
    Delete "t" from position 156
    Add "Т" to position 157
    Delete "t" from position 171
    Delete "o" from position 172
    Add "Т" to position 173
    Add "о" to position 174
    Delete "c" from position 176
    Add "с" to position 177
    Delete "t" from position 181
    Add "Т" to position 182
    Delete "a" from position 187
    Add "A" to position 188
    Delete "t" from position 193
    Add "Т" to position 194
    Delete "i" from position 200
    Add "I" to position 201
    Delete "i" from position 203
    Delete "o" from position 204
    Delete "n" from position 205
    Add "I" to position 206
    Add "о" to position 207
    Add "N" to position 208
    Delete "o" from position 211
    Add "о" to position 212
    Delete " " from position 214
    Delete "p" from position 215
    Add "
    " to position 216
    Add "р" to position 217
    Delete "t" from position 219
    Delete "h" from position 220
    Delete "o" from position 221
    Delete "s" from position 222
    Add "Т" to position 223
    Add "H" to position 224
    Add "О" to position 225
    Add "S" to position 226
    Delete "t" from position 235
    Add "т" to position 236
    Delete "t" from position 239
    Add "Т" to position 240
    Delete "t" from position 243
    Add "Т" to position 244
    Delete "e" from position 249
    Delete "t" from position 250
    Add "E" to position 251
    Add "Т" to position 252
    Delete "o" from position 262
    Add "о" to position 263
    Add "O" to position 264
    Add " " to position 265
    Add "W" to position 266
    Add "i" to position 267
    Add "т" to position 268
    Add "n" to position 269
    Add "E" to position 270
    Add "s" to position 271
    Add "s" to position 272
    Add "e" to position 273
    Add "D" to position 274
    Add " " to position 275
    Add "I" to position 276
    Add "n" to position 277
    Add " " to position 278
    Add "т" to position 279
    Add "h" to position 280
    Add "e" to position 281
    Add " " to position 282
    Add "Т" to position 283
    Add "h" to position 284
    Add "e" to position 285
    Add "a" to position 286
    Add "Т" to position 287
    Add "P" to position 289
    Add "," to position 290
    Add " " to position 291
    Add "f" to position 292
    Add "i" to position 293
    Add "L" to position 294
    Add "l" to position 295
    Add " " to position 296
    Add "Т" to position 297
    Add "h" to position 298
    Add "e" to position 299
    Add " " to position 300
    Add "m" to position 301
    Add "I" to position 302
    Add "N" to position 303
    Add "d" to position 304
    Add " " to position 305
    Add "A" to position 306
    Add "n" to position 307
    Add "d" to position 308
    Add "
    " to position 309
    Add "l" to position 310
    Add "i" to position 311
    Add "n" to position 312
    Add "g" to position 313
    Add "e" to position 314
    Add "r" to position 315
    Add " " to position 316
    Add "Т" to position 317
    Add "h" to position 318
    Add "e" to position 319
    Add "r" to position 320
    Add "e" to position 321
    Add "." to position 322
    Add " " to position 323
    Add "H" to position 324
    Add "E" to position 325
    Add " " to position 326
    Add "i" to position 327
    Add "s" to position 328
    Add " " to position 329
    Add "a" to position 330
    Delete "i" from position 333
    Delete "t" from position 334
    Delete "n" from position 335
    Add "R" to position 336
    Add "I" to position 337
    Add "Т" to position 338
    Delete "s" from position 340
    Delete "s" from position 341
    Delete "e" from position 342
    Delete "d" from position 343
    Delete " " from position 344
    Delete "i" from position 345
    Delete "n" from position 346
    Delete " " from position 347
    Delete "t" from position 348
    Delete "h" from position 349
    Delete "e" from position 350
    Delete " " from position 351
    Delete "t" from position 352
    Delete "h" from position 353
    Delete "e" from position 354
    Delete "a" from position 355
    Delete "t" from position 356
    Delete "e" from position 358
    Delete "," from position 359
    Add "A" to position 361
    Delete "i" from position 363
    Delete "l" from position 364
    Delete "l" from position 365
    Add "G" to position 367
    Delete "t" from position 368
    Delete "h" from position 369
    Delete "e" from position 370
    Delete " " from position 371
    Delete "m" from position 372
    Delete "i" from position 373
    Delete "n" from position 374
    Delete "d" from position 375
    Delete " " from position 376
    Delete "a" from position 377
    Delete "n" from position 378
    Delete "d" from position 379
    Delete " " from position 380
    Delete "l" from position 381
    Delete "i" from position 382
    Delete "n" from position 383
    Delete "g" from position 384
    Delete "e" from position 385
    Add "E" to position 387
    Add "A" to position 388
    Add "Т" to position 389
    Delete "t" from position 391
    Delete "h" from position 392
    Add "i" to position 393
    Add "N" to position 394
    Add "Т" to position 395
    Delete "r" from position 397
    Add "l" to position 398
    Add "l" to position 399
    Add "с" to position 401
    Add "т" to position 402
    Add "u" to position 403
    Add "a" to position 404
    Add "l" to position 405
    Add " " to position 406
    Add "r" to position 407
    Add "a" to position 408
    Add "р" to position 409
    Add "i" to position 410
    Add "d" to position 411
    Add "i" to position 412
    Add "Т" to position 413
    Add "y" to position 414
    Add "," to position 415
    Add " " to position 416
    Add "р" to position 417
    Add "e" to position 418
    Add "r" to position 419
    Add "с" to position 420
    Add "E" to position 421
    Add "р" to position 422
    Add "Т" to position 423
    Add "i" to position 424
    Add "v" to position 425
    Add "e" to position 426
    Add "n" to position 427
    Add "e" to position 428
    Add "S" to position 429
    Add "s" to position 430
    Add "," to position 431
    Add " " to position 432
    Add "a" to position 433
    Add "n" to position 434
    Add "d" to position 435
    Add "
    " to position 436
    Add "р" to position 437
    Add "О" to position 438
    Add "E" to position 439
    Add "т" to position 440
    Add "i" to position 441
    Add "с" to position 442
    Add " " to position 443
    Add "р" to position 444
    Add "о" to position 445
    Add "w" to position 446
    Add "e" to position 447
    Add "R" to position 448
    Delete " " from position 450
    Delete "H" from position 451
    Delete "e" from position 452
    Delete " " from position 453
    Delete "i" from position 454
    Delete "s" from position 455
    Delete " " from position 456
    Delete "a" from position 457
    Delete " " from position 458
    Delete "w" from position 459
    Delete "r" from position 460
    Delete "i" from position 461
    Delete "t" from position 462
    Delete "e" from position 463
    Delete "r" from position 464
    Delete " " from position 465
    Delete "o" from position 466
    Delete "f" from position 467
    Delete " " from position 468
    Delete "g" from position 469
    Delete "r" from position 470
    Delete "e" from position 471
    Delete "a" from position 472
    Delete "t" from position 473
    Delete " " from position 474
    Delete "i" from position 475
    Delete "n" from position 476
    Delete "t" from position 477
    Delete "e" from position 478
    Delete "l" from position 479
    Delete "l" from position 480
    Delete "e" from position 481
    Delete "c" from position 482
    Delete "t" from position 483
    Delete "u" from position 484
    Delete "a" from position 485
    Delete "l" from position 486
    Delete " " from position 487
    Delete "r" from position 488
    Delete "a" from position 489
    Delete "p" from position 490
    Delete "i" from position 491
    Delete "d" from position 492
    Delete "i" from position 493
    Delete "t" from position 494
    Delete "y" from position 495
    Delete "," from position 496
    Delete " " from position 497
    Delete "p" from position 498
    Delete "e" from position 499
    Delete "r" from position 500
    Delete "c" from position 501
    Delete "e" from position 502
    Delete "p" from position 503
    Delete "t" from position 504
    Delete "i" from position 505
    Delete "v" from position 506
    Delete "e" from position 507
    Delete "n" from position 508
    Delete "e" from position 509
    Delete "s" from position 510
    Delete "s" from position 511
    Delete "," from position 512
    Delete " " from position 513
    Delete "a" from position 514
    Delete "n" from position 515
    Delete "d" from position 516
    Delete " " from position 517
    Delete "p" from position 518
    Delete "o" from position 519
    Delete "e" from position 520
    Delete "t" from position 521
    Delete "i" from position 522
    Delete "c" from position 523
    Delete " " from position 524
    Delete "p" from position 525
    Delete "o" from position 526
    Delete "w" from position 527
    Delete "e" from position 528
    Delete "r" from position 529
    Delete "." from position 530
    Delete " " from position 531
    Delete "
    " from position 532
    =============================================
    "a " -   6.38%
    "y " -   0.58%
    "e " -  11.01%
    "c " -   2.03%
    "o " -   4.35%
    "p " -   2.03%
    "H " -   0.29%
    "\n" -   0.29%
    =============================================
    "a " -   5.54% 
    "y " -   0.58% 
    "e " -   8.75% 
    "с " -   2.04% 
    "о " -   3.21% 
    "E " -   2.04% 
    "р " -   2.04% 
    "О " -   0.87% 
    "\n" -   1.17% 
    "H " -   0.87% 
    "A " -   1.17% 
    "O " -   0.29% 
    "P " -   0.29% 