# PHP Superglobals Cheat Sheet
| تابع | تا
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
| `var_export(1,true) -> 1` |  |  |
