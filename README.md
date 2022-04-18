printf - format and print data

This is our printf function recoded from scratch, for education purpose.
Authorized functions and macros

    write (man 2 write)
    malloc (man 3 malloc)
    free (man 3 free)
    va_start (man 3 va_start)
    va_end (man 3 va_end)
    va_copy (man 3 va_copy)
    va_arg (man 3 va_arg)

Custom functions prototypes

    int _putchar(char c);
    int _printf(const char *format, ...);
    int(*getspecifier(char))(va_list);

Functions in file (fn_char.c) :

    int print_c(va_list c);
    int print_s(va_list s);
    int print_S(va_list S);
    int print_rs(va_list rs);
    int print_rot(va_list ro);

Functions in file (fn_numbers.c) :

    int _print_i(va_list vi);
    int _print_b(va_list b);

Functions in file (fn_uoxX.c) :

    int _print_u(va_list u);
    int _print_o(va_list o);
    int _print_x(va_list o);
    int _print_X(va_list o);
    int _print_p(va_list p);


File Descriptions

_printf.c: - contains the _printf function, which uses the prototype int _printf(const char *format, ...);.The format string is composed of zero or more directives. See man 3 printf for more detail. _printf will return the number of characters printed (excluding the null byte used to end output to strings) and will write output to stdout, the standard output stream.

_putchar.c: - contains the function _putchar, which writes a character to stdout.

main.h: - contains all function prototypes used for _printf.

man_3_printf: - manual page for the custom _printf function.

fn_char.c: - contains the functions print_char, print_string, print_porc, and print_rev which handle the conversion specifiers c, s, %, and r, respectively, as well as
print_bin, which prints binary numbers.

getspecifier.c: - which contains the structure array to find the function that the program needs to execute for each format.
