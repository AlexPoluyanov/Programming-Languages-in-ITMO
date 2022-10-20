<h1 align="center"> Ответы на онлайн-курс по Языкам Программирования на платформе <a href="https://stepik.org/course/73618/">Stepik</a></h1>
<h2>Список тем:</h2>

<ul>
  <li>
    <h3><a href ="#1">Основы языка С</a></h3>
    <ol type="1">
    	<li><a href ="#1.1">Введение</a></li>
    	<li><a href ="#1.2">Основные правила вычислений</a></li>
    	<li><a href ="#1.3">Условные переходы</a></li>
      <li><a href ="#1.4">Потоки ввода и вывода</a></li>
      <li><a href ="#1.5">Глобальные и локальные переменные</a></li>
      <li><a href ="#1.6">Циклы</a></li>
      <li><a href ="#1.7">Массивы и указатели</a></li>
      <li><a href ="#1.8">Структура кода</a></li>
    </ol>
  
  </li>
  
  <li>
    <h3><a href ="#2">Типы</a></h3>
     <ol type="1">
    	<li><a href ="#2.1">Обзор системы типов, численные типы</a></li>
    	<li><a href ="#2.2">Интерлюдия. Динамическое выделение памяти</a></li>
    	<li><a href ="#2.3">Структуры</a></li>
      <li><a href ="#2.4">Связный список</a></li>
      <li><a href ="#2.5">Объединения и перечисления</a></li>
      <li><a href ="#2.6">Функции</a></li>
      <li><a href ="#2.7">Функции высшего порядка</a></li>
    </ol>
  </li>
  
  <li>
    <h3><a href ="#3">Структура кода</a></h3>
     <ol type="1">
    	<li><a href ="#3.1">Декларативность. Стёк 1.0</a></li>
    	<li><a href ="#3.2">Модульность и абстракция</a></li>
    </ol>
  </li>
</ul>

<h2>Ответы</h2>
<h3 id="1">1. Основы языка С</h3>

<h4 id="1.1">1.1 Введение</h4>
<p>В блоке нет оцениваемых заданий</p>

<h4 id="1.2">1.2 Введение</h4>
<p>❔:   Nevergonna give you up</p><br>

<pre>printf("%d", 17283+(5*6*7*8));</pre>
<pre>void print_newline(){
  printf("\n");
}</pre>

<pre>greet();
b();
print_newline();
greet();
v();
print_newline();
greet();
b();
print_newline();</pre>
<pre>greet(10);
greet(20);
greet(42);</pre>

<pre>void f(int first, int second){
  printf("%d", first+second);
}</pre>

<pre>int avg3(int first, int second, int third){
  return (first+second+third)/3;
}</pre>

<h4 id="1.3">1.3 Условные переходы</h4>
<p>❔:   123</p>
<p>❔:   9</p>
<p>❔:   0</p>
<p>❔:   ✅ 4>3<br>
       ✅      (44 > 99) || (99 > 44)</p>
<p>❔:   
✅ (1 < 3) > 0<br>
       ✅ 1 && 9<br>
       ✅ 0 || 9</p>
       
<pre>// Возвращает 1 если в числе одна цифра, иначе 0
int is_single_digit(int n) {
    return 0 <= n && n <= 9;
}

// Возвращает 1 если в числе ровно две цифры, иначе 0
int is_double_digit(int n) {
    return 10 <= n && n <= 99;
}</pre>
<p>❔:✅ 4 > 3 && print(10)<br>
       ✅ print(0) && print(9)<br>
       ✅ 4 < 3 || print(42) || print(88)</p>
<pre>int is_sorted3(int a, int b, int c) {
    if (a>b && b>c) return -1;
    else return c>b && b>a;
}</pre>
<pre>int max3(int a, int b, int c) {
	if (a < b) { a = b; }
	if (a < c) { a = c; }
	return a;
}</pre>
<pre>void fizzbuzz (int num) {
    if (!(num > 0)) {printf("no"); return;}
    if (num % 3 == 0) {printf("fizz");}
    if (num % 5 == 0) {printf("buzz");}
}</pre>


<h4 id="1.4">1.4 Потоки ввода и вывода</h4>
<p>❔:  ✅ Если мы запустили приложение в эмуляторе терминала, то вызов printf означает, что эмулятор терминала нарисует на экране какой-то текст</p>
<p>❔:  ✅ 1107924407</p>
<p>❔:  ✅ В поток ввода можно подавать не только текст, но и любые данные</p>
<p>❔:  ✅ Можно соединить поток вывода одной программы с потоком ввода другой<br>
       ✅ При запуске в эмуляторе терминала вывод по-умолчанию осуществляется через эмулятор терминала на экран<br>
       ✅ read_int считывает число со стандартного потока ввода, поэтому если в него направить файл, то можно считать число из файла</p>
       
       
<h4 id="1.5">1.5 Глобальные и локальные переменные</h4>

<p>❔:  ✅ a = 20 b = 20</p>
<p>❔:  ✅ a = 10 b = 10</p>
<p>❔:  ✅ a = 40 b = 10 c = 30</p>
<pre>int main() {
  int input1 = read_int(); // читаем первое число
  int input2 = read_int(); // читаем второе число<br>

  printf("%d", input1 + input2); // печатаем сумму

  return 0;
}</pre>
<pre>int discriminant(int a, int b, int c) { return b*b-4*a*c; }

int root_count(int d) { return (d > 0) - (d < 0) + 1; }

int main() {
    int a = read_int(); int b = read_int(); int c = read_int();
    printf ("%d", root_count(discriminant(a, b, c)));
    return 0;
}</pre>


<h4 id="1.6">1.6 Глобальные и локальные переменные</h4>
<pre>int main() {
    int i = read_int(); 
    if(i > 10) printf("No");
    while(i <= 10) {
        printf("%d ", i++);
    }
    return 0;
}</pre>
<pre>int is_square(int n) {
    int i = 0;
    while (i * i < n) i++;
    return i * i == n;
}</pre>

<pre>
int main()
{
    for (int i = 1; i <= 100; i++) {
        printf("%d: ", i);
        for (int j = 2; j <= i; j++) {
            if (!(i % j)) { printf("%d ", j); }
        }
        puts("");
    }

    return 0;
}
</pre>

<pre>int is_prime(int n) {
    for (int i = 2; i < n; i++) {
        if (n % i == 0) return 0;
    }
    return n > 1;
}</pre>

<h4 id="1.7">1.7 Глобальные и локальные переменные</h4>
<p>❔:  ✅ x == 10<br>
       ✅ &x == 1016<br>
       ✅ &p == 2056<br>
       ✅ p == 1016<br>
       ✅ *p == 10</p>
<pre>void swap(int* a, int* b)
{
    int c = *b;
    *b = *a;
    *a = c;
}</pre>
<pre>void normalize(int *n) {
    for (; *n % 2 == 0 && *n > 0; *n /= 2);
}</pre>
<pre>
void factorize( int n, int* a, int* b )
{
    *a = 1;
    *b = n;
    
    for ( int i=2; i <= n/2; i = i + 1 ) {
        if ( n % i == 0 ) {
            *a = i;
            *b = n / i;
            return;
        }
    }
}
</pre>
<pre>void swap( int* a, int* b) {
    int c = *a;
    *a = *b;
    *b = c;
}

void array_reverse(int* array, int size) {
    for (int i = 0; i < size/2; i++) 
       swap( array + i, array + size - 1 - i);
}

void array_reverse_ptr(int* array, int* limit) {
    array_reverse( array, limit - array );
}</pre>
<pre>void array_fib(int* array, int* limit) {
    for (int i = 0; i < limit - array; i++) {
        if (i < 2) array[i] = 1;
        else array[i] = array[i - 2] + array[i - 1];
    }
}</pre>
<p>❔:  ✅ &p == 2056<br>
       ✅ &pp == 8000<br>
       ✅ pp == 2056<br>
       ✅ *pp == 1016<br>
       ✅ **pp == 10<br>
       ✅ pp[0] == 1016<br>
       ✅ pp[0][0] == 10<br>
       ✅ *pp[0] == 10</p>

<pre>int array_contains(int* array, int* limit, int** position) {
    for (*position = array; *position < limit; ++(*position))
        if (predicate(**position))
            return 1;
    return 0;
}</pre>
<pre>int is_whitespace(char c) { return c == ' ' || c == '\t' || c == '\n' || c == '\0'; }

int string_count(char* str) {
    int count = 0;
    while (str[count] != '\0') { count++; }
    return count;
}

int string_words(char* str) {
    int count = 0;
    for (int i = 0; i < string_count(str); i++) {
        if (!is_whitespace(str[i]) && is_whitespace(str[i+1])) { count++; }
    }
    return count;
}</pre>

<h4 id="1.8">1.8 Структура кода</h4>
<pre>void sum(int*, int*, int);</pre>

<pre>int stack_push(int);
int stack_pop(int*);</pre>

<pre>#ifndef ARITH_H
#define ARITH_H
int sum(int*, int);
#endif</pre>

<h3 id="2">2. Типы</h3>
<h4 id="2.1">2.1 Структура кода</h4>
<p>❔:  ✅ Да, такой компилятор соответствует стандарту языка</p>
<pre>// Определите массив в котором будут 8*1024*1024 чисел
// Массив не должен занимать больше 40 МБ памяти

uint32_t data[8*1024*1024] = {0};

// Определите функцию count_gt
// Она должна вернуть количество чисел в data, которые больше LIMIT
// LIMIT это определение препроцессора, оно вам уже доступно
// скрытый от вас код заполнит массив data числами и проверит правильность
// вашей функции
size_t count_gt(uint32_t * array, size_t size) {
    size_t count = 0;
    for (size_t i = 0; i != size; i++) {
        if (array[i] > LIMIT)
            count++;
    }
    return count;
}</pre>
<pre>size_t count_zeroes(const void* data, size_t sz ) {
    size_t answer = 0;
    for (int8_t* p = (int8_t*)data; p < (int8_t*)data+sz; p++) {
        answer += !*p;
    }
    return answer;
}</pre>

<h4 id="2.2">2.2 Интерлюдия. Динамическое выделение памяти</h4>
<p>❔:  ✅ 0<br>
       ✅ -1<br>
       ✅ 1024</p>
<p>❔:  ✅ 0<br>
       ✅ -1<br>
       ✅ 1024<br>
       ✅ ошибка</p>
<pre>// заполнить уже выделенный массив array размера size числами
void array_int_fill( int64_t* array, size_t size )
{
    for (size_t i = 0; i < size; i++, array++) {
        scanf("%" SCNd64 "", array);
    }
}

// Считать размер массива в *size, выделить память под массив и заполнить его числами.
int64_t* array_int_read( size_t* size )
{
    size_t s;
    scanf("%zu", &s);
    int64_t *array = (int64_t*)malloc(s * sizeof (int64_t));
    array_int_fill(array, s);
    *size = s;
    return array;
}</pre>

<pre>int64_t* array_int_min( int64_t* array, size_t size )
{
    int64_t min = 0;
    for (; size; size--)
        if (array[size - 1] < array[min]) min = size - 1;
    return array + min;
}</pre>

<pre>// эти функции вы уже реализовали на предыдущих шагах
int64_t* array_int_read( size_t* size );
int64_t* array_int_min( int64_t* array, size_t size); 

// Выводит None если x == NULL, иначе число, на которое указывает x.
void intptr_print( int64_t* x ) {
    x == NULL? printf("None"):printf("%" PRId64,*x);
  }

void perform() {
    size_t size = 0;
    int64_t* array = array_int_read(&size);
    intptr_print(array_int_min(array, size));
    free(array);
  }</pre>
  
<pre>// Вам доступны эти функции из прошлых заданий
size_t read_size();
void array_int_fill( int64_t* array, size_t size );
int64_t* array_int_read( size_t* size );

int64_t** marray_read( size_t* rows, size_t** sizes ) {
    size_t i;
    int64_t** marray;
    *rows = read_size();
    *sizes = malloc(*rows * sizeof(size_t));
    marray = malloc(*rows * sizeof(int64_t*));
    for (i = 0; i < *rows; i++) {
        marray[i] = array_int_read(&((*sizes)[i]));
    }
    return marray;
}

void marray_print(int64_t** marray, size_t* sizes, size_t rows) {
    for( size_t i = 0; i < rows; i = i + 1 ) {
        array_int_print( marray[i], sizes[i] );
        print_newline();
    }
}</pre>

<pre>void marray_free( int64_t** marray, size_t rows ) {
  for(size_t i = 0; i < rows; i++) free(marray[i]);
  free(marray);
}</pre>

<pre>// Вам доступны следующие функции:
size_t read_size();
int64_t* array_int_min( int64_t* array, size_t size );
int64_t** marray_read( size_t* rows, size_t* sizes[] );
void marray_free( int64_t** marray, size_t rows );
void marray_print(int64_t** marray, size_t* sizes, size_t rows);


// Указатель на минимальное из двух чисел.
// если хотя бы одно число NULL, то возвращать второе
// если оба числа NULL результат NULL
int64_t* int64_ptr_min(int64_t* x, int64_t* y) {
    if (x == NULL) return y;
    if (y == NULL) return x;
    if (*x > *y) return y;
    return x;
}

// Вернуть адрес минимального элемента массива массивов
int64_t* marray_int_min( int64_t** marray, size_t* sizes, size_t rows ) {
    int64_t* result = NULL;
    for (size_t i = 0; i < rows; i++) {
        for (size_t j = 0; j < sizes[i]; j++) {
            result = int64_ptr_min(result, &marray[i][j]);
        }
    }
    return result;
}

// Вычесть m изо всех элементов массива
void marray_normalize( int64_t** marray, size_t sizes[], size_t rows, int64_t m ) {
    for (size_t i = 0; i < rows; i++) {
        for (size_t j = 0; j < sizes[i]; j++) {
            marray[i][j] = marray[i][j] - m;
        }
    }
}

// Прочитать, найти минимум и нормализовать массив, вывести результат
void perform() {
    size_t rows = 0;
    size_t* sizes;
    int64_t** marray = NULL;
    marray = marray_read(&rows, &sizes );
    int64_t* min = marray_int_min( marray, sizes, rows );
    if (min != NULL) marray_normalize( marray, sizes, rows, *min );
    marray_print(marray, sizes, rows);
    marray_free( marray, rows );
    free(sizes);
}</pre>

<h4 id="2.3">2.3 Структуры</h4>
<p>❔:  ✅ Поля структуры расположены в памяти последовательно, возможны пропуски между ними</p>
<p>❔:  ✅ Можно создать массив из таких структур</p>
<pre>void maybe_int64_print(struct maybe_int64 i) 
{
    if (i.valid != true)
        printf("None");
    else
        printf("Some %" PRId64, i.value);
}

struct maybe_int64 maybe_int64_min(struct maybe_int64 a, struct maybe_int64 b) 
{
    if (!a.valid && !b.valid)
        return (none_int64);
    if (!a.valid || (b.valid && a.value > b.value))
        return (b);
    return (a);
}</pre>

<pre>// Чтенине размера массива или количество строк (массивов)
size_t read_size(){ 
    size_t sz = 0; 
    scanf("%zu", &sz); 
    return sz;
}

// Структура описывающая массив
struct array_int {
    size_t size;
    int64_t* data;
};

// Заполнение существующего массива значениями
void array_int_fill( int64_t* array, size_t sz ) {
  for( size_t i = 0; i < sz; i = i + 1 ) {
    array[i] = read_int64();
  }
}

// Создание массива. Размер считывается из ввода, 
// возвращается структура размер + адрес начала массива
struct array_int array_int_read() {
  const size_t size = read_size();
  if (size > 0) {
    int64_t* array = malloc( sizeof(int64_t) * size);
    array_int_fill( array, size );
    return (struct array_int) { .data = array, .size = size };
  }
  else return (struct array_int) {0};
}

// возвращает ошибку если индекс за пределами массива
struct maybe_int64 array_int_get( struct array_int a, size_t i ) {
    if(i < a.size) return some_int64(a.data[i]);
    return none_int64;
}

// возвращает false если индекс за пределами массива
bool array_int_set( struct array_int a, size_t i, int64_t value ) {
    if(i < a.size) a.data[i] = value;
    return i < a.size;
}

// Печать массива
void array_int_print( struct array_int array ) {
  for (size_t i = 0; i < array.size; i++) {
    printf("%" PRId64 " " , array_int_get( array, i).value);
  }
}

// Поиск наименьшего значения в массиве
struct maybe_int64 array_int_min( struct array_int array ) {
    if(!array.size) return none_int64;
    size_t min_index = 0;
    for(size_t i = 0; i < array.size; i++){
        if(array_int_get(array, min_index).value > array_int_get(array, i).value)
            min_index = i;
    }
    return (struct maybe_int64) {array_int_get(array, min_index).value, true};
}

// Освобождение выделенной под массив памяти
void array_int_free( struct array_int a ) { 
    if ( a.size > 0 ) {
        free(a.data); 
        a.size = 0;
    } 
}</pre>
<pre>/* Вы можете пользоваться этими функциями из предыдущих заданий */
size_t read_size() { size_t i; scanf("%zu", &i); return i; }
void array_int_fill( int64_t* array, size_t sz );

struct array_int array_int_read();
struct maybe_int64 array_int_get( struct array_int a, size_t i );
bool array_int_set( struct array_int a, size_t i, int64_t value );
void array_int_print( struct array_int array );
struct maybe_int64 array_int_min( struct array_int array );
void array_int_free( struct array_int a );

void array_int_normalize( struct array_int array, int64_t m ) {
  for (size_t i = 0; i < array.size; i = i + 1) {
    array.data[i] = array.data[i] - m;
  }
}

/*  ---- maybe int[] ---- */

struct maybe_array_int {
  struct array_int value;
  bool valid;
};

//struct array_int {
//  int64_t* data;
//  size_t size;
//};

struct maybe_array_int some_array_int(struct array_int array) {
  return (struct maybe_array_int) { array, true };
}
const struct maybe_array_int none_array_int = { {NULL, 0}, false };

/*  ---- int[][] ---- */

struct array_array_int {
  struct array_int* data;
  size_t size;
};

/*  --- строки ---  */

struct maybe_array_int array_array_int_get_row( struct array_array_int a, size_t i ) {
  if ( 0 <= i && i < a.size ) { return some_array_int( a.data[i] ); }
  else { return none_array_int; }
}

bool array_array_int_set_row( struct array_array_int a, size_t i, struct array_int value ) {
  if (0 <= i && i < a.size) {
    a.data[i] = value;
    return true;
  }
  else { return false; }
}

/*  --- get/set ---  */

struct maybe_int64 array_array_int_get( struct array_array_int a, size_t i, size_t j ) {
  struct maybe_int64 result;
  if (i < a.size && j < a.data[i].size) {
    result.value = a.data[i].data[j];
    result.valid = true;
  }
  else result.valid = false;
  return result;
}

bool array_array_int_set( struct array_array_int a, size_t i, size_t j, int64_t value ) {
  if (i < a.size && j < a.data[i].size) {
    a.data[i].data[j] = value;
    return true;
  } else {
    return false;
  }
}

/*  --- read/print ---  */

struct array_array_int array_array_int_read() {
    const size_t size = read_size();
    struct array_array_int array_array;    
    array_array.data = malloc( sizeof(struct array_int) * size);
    for (size_t i=0; i<size; i++) {
        array_array.data[i] = array_int_read();  
    }
    array_array.size = size;
    return array_array;
}

void array_array_int_print( struct array_array_int array) {
    for (size_t i=0; i< array.size; i++) {
        for (size_t j=0; j< array.data[i].size; j++)
            printf("%" PRId64 " ", array.data[i].data[j]);
        printf("\n");   
    }
}

/*  --- min/normalize ---  */

// найти минимальный элемент в массиве массивов
struct maybe_int64 array_array_int_min( struct array_array_int array ) {
  struct maybe_int64 result;
  result.valid = false;
  for (size_t i=0; i < array.size; i++)
    for (size_t j=0; j < array.data[i].size; j++) {
      if (!result.valid && array_array_int_get(array, i, j).valid) {
        result.value = array.data[i].data[j];
        result.valid = true;
      }
      if (result.valid && result.value > array.data[i].data[j])
        result.value = array.data[i].data[j];
    }
  return result;
}

// вычесть из всех элементов массива массивов число m
void array_array_int_normalize( struct array_array_int array, int64_t m) {
  for (size_t i = 0; i < array.size; i = i + 1) {
    const struct maybe_array_int cur_row = array_array_int_get_row( array, i );
    if (cur_row.valid) {
         array_int_normalize( cur_row.value, m );
    }
  }
}

void array_array_int_free( struct array_array_int array ) {
  for (size_t i=0; i<array.size; i++)
    if (array.data[i].size>0) free(array.data[i].data);
  free(array.data);
}</pre>

<pre>
struct stack {
  size_t count;
  struct array_int data;
};

// Количество элементов в стеке
size_t stack_count( const struct stack* s ) {
    return s->count;
}

// Создаем и деинициализируем стек
struct stack stack_create( size_t size ) {
    return (struct stack) { .count = 0, .data = array_int_create(size) };
}
void stack_destroy( struct stack* s ) {
    array_int_free(&(s->data));
}

// Стек полный
bool stack_is_full( const struct stack * s) {
    return s->count == s->data.size;
}
// Стек пустой
bool stack_is_empty( const struct stack * s) {
    return !(s->count);
}

// Поместить значение в стек
bool stack_push( struct stack* s, int64_t value ) {
    return array_int_set(s->data, s->count++, value);
}

// Вынуть значение с вершины стека. Может вернуть none_int64
struct maybe_int64
stack_pop( struct stack* s ) {
    if (stack_is_empty(s)) {
        return none_int64;
    }
    return array_int_get(s->data, --(s->count));
}

void stack_print( const struct stack* s ) {
  for (size_t i = 0; i < stack_count( s ); i = i + 1 ) {
    print_int64( array_int_get( s->data, i).value );
    printf(" ");
  }
}</pre>


<h4 id="2.4">2.4 Связный список</h4>

<pre>struct list {
  int64_t value;
  struct list* next;
};

struct list* node_create( int64_t value ) {
    struct list* list = malloc( sizeof *list );
    list -> value = value;
    return list;
}</pre>

<pre>struct list* node_create( int64_t value );

void list_add_front( struct list** old, int64_t value ) {
    struct list* link = node_create(value);
    link -> next = *old;
    *old = link;
}</pre>

<pre>size_t list_length(const struct list* l) 
{
    if (l == NULL){
        return 0;
    }
    return 1 + list_length(l->next);
}</pre>

<pre>void list_destroy( struct list* list ) {
  if (list) {
    list_destroy(list->next);
    free(list);
  }
}</pre>

<pre>struct list* list_last( struct list * list ) {
    while (list && list->next) {
		list = list -> next;
	}
	return list;
}</pre>

<pre>void list_add_back( struct list** old, int64_t value ) {
    if (*old == NULL){
        *old = node_create(value);
        return;
    }
    list_last(*old)->next=node_create(value);
}</pre>
<pre>int64_t list_sum( const struct list* list ) {
    int64_t sum = 0;
    if(list != NULL){
    while(list -> next != NULL){
        sum += list -> value;
        list = list -> next;
    }
    sum += list -> value;
    }
    return sum;
}</pre>
<pre>struct maybe_int64 list_at(  const struct list* list, size_t idx ) {
	while (list && idx--) { list = list->next; }
    
    return list 
        ? some_int64(list->value) 
        : none_int64;
}</pre>
<pre>struct list* list_reverse( struct list const * list ) {
  struct list* new = NULL;
  for (struct list const* current = list; current ; current = current -> next ) {
    list_add_front( &new, current-> value );
  }
  return new;
}</pre>
<pre>struct maybe_int64 maybe_read_int64() {
    struct maybe_int64 read;
    read.valid = (scanf("%" SCNd64, &read.value) == 1);
    return read;
}</pre>
<pre>struct list* list_read() {
  struct list* list = NULL;
  struct maybe_int64 t = maybe_read_int64();
  if (t.valid) {
    list = node_create(t.value);
    list->next = list_read();
  }
  return list;
}</pre>

<h4 id="2.5">2.5 Объединения и перечисления</h4>
<p>❔:  ✅ 64</p>

<pre>enum either_type { ET_INT, ET_STRING };

struct either_int_string {
  enum either_type type;
  union {
    char* as_string;
    int64_t as_int;
  };
};


// Создание экземпляров из строки или из числа
// Всегда передаётся строка, выделенная в куче
struct either_int_string either_from_string(char* s) {
    return (struct either_int_string){.type = ET_STRING, .as_string = s};
}
struct either_int_string either_from_int(int64_t i) {
    return (struct either_int_string){.type = ET_INT, .as_int = i};
}

// очистить память под строку (если строка)
void either_int_string_destroy(struct either_int_string e) {
    if(e.type == ET_STRING)
        free(e.as_string);
}

// конструкция switch используется для ветвления по значению числа,
// например, перечисления.
// Для строк и других типов данных использоваться не может
// Каждая ветка должна завершаться break
void print(struct either_int_string e) {
  switch (e.type) {
  case ET_INT: {
       printf("Int %" PRId64, e.as_int);
       break;
  }
  case ET_STRING: {
       printf("String %s", e.as_string);  
       break;
  }
  // Ветка по-умолчанию, если e.type не равен ни ET_INT, ни ET_STRING
  default: {
      break;
  }
  }
}</pre>

<pre>struct heap_string {
  char* addr;
};

// скопировать в кучу
struct heap_string halloc( const char* s ) {
    size_t count = 0;
    while (s[count++]);
    char* copied = malloc(sizeof(char)*count);
    for (size_t i = 0; i < count; i++) {
        copied[i] = s[i];
    }
    return (struct heap_string) { .addr = copied };
}

// освободить память
void heap_string_free( struct heap_string h ) {
    free(h.addr);
}</pre>

<h4 id="2.6">2.6 Функции</h4>

<pre>typedef char ftype(const float*, const float*);</pre>

<pre>// Мы хотим, чтобы в структуре user хранились ссылки только на строчки из кучи.
typedef struct { char* addr; } string_heap ;

/*  Тип для идентификаторов пользователей
    и его спецификаторы ввода и вывода для printf */
typedef uint64_t uid;
#define PRI_uid PRIu64
#define SCN_uid SCNu64

enum city {C_SARATOV, C_MOSCOW, C_PARIS, C_LOS_ANGELES, C_OTHER};

/*  Массив, где элементам перечисления сопоставляются их текстовые представления */
const char* city_string[] = {
  [C_SARATOV] = "Saratov",
  [C_MOSCOW] = "Moscow",
  [C_PARIS] = "Paris",
  [C_LOS_ANGELES] = "Los Angeles",
  [C_OTHER] = "Other"
};


struct user {
  const uid id;
  const string_heap name;
  enum city city;
};

void user_qsort(struct user users[], size_t size, int (*f)(const struct user*, const struct user*))
{
    int (*fvoid)(const void*, const void*) = (int (*)(const void*, const void*))(f);
    qsort(users, size, sizeof(struct user), fvoid);
}

/* Сортировать массив пользователей по полю uid по возрастанию */
int uid_compare(const struct user* x, const struct user* y) 
{
    if (x->id > y->id)
    {
        return 1;
    }
    if (x->id < y->id)
    {
        return -1;
    }
    return 0;
}

void users_sort_uid(struct user users[], size_t sz)
{
    user_qsort(users, sz, &uid_compare);
}

/* Сортировать массив пользователей по полю name */
/* Порядок строк лексикографический; можно использовать компаратор 
   строк -- стандартную функцию strcmp */
int string_heap_compare(const struct user* x, const struct user* y) 
{
    return strcmp(x->name.addr, y->name.addr);
}

void users_sort_name(struct user users[], size_t sz) 
{
    user_qsort(users, sz, &string_heap_compare);
}

/* Сортировать массив по _текстовому представлению_ города */
int enum_city_compare(const struct user* x, const struct user* y) 
{
    return strcmp(city_string[x->city], city_string[y->city]);
}

void users_sort_city(struct user users[], size_t sz) 
{
    user_qsort(users, sz, &enum_city_compare);
}</pre>

<pre>enum move_dir { MD_UP, MD_RIGHT, MD_DOWN, MD_LEFT, MD_NONE };

typedef void move_callback(enum move_dir);

struct list_callback{
    move_callback* function;
    struct list_callback * next;
};

struct robot {
    const char* name;
    struct list_callback* head;
};

struct list_callback* struct_list_callback_get_last(struct list_callback* head){
    if (head == NULL){
        return NULL;
    }
    struct list_callback* link = head;
    
    while(link -> next != NULL){
        link = link -> next;
    }
    return link;
}

struct list_callback* struct_list_callback_new(move_callback new_cb){
    struct list_callback* list = malloc(sizeof(struct list_callback));
    list -> function = new_cb;
    list -> next = NULL;
    
    return list;
}

void struct_list_callback_clear(struct list_callback** adr_head){
    struct list_callback* link = *adr_head;
    
    while(link != NULL){
        struct list_callback* next_link = link -> next;
        free(link);
        link = next_link;
    }
    
   *adr_head = NULL;
}

void struct_list_callback_call_all(struct list_callback* head, enum move_dir dir){
    struct list_callback* link = head;
    
    while(link != NULL){
        (link -> function)(dir);
        link = link -> next;
    }
    
}

void register_callback(struct robot* robot, move_callback new_cb) {
    struct list_callback* last = struct_list_callback_get_last(robot -> head);
    if (last == NULL){
        robot -> head = struct_list_callback_new(new_cb);
    }
    else{ 
        last -> next = struct_list_callback_new(new_cb);
    }
}

void unregister_all_callbacks(struct robot* robot) {
    struct_list_callback_clear(&(robot -> head));
}

void move(struct robot* robot, enum move_dir dir) {
    struct_list_callback_call_all(robot -> head, dir);
}</pre>


<h4 id="2.7">2.7 Функции высшего порядка</h4>

<pre>void print_int64(int64_t i);

/* Запустить функцию f на каждом элементе списка  */
void list_foreach(const struct list* l, void (f)(int64_t)) {
    while(l != NULL){
        f(l->value);
        l = l->next;
    }
}

/* Вывести список с помощью foreach и дополнительной функции */
void list_print(const struct list* l) { 
    list_foreach(l, print_int64_space);
}</pre>

<pre>/* Изменить каждый элемент списка с помощью функции f  */
void list_map_mut(struct list* l, int64_t (f) (int64_t))  {
    while(l != NULL){
        l->value = f(l->value);
        l = l->next;
    }
}

static int64_t triple( int64_t x ) { return x * 3; }

/* Используя list_map_mut умножьте все элементы списка на 3 */
void list_triple(struct list* l ) { 
    list_map_mut(l, triple);
}</pre>

<pre>/* Вы можете пользоваться следующими функциями */
void print_int64(int64_t i);
struct list* node_create( int64_t value );



/*  Создать новый список, в котором каждый элемент получен из соответствующего
    элемента списка l путём применения функции f */
struct list* list_map( struct list const* l, int64_t (f) (int64_t))  {
    struct list* new_list = NULL;
    struct list** cur = &new_list;
    
    while(l) {
        *cur = node_create( f(l->value) );
        cur = &(*cur)->next;
        l = l->next;
    }
    
    return new_list;
}

int64_t id(int64_t i) {
    return i;
}

struct list* list_copy( struct list const* l ) {
    return list_map(l, id);
}

typedef int64_t (my_mapper) (int64_t);
struct list* list_abs( struct list const* l ) {
    return list_map(l, (my_mapper*) abs);
}</pre>

<pre>/* Вы можете пользоваться этими функциями */
void print_int64(int64_t i);
struct list* node_create( int64_t value );
void list_destroy( struct list* list );

static int64_t sum( int64_t x, int64_t y) { return x + y; }

typedef int64_t folding(int64_t, int64_t);

int64_t list_fold(const struct list* l, int64_t init, folding f) {
    int64_t result = init;
    while (l) {
        result = f(result, l->value);
        l = l->next;
    }
    return result;
}

int64_t list_sum(const struct list* l) {
    return list_fold(l, 0, sum);
}</pre>

<pre>void print_int64(int64_t i);

struct list* node_create( int64_t value );
void list_destroy( struct list* list );


struct list* create_node(int64_t value, struct list* next) {
    struct list* list = malloc(sizeof(struct list));
    list->value = value;
    list->next  = next;
    return list;
}

/*  Сгенерировать список длины sz с помощью значения init и функции f
 Результат: init, f(init), f(f(init)), ... */
struct list* list_iterate( int64_t init, size_t sz, int64_t(f)(int64_t)) {
    if (sz == 0) return NULL;
    return create_node(init, list_iterate(f(init), --sz, f));
}</pre>




<h4 id="3">3. Структура кода</h4>



<h4 id="3.1">3.1 Декларативность. Стёк 1.0</h4>
<p>❔:  ✅ 42</p>
<p>❔:  ✅ 80 1</p>
<pre>const union ins program[] = {
    {BC_IREAD},
    {.as_arg64 = {BC_PUSH, .arg = 10}},
    {BC_ISUB},
    {.as_arg64 = {BC_PUSH, .arg = 2}},
    {BC_IDIV},
    {BC_IPRINT},
    {BC_STOP}
};</pre>
<p>❔:  ✅ 1</p>
<p>❔:  ✅ 3</p>
<pre>/* Описание инструкций (см. предыдущий шаг) */
enum opcode { BC_PUSH, BC_IPRINT, BC_IREAD, BC_IADD, BC_STOP };

struct bc_noarg {
  enum opcode opcode;
};
struct bc_arg64 {
  enum opcode opcode;
  int64_t arg;
};
union ins {
  enum opcode opcode;
  struct bc_arg64 as_arg64;
  struct bc_noarg as_noarg;
};

/* ------------------------ */

struct vm_state {
  const union ins *ip;
  struct stack data_stack;
};

/* Начальная вместимость стека задаётся определением STACK_CAPACITY */
struct vm_state state_create(const union ins *ip) {
  return (struct vm_state){.ip = ip,
                           .data_stack = stack_create(STACK_CAPACITY)};
}

// Как правильно деинициализировать состояние, освободить все ресурсы?
void state_destroy(struct vm_state *state) {
    stack_destroy(&state->data_stack);
}


/* Вы можете использовать эти функции: */
void print_int64(int64_t);
struct maybe_int64 maybe_read_int64();

struct stack stack_create(size_t size);
void stack_destroy(struct stack *s);
bool stack_push(struct stack *s, int64_t value);
struct maybe_int64 stack_pop(struct stack *s);

/* Опишите цикл интерпретации с выборкой и выполнением команд (пока не выполним STOP) */
void interpret(struct vm_state *state) {
    const union ins* cur = state->ip;
    while (cur->opcode != BC_STOP) {
        switch (cur->opcode) {
            case BC_PUSH: {
                stack_push(&state->data_stack, cur->as_arg64.arg);
                cur++;
                break;
            }
            case BC_IADD: {
                struct maybe_int64 a = stack_pop(&state->data_stack);
                struct maybe_int64 b = stack_pop(&state->data_stack);
                stack_push(&state->data_stack, a.value + b.value);
                cur++;
                break;
            }
            case BC_IPRINT: { 
                stack_print(state->data_stack);
                cur++;
                break;
            }
            case BC_IREAD: {
                struct maybe_int64 a = maybe_read_int64();
                stack_push(&state->data_stack, a.value);
                cur++;
                break;
            }
        }
    }
}

void interpret_program(const union ins *program) {
  struct vm_state state = state_create(program);
  interpret(&state);
  state_destroy(&state);
}</pre>

<pre>void interpret_push(struct vm_state* state) {
  stack_push(& state->data_stack, state->ip->as_arg64.arg);
}

void interpret_iread(struct vm_state* state ) {
  stack_push(&state->data_stack, maybe_read_int64().value);
}
void interpret_iadd(struct vm_state* state ) {
  stack_push(&state->data_stack, stack_pop(&state->data_stack).value+stack_pop(&state->data_stack).value);
}
void interpret_iprint(struct vm_state* state ) {
  print_int64(stack_pop(&state->data_stack).value);
}

/* Подсказка: можно выполнять программу пока ip != NULL,
    тогда чтобы её остановить достаточно обнулить ip */
void interpret_stop(struct vm_state* state ) {
  free(state->ip);
}

//void (*func_ptr[])(struct vm_state* state ) = {fun1, fun2, fun3};
typedef void (*interpret_ins)(struct vm_state* state );

interpret_ins interpreters[] = {
  [BC_PUSH] = interpret_push,
  [BC_IREAD] = interpret_iread, 
  [BC_IADD] = interpret_iadd,
  [BC_IPRINT] = interpret_iprint,
  [BC_STOP] = interpret_stop
};

void interpret(struct vm_state* state) {
    for (; state->ip->opcode != BC_STOP; state->ip++) {
      interpreters[state->ip->opcode](state);
    }
}</pre>


<pre>/* Вам уже доступны функции: */
bool stack_push( struct stack* s, int64_t value );
struct maybe_int64 stack_pop( struct stack* s );

struct maybe_int64 some_int64(int64_t i);
/*  const struct maybe_int64 none_int64; */


/*  Интерпретаторы команд */
void interpret_swap  ( struct vm_state* state )  {
    struct maybe_int64 x = stack_pop( &state -> data_stack );
    struct maybe_int64 y = stack_pop( &state -> data_stack );
    stack_push( &state -> data_stack, x.value );
    stack_push( &state -> data_stack, y.value );
}
void interpret_pop   ( struct vm_state* state )  {
    stack_pop( &state -> data_stack );
}

void interpret_dup   ( struct vm_state* state )  {
    struct maybe_int64 x = stack_pop( &state -> data_stack );
    stack_push( &state -> data_stack, x.value );
    stack_push( &state -> data_stack, x.value );
    
}

// Эти функции поднимают операции над числами на уровень стековых операций
// lift_unop применяет операцию к вершине стека;
void lift_unop( struct stack* s, int64_t (f)(int64_t)) { 
    stack_push( s, f( stack_pop( s ).value ) );
}

// lift_binop забирает из стека два аргумента,
// применяет к ним функцию от двух переменных и возвращает в стек результат
void lift_binop( struct stack* s, int64_t (f)(int64_t, int64_t)) {
    stack_push( s, f( stack_pop( s ).value, stack_pop( s ).value ) );
}


int64_t i64_add(int64_t a, int64_t b) { return a + b; }
int64_t i64_sub(int64_t a, int64_t b) { return a - b; }
int64_t i64_mul(int64_t a, int64_t b) { return a * b; }
int64_t i64_div(int64_t a, int64_t b) { return a / b; }
int64_t i64_cmp(int64_t a, int64_t b) { if (a > b) return 1; else if (a < b) return -1; return 0; }

int64_t i64_neg(int64_t a) { return -a; }

void interpret_iadd( struct vm_state* state ) { lift_binop(& state->data_stack, i64_add); }
void interpret_isub( struct vm_state* state ) { lift_binop(& state->data_stack, i64_sub); }
void interpret_imul( struct vm_state* state ) { lift_binop(& state->data_stack, i64_mul); }
void interpret_idiv( struct vm_state* state ) { lift_binop(& state->data_stack, i64_div); }
void interpret_icmp( struct vm_state* state ) { lift_binop(& state->data_stack, i64_cmp); }

void interpret_ineg( struct vm_state* state ) { lift_unop (& state->data_stack, i64_neg);  }</pre>

<pre>void interpret(struct vm_state* state, ins_interpreter * const (actions)[]) {
    for (; state->ip ;) {
        const union ins* ins = state->ip;
        const struct ins_descr* ins_descr = instructions + ins->opcode;
        /** решение */
        if (ins_descr->stack_min > state->data_stack.count) {
            printf("Stack underflow\n");
            return;
        }
        if (ins_descr->stack_delta > (int64_t)(state->data_stack.data.size - state->data_stack.count)) {
            printf("Stack overflow\n");
            return;
        }
        /** /решение */
        actions[ins->opcode](state);
        if (!ins_descr->affects_ip) { state->ip = state->ip + 1; }
    }
}</pre>





<h4 id="3.2">Модульность и абстракция</h4>
<p>❔:  ✅ cube<br>
       ✅ square</p>
<pre>
#ifndef STACK_H
#define STACK_H
#include <stdbool.h>
#include <stdint.h>
#include <stddef.h>

typedef struct {
  int64_t value;
} item;

#define STACK_ITEM_PRI PRId64

struct maybe_item {
  bool valid;
  item value;
};

static const struct maybe_item none_int = {0, {0}};

static struct maybe_item some_int(int64_t value) {
  return (struct maybe_item){true, {value}};
}

// Опишите непрозрачную структуру stack_int 
struct stack_int;



struct stack_int *stack_int_create();

void stack_int_destroy(struct stack_int *s);

bool stack_int_empty(struct stack_int const *s);
bool stack_int_full(struct stack_int const *s);

// Опишите функции:
// stack_int_push (первый аргумент структура, второй типа item, возвращает bool)
bool stack_int_push (struct stack_int *s, item i);
// stack_int_pop (аргумент структура, возвращает maybe_item) 
struct maybe_item stack_int_pop(struct stack_int *s);

void stack_int_print(struct stack_int const*);
#endif
</pre>

<pre>struct list {
    item value;
    struct list *next;
};

struct stack_int {
    struct list *items;
};

static struct list *c(item i, struct list *next) {
    struct list *result = malloc(sizeof(struct list));
    *result = (struct list){ i, next };
    return result;
}

static struct stack_int stack_int_default() {
    return (struct stack_int){.items = NULL};
}

struct stack_int *stack_int_create() {
    struct stack_int *const result = malloc(sizeof(struct stack_int));
    *result = stack_int_default();
    return result;
}

static void list_free( struct list* l ) {
    while (l) {
        struct list *cur = l;
        l = l->next;
        free(cur);
    }
}

void stack_int_destroy(struct stack_int *s) { // <==
    list_free(s->items);
    free(s);
}

bool stack_int_empty(struct stack_int const *s) { // <==
    return !s->items;
}

bool stack_int_full(struct stack_int const *s) { // <==
    return false;
}

bool stack_int_push(struct stack_int *s, item i) { // <==
    if (stack_int_full(s))
        return false;
    s->items = c(i, s->items);
    return true;
}

struct maybe_item stack_int_pop(struct stack_int *s) { // <==
    if (stack_int_empty(s))
        return none_int;
    struct list* p = s->items;
    struct maybe_item item = some_int(p->value.value);
    s->items = s->items->next;
    free(p);
    return item;
}

static void stack_int_foreach(struct stack_int const *s, void (f)(item)) {
    for (struct list *l = s->items; l; l = l->next)
        f(l->value);
}

static void print_int64_cr(item i) { printf("%" STACK_ITEM_PRI "\n", i.value); }

void stack_int_print(struct stack_int const *s) {
    stack_int_foreach(s, print_int64_cr);
}</pre>

<pre>static struct stack_interface {
    struct stack_int_interface {
        struct stack_int* (*create)();
        bool (*empty)(struct stack_int const*);
        bool (*full)(struct stack_int const*);
        void (*destroy)(struct stack_int*);
        bool (*push)(struct stack_int *, item);
        struct maybe_item (*pop)(struct stack_int *);
    } int64;
    
} const stack = {{stack_int_create, stack_int_empty, stack_int_full, stack_int_destroy, stack_int_push, stack_int_pop}};</pre>

<p>❔:  ✅ 200</p>
<pre>static bool divides(int64_t x, int64_t y) { return x % y == 0; }
static void print_int_space(int64_t x) {printf("%" PRId64 " ", x); }
static int64_t read_int() { int64_t x; scanf("%" PRId64, &x); return x; }

void print_divisors(int64_t n) {
  if (n > 0){ 
    for (int64_t i = 1; i <= n; i = i + 1){
      if (divides(n, i)){
        print_int_space(i); 
      }
    }
    printf("$");
  }
  else{ printf("No");}
}</pre>
