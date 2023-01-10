# RusTextMorpher v1.2

 An engine to obscure and depersonalize user's text for russian and english languages.
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
shuffle_uniqcode = True
shuffle_wnlines = True
shuffle_uppercase = True
shuffle_errors = True
shuffle_translit = True