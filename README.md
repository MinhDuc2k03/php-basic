# PHP-Basic



## Introduction to Web Technology (Công nghệ Web)
Web Technology (Công nghệ Web) là một thuật ngữ chung đề cập đến nhiều ngôn ngữ và gói đa phương tiện được sử dụng kết hợp với nhau, để tạo ra các trang web. Mỗi công nghệ có chức năng riêng biệt và cần yêu cầu sử dụng kép ít nhất thêm một công nghệ khác. Do đó, có thể nói rằng tất cả các thành phần tạo nên một trang web phụ thuộc lẫn nhau.



## Introduction to HTML5 and CSS


### HTML5
HTML5 (Hypertext Markup Language 5) là ngôn ngữ lập trình được phát triển dựa trên nền tảng ngôn ngữ HTML. Thành phần quan nhất của nó là WWW (World Wide Web). HTML5 được sử dụng để thiết kế cấu trúc của website. HTML5 hỗ trợ tối đa cho các ứng dụng đa phương tiện trên website.

Đồng thời chúng vẫn có những cải tiến hỗ trợ và giúp cho website thân thiện hơn với người dùng, thiết bị, các chương trình máy tính, và các trình duyệt web,…


### CSS
CSS (Cascading Style Sheet) là ngôn ngữ tạo phong cách cho trang web. Nó dùng để tạo phong cách và định kiểu cho những yếu tố được viết dưới dạng ngôn ngữ đánh dấu như HTML. Nó có thể điều khiển định dạng của nhiều trang web cùng lúc để tiết kiệm công sức cho người viết web. Nó phân biệt cách hiển thị của trang web với nội dung chính của trang bằng cách điều khiển bố cục, màu sắc, và font chữ.


## PHP Introduction
PHP (Personal Home Page) là một dạng mã lệnh hoặc một chuỗi ngôn ngữ kịch bản được dùng để phát triển các ứng dụng web chạy trên máy chủ. Khi các lập trình viên PHP viết chương trình, chuỗi lệnh sẽ được xử lý trên server sau đó sinh ra mã HTML trên client. Dựa vào đó, các ứng dụng trên website sẽ hoạt động một cách dễ dàng.

 - Ưu điểm:
    - Dễ học và dễ sử dụng, có tính linh hoạt cao để giải quyết các vấn đề
    - Tương thích tốt với các trình duyệt web
    - Tối ưu tốc độ load web và xử lý dữ liệu
    - Cơ sở dữ liệu đa dạng
    - Khả năng bảo mật cao
    - Khả năng mở rộng

 - Nhược điểm
    - Chỉ sử dụng để làm web và các ứng dụng web mở rộng.
    - Hạn chế cấu trúc ngữ pháp



## PHP Syntax
Cú pháp cho PHP có thể đặt bất cứ đâu trong tệp.

Tập lệnh PHP bắt đầu bằng `<?php` và kết thúc bằng `?>`:

```php
<?php
    // Viết PHP trong đây
?>
```

Phần mở rộng tệp mặc định cho tệp PHP là ".php".

Tệp PHP thường chứa các thẻ HTML và một số mã tập lệnh PHP:

```php
<!DOCTYPE html>
<html>
<body>

<h1>Trang PHP</h1>

<?php
echo "Hello World!";
?>

</body>
</html>
```



## PHP Data Types
PHP hỗ trợ các kiểu dữ liệu sau:
 - String
 - Integer
 - Float (số dấu phẩy động, còn được gọi là số kép)
 - Boolean
 - Array
 - Object
 - NULL


### String (Chuỗi)
String là một chuỗi các ký tự, chẳng hạn như "Hello world!".

Một string có thể là bất kỳ văn bản nào bên trong dấu ngoặc kép. Bạn có thể sử dụng dấu ngoặc đơn hoặc dấu ngoặc kép:

```php
<?php
$x = "Hello world!";
$y = 'Hello world!';
?>
```


### Integer (Số nguyên)
Kiểu dữ liệu số nguyên là số **không** thập phân trong khoảng từ -2,147,483,648 đến 2,147,483,647.

Những quy tắc cho số nguyên:
 - Phải có ít nhất một chữ số.
 - Không được có dấu thập phân.
 - Có thể là số dương hoặc số âm
 - Có thể được chỉ định bằng: ký hiệu thập phân (cơ sở 10), thập lục phân (cơ sở 16), bát phân (cơ sở 8) hoặc ký hiệu nhị phân (cơ sở 2)

```php
<?php
$x = 5985;
$y = -892346;
$z = 0;
?>
```


### Float (số dấu phẩy động)
Số số dấu phẩy động là một số có dấu thập phân hoặc số ở dạng hàm mũ.

```php
<?php
$x = 10.365;
$y = -15.636;
?>
```


### Boolean
Boolean đại diện cho hai trạng thái có thể có: TRUE hoặc FALSE.

```php
<?php
$x = true;
$y = false;
?>
```

Booleans thường được sử dụng trong thử nghiệm có điều kiện.


### Array (Mảng)
Một mảng lưu trữ nhiều giá trị trong một biến duy nhất.

```php
<?php
$arrayA = array(
    "foo" => "bar",
    "bar" => "foo",
);

$arrayB = [
    "foo" => "bar",
    "bar" => "foo",
];
?>
```


### Object (Đối tượng)
Classes (lớp) và đối tượng là hai khía cạnh chính của **lập trình hướng đối tượng**.

Lớp là một mẫu cho các đối tượng và đối tượng là một thể hiện của một lớp.

Khi các đối tượng riêng lẻ được tạo, chúng kế thừa tất cả các thuộc tính và hành vi từ lớp, nhưng mỗi đối tượng sẽ có các giá trị thuộc tính khác nhau.

```php
class Car {
  public $color;
  public $model;
  public function __construct($color, $model) {
    $this->color = $color;
    $this->model = $model;
  }
  public function message() {
    return "My car is a " . $this->color . " " . $this->model . "!";
  }
}
```


### NULL (Vô giá trị)
Null là kiểu dữ liệu đặc biệt chỉ có thể có một giá trị: NULL.

Biến có kiểu dữ liệu NULL là biến không được gán giá trị.
```php
<?php
$x = null;
?>
```



## PHP Variables, Constants and Array


### Variables (Biến)
Biến là "thùng chứa" để lưu trữ thông tin.
```php
<?php
$x = 5;
$y = "John"
?>
```

Một biến có thể có tên ngắn (như `$x` và `$y`) hoặc tên mang tính mô tả hơn (`$age`, `$carname`, `$total_volume`).

Quy tắc cho các biến PHP:
 - Bắt đầu bằng dấu `$`, theo sau là tên biến
 - Tên biến phải bắt đầu bằng một chữ cái hoặc ký tự gạch dưới
 - Tên biến không thể bắt đầu bằng một số
 - Tên biến chỉ có thể chứa các ký tự chữ và số và dấu gạch dưới (A-z, 0-9 và _ )
 - Tên biến có phân biệt chữ hoa chữ thường (`$age` và `$AGE` là hai biến khác nhau)

**Ghi chú:** Tên biến PHP có phân biệt chữ hoa chữ thường.


### Constants (Hằng số)
Hằng số là mã định danh (tên) cho một giá trị đơn giản. Giá trị không thể thay đổi trong tập lệnh.

Tên hằng hợp lệ bắt đầu bằng một chữ cái hoặc dấu gạch dưới (không có dấu `$` trước tên hằng).

**Lưu ý:** Không giống như biến, hằng số tự động mang tính tổng thể trên toàn bộ tập lệnh.

Để tạo một hằng số, sử dụng `define(tên, giá trị)`.
```php
<?php
define("V1", "hello");  //hello có phân biệt chữ hoa
?>
```

Bạn cũng có thể tạo một hằng số bằng cách sử dụng từ khóa `const`:
```php
<?php
const x = "Hello";
?>
```


### Array (Mảng)
Mảng là một biến đặc biệt có thể chứa nhiều giá trị dưới một tên duy nhất và bạn có thể truy cập các giá trị đó bằng cách tham chiếu đến số hoặc tên chỉ mục.

Trong PHP có 3 loại mảng:
 - Mảng được lập chỉ mục - Mảng có chỉ mục bằng số
 - Mảng kết hợp - Mảng có khóa được đặt tên
 - Mảng đa chiều - Mảng chứa một hoặc nhiều mảng
```php
<?php
$arrayA = array("Apple", "Orange", "Banana");

$arrayB = array("brand"=>"Ikea", "model"=>"chair", "year"=>1964);

$arrayC = array (
  array("Volvo", 22, 18),
  array("BMW", 15, 13),
  array("Saab", 5, 2),
  array("Land Rover", 17, 15)
);
?>
```



## PHP Operators
| Operator | Tên                 | Syntax   | Operation                          |
|----------|---------------------|----------|------------------------------------|
| +        | Cộng                | $x + $y  | Phép tính cộng                     |
| -        | Trừ                 | $x - $y  | Phép tính trừ                      |
| *        | Nhân                | $x * $y  | Phép tính nhân                     |
| /        | Chia                | $x / $y  | Phép tính chia                     |
| **       | Lũy thừa            | $x ** $y | $x nâng lên thành lũy thừa $y      |
| %        | Mô đun              | $x % $y  | Phần còn lại của $x chia cho $y    |
| >        | Lớn hơn             | $x > $y  | $x phải lớn hơn $y                 |
| <        | Nhỏ hơn             | $x < $y  | $x phải lớn hơn $y                 |
| ==       | Bằng                | $x == $y | $x bằng $y                         |
| <=       | Nhỏ hơn hoặc bằng   | $x <= $y | $x nhỏ hơn hoặc bằng $y            |
| >=       | Lớn hơn hoặc bằng   | $x >= $y | $x lớn hơn hoặc bằng $y            |
| +=       | Cộng bằng           | $x += $y | $x += $y => $x = $x + $y           |
| -=       | Trừ bằng            | $x -= $y | $x -= $y => $x = $x - $y           |
| *=       | Nhân bằng           | $x `*= $y| $x *= $y => $x = $x `* $y          |
| /=       | Chia bằng           | $x /= $y | $x /= $y => $x = $x / $y           |
| %=       | Modulo bằng         | $x %= $y | $x %= $y => $x = $x % $y           |
| !        | Toán NOT (phủ định) | !($x)    | !(true || true) ≡ false            |
| &&       | Toán tử và          |($x && $y)| (true && true) ≡ true              |



## Control Structures



### if else statement (Câu lệnh if else)
Câu lệnh if else thực thi một số mã nếu điều kiện đúng và mã khác nếu điều kiện đó sai.
```php
<?php
if ($a > $b) {
  echo "a lớn hơn b";
  
} else {
  echo "a nhỏ hơn b";
}
?>
```


### else if statement
```php
<?php
if ($a > $b) {
  echo "a lớn hơn b";

} elseif ($a == $b) {
  echo "bằng b";
  
} else {
  echo "a nhỏ hơn b";
}
?>
```


### switch case
Sử dụng câu lệnh switch để chọn một trong nhiều khối mã sẽ được thực thi.
```php
<?php
$color = "red";

switch ($color) {
  case "red":
    echo "Your favorite color is red!";
    break;
  case "blue":
    "Your favorite color is blue!";
    break;
  case "green":
    echo "Your favorite color is green!";
    break;
  default:
    echo "Your favorite color is neither red, blue, nor green!";
}
?>
```

Đây là cách nó hoạt động:
 - Biểu thức được đánh giá một lần
 - Giá trị của biểu thức được so sánh với giá trị của từng trường hợp
 - If there is a match, the associated block of code is executed
 - Từ khóa `break` thoát ra khỏi khối `switch`
 - Khối mã `default` được thực thi nếu không khớp


### Loops (Vòng lặp)
Vòng lặp được sử dụng để thực thi lặp đi lặp lại cùng một khối mã, miễn là một điều kiện nhất định là đúng.


### while
Vòng lặp while thực thi một khối mã miễn là điều kiện đã chỉ định là đúng.
```php
<?php
$i = 1;

while ($i < 6) {
  echo $i;
  $i++;
}
?>
```

**Lưu ý:** Nhớ tăng $i, nếu không vòng lặp sẽ tiếp tục mãi mãi.


### do while
Vòng lặp do...while sẽ luôn thực thi khối mã ít nhất một lần, sau đó nó sẽ kiểm tra điều kiện và lặp lại vòng lặp trong khi điều kiện đã chỉ định là đúng.
```php
<?php
$i = 1;

do {
  echo $i;
  $i++;
} while ($i < 6);
?>
```


### for
Vòng lặp for được sử dụng khi bạn biết tập lệnh sẽ chạy bao nhiêu lần.
```php
<?php
for ($x = 0; $x <= 10; $x++) {
  echo "x bằng $x <br>";
}
?>
```


### foreach
Vòng lặp foreach lặp qua một khối mã cho từng phần tử trong một mảng hoặc từng thuộc tính trong một đối tượng.
```php
<?php
$colors = array("red", "green", "blue", "yellow");

foreach ($colors as $x) {
  echo "$x <br>";
}
?>
```


## String Functions
Các hàm xử lý chuỗi trong PHP hay dùng:


### strlen()
Trả về độ dài của một chuỗi.
```php
<?php
echo strlen("Hello world!");  //12
?>
```

### str_word_count()
Đếm số từ trong một chuỗi.
```php
<?php
echo str_word_count("Hello world!");  //2
?>
```


### strpos()
Tìm một văn bản cụ thể trong một chuỗi.
Nếu tìm thấy kết quả khớp, hàm sẽ trả về vị trí ký tự của kết quả khớp đầu tiên. Nếu không tìm thấy kết quả phù hợp thì nó sẽ trả về FALSE.
```php
<?php
echo strpos("Hello world!", "world"); //6
?>
```


### strtoupper()
Trả về chuỗi trong chữ hoa.
```php
<?php
$x = "Hello World!";
echo strtoupper($x);?>  //HELLO WORLD!
?>
```


### strtolower()
Trả về chuỗi trong chữ thường.
```php
<?php
$x = "Hello World!";
echo strtolower($x);?>  //hello world!
?>
```


### str_replace()
Thay thế một số ký tự bằng một số ký tự khác trong chuỗi.
```php
<?php
$x = "Hello World!";
echo str_replace("World", "Duc", $x); //Hello Duc!
?>
```


### trim()
Xóa mọi khoảng trắng ở đầu hoặc cuối chuỗi.



### explode()
Tách một chuỗi thành một mảng.
```php
<?php
$x = "Hello World!";
$y = explode(" ", $x);

//Sử dụng hàm print_r() để hiển thị kết quả:
print_r($y);   //Array ( [0] => Hello [1] => World! )
?> 
```


### substr()
Trả về một loạt ký tự.
```php
<?php
$x = "Hello World!";
echo substr($x, 6, 5);  //World
?> 
```

**Lưu ý:** Ký tự đầu tiên có chỉ số 0.


## Array Functions
array(*value1, value2, value3, etc.*): Tạo một mảng

array_change_key_case(*array, case*): Thay tất cả các khóa trong mảng thành chữ hoa

array_chunk(*array, size, preserve_key*): Chia một mảng thành hai phần

array_column(*array, column_key, index_key*): Trả về các giá trị từ một cột trong mảng đầu vào

array_keys(*array, value, strict*): Trả về một mảng chứa các khóa.

array_combine(*keys, values*): Tạo một mảng bằng cách sử dụng các phần tử từ một mảng "khóa" và một mảng "giá trị".

array_values(*array*): Trả về một mảng chứa tất cả các giá trị của một mảng.

array_push(*array, value1, value2, ...*): Chèn một hoặc nhiều phần tử vào cuối mảng.

sort(*array, sorttype*): Sắp xếp một mảng được lập chỉ mục theo thứ tự tăng dần.

rsort(*array, sorttype*): Sắp xếp một mảng được lập chỉ mục theo thứ tự giảm dần.

count(*array, mode*): Đếm phần tử trong mảng

và nhiều function hơn tại [đây](https://www.w3schools.com/php/func_array_keys.asp).



## File handling (Xử lý tệp)
Xử lý tệp là một phần quan trọng của bất kỳ ứng dụng web nào. Bạn thường cần mở và xử lý một tệp cho các tác vụ khác nhau.


### readfile()
Hàm readfile() đọc một tệp và ghi nó vào bộ đệm đầu ra.


### fopen()
Một phương pháp tốt hơn để mở tệp là sử dụng hàm fopen(). Hàm này cung cấp cho bạn nhiều tùy chọn hơn hàm readfile().

Hàm fopen() cũng được sử dụng để tạo một tập tin mới.


### fread()
Hàm fread() đọc từ một file đang mở bằng `fopen()`.


### fclose()
Hàm fclose() được sử dụng để đóng một file đang mở bằng `fopen()`.


### fgets()
Hàm fgets() được sử dụng để đọc **một dòng** từ một tệp.


### feof() (Check End-Of-File)
Hàm feof() kiểm tra xem đã đạt đến "cuối tập tin" (EOF) hay chưa.

The feof() function is useful for looping through data of unknown length.


### fgetc()
Hàm fgetc() được sử dụng để đọc **một ký tự** từ một tệp.


### fwrite()
Hàm fwrite() được sử dụng để ghi vào một tập tin.