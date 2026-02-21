# PHP Superglobals Cheat Sheet
| تابع | تا
## PHP Variable & String Functions – Compact Cheat Sheet (3 Columns)

| | | |
|---|---|---|
| `boolval(1) -> true` | `debug_zval_dump(1) -> int(1)` | `empty("") -> true` |
| `floatval("3.2") -> 3.2` | `get_defined_vars() -> array` | `get_resource_type(fopen("a.txt","r")) -> stream` |
| `gettype(10) -> integer` | `import_request_variables("gp") -> null` | `intval("5") -> 5` |
| `is_array([]) -> true` | `is_bool(true) -> true` | `is_callable("strlen") -> true` |
| `is_countable([]) -> true` | `is_float(1.2) -> true` | `is_int(3) -> true` |
| `is_iterable([]) -> true` | `is_null(null) -> true` | `is_numeric("12") -> true` |
| `is_object(new stdClass()) -> true` | `is_resource(fopen("a.txt","r")) -> true` | `is_scalar("a") -> true` |
| `is_string("a") -> true` | `isset($a) -> false` | `print_r([1,2]) -> Array` |
| `serialize([1,2]) -> a:2:{i:0;i:1;i:1;i:2;}` | `settype($a,"int") -> true` | `strval(10) -> "10"` |
| `unserialize("i:5;") -> 5` | `unset($a) -> null` | `var_dump(1) -> int(1)` |
| `var_export(1,true) -> 1` | `String Functions` |  |
| `addcslashes("hello","e") -> h\e\llo` | `addslashes("O'Reilly") -> O\'Reilly` | `bin2hex("AB") -> 4142` |
| `chop("hello ") -> hello` | `chr(65) -> A` | `chunk_split("Hello",2,"-") -> He-ll-o-` |
| `convert_cyr_string("тест","d","w") -> test` | `convert_uudecode("hZ") -> h` | `convert_uuencode("hi") -> h+` |
| `count_chars("hello",1) -> Array` | `crc32("hello") -> 907060870` | `crypt("pass") -> $6$...` |
| `echo "hi"` | `explode(" ","a b") -> Array` | `fprintf(STDOUT,"%s","hi") -> 2` |
| `get_html_translation_table(HTML_SPECIALCHARS)` | `hebrev("text") -> ...` | `hebrevc("text") -> ...` |
| `hex2bin("41") -> A` | `html_entity_decode("&lt;") -> <` | `htmlentities("<") -> &lt;` |
| `htmlspecialchars_decode("&lt;") -> <` | `htmlspecialchars("<") -> &lt;` | `implode("-",["a","b"]) -> a-b` |
| `lcfirst("Hello") -> hello` | `levenshtein("kitten","sitting") -> 3` | `localeconv() -> Array` |
| `ltrim(" hello") -> hello` | `md5("hello") -> 5d41402abc4b2a76b9719d911017c592` | `md5_file("file.txt") -> hash` |
| `metaphone("hello") -> HL` | `money_format("%i",1234.56) -> $1,234.56` | `nl_langinfo(CODESET) -> UTF-8` |
| `nl2br("a\nb") -> a<br>b` | `number_format(1234.56) -> 1,235` | `ord("A") -> 65` |
| `parse_str("a=1&b=2") -> a=1,b=2` | `print("hi") -> hi` | `printf("%d",5) -> 5` |
| `quoted_printable_decode("=41") -> A` | `quoted_printable_encode("A") -> =41` | `quotemeta(".$") -> \.\$` |
| `rtrim("hi ") -> hi` | `setlocale(LC_ALL,"en_US") -> en_US` | `sha1("hello") -> aaf4c61ddcc5e8a2` |
| `sha1_file("file.txt") -> hash` | `similar_text("hi","he") -> 1` | `soundex("hello") -> H400` |
| `sprintf("%d",5) -> 5` | `sscanf("10","%d") -> 10` | `str_getcsv("a,b") -> Array` |
| `str_ireplace("a","b","A") -> B` | `str_pad("hi",5,"_") -> hi___` | `str_repeat("hi",2) -> hihi` |
| `str_replace("a","b","abc") -> bbc` | `str_rot13("abc") -> nop` | `str_shuffle("abc") -> bac` |
| `str_split("abc",1) -> Array` | `str_word_count("hi world") -> 2` | `strcasecmp("a","A") -> 0` |
| `strcmp("a","b") -> -1` | `strcoll("a","b") -> -1` | `strcspn("abc","b") -> 1` |
| `strip_tags("<b>hi</b>") -> hi` | `stripcslashes("h\e") -> he` | `stripslashes("O\'Reilly") -> O'Reilly` |
| `stripos("Hello","h") -> 0` | `stristr("Hello","h") -> Hello` | `strlen("Hello") -> 5` |
| `strnatcasecmp("a1","A2") -> -1` | `strnatcmp("a1","A2") -> -1` | `strncasecmp("abc","ABC",2) -> 0` |
| `strncmp("abc","ABC",2) -> 1` | `strpbrk("hello","eo") -> e` | `strpos("hello","e") -> 1` |
| `strrchr("hello","l") -> llo` | `strrev("abc") -> cba` | `strripos("Hello","l") -> 3` |
| `strrpos("Hello","l") -> 3` | `strspn("abcde","abc") -> 3` | `strstr("hello","e") -> ello` |
| `strtok("a,b,c",",") -> a` | `strtolower("HELLO") -> hello` | `strtoupper("hello") -> HELLO` |
| `strtr("abc","a","A") -> Abc` | `substr("hello",1,3) -> ell` | `substr_compare("hello","ell",1,3) -> 0` |
| `substr_count("hello","l") -> 2` | `substr_replace("hello","i",4) -> helli` | `trim(" hi ") -> hi` |
| `ucfirst("hello") -> Hello` | `ucwords("hello world") -> Hello World` | `vfprintf(STDOUT,"%d",5) -> 1` |
| `vprintf("%d",5) -> 5` | `vsprintf("%d",5) -> 5` | `wordwrap("Hello World",5) -> Hello\nWorld` |
