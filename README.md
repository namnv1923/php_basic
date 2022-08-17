# PHP-Basic
## Introduction to web Technology(Giới thiệu về công nghệ web):
- Công nghệ Web đề cập đến các công cụ và kỹ thuật khác nhau được sử dụng trong quá trình giao tiếp giữa các loại thiết bị khác nhau qua internet. Trình duyệt web được sử dụng để truy cập các trang web. Trình duyệt web có thể được định nghĩa là các chương trình hiển thị văn bản, dữ liệu, hình ảnh, hoạt ảnh và video trên Internet. Các tài nguyên siêu liên kết trên World Wide Web có thể được truy cập bằng giao diện phần mềm do trình duyệt Web cung cấp.
### Công nghệ Web có thể được phân loại thành các phần sau:
- **World Wide Web (WWW):** World Wide Web dựa trên một số công nghệ khác nhau: Trình duyệt web, Ngôn ngữ đánh dấu siêu văn bản (HTML) và Giao thức truyền siêu văn bản (HTTP).
- **Web Browser(Trình duyệt web):** Trình duyệt web là một phần mềm ứng dụng để khám phá www (World Wide Web). Nó cung cấp giao diện giữa máy chủ và máy khách và yêu cầu máy chủ cung cấp các tài liệu và dịch vụ web.
- **Web Server(Máy chủ Web):** Máy chủ web là một chương trình xử lý các yêu cầu mạng của người dùng và phục vụ họ với các tệp tạo trang web. Việc trao đổi này diễn ra bằng cách sử dụng Giao thức truyền siêu văn bản (HTTP).
- **Web Pages(Trang Web):** Trang web là một tài liệu kỹ thuật số được liên kết với World Wide Web và bất kỳ ai được kết nối với internet có trình duyệt web đều có thể xem được.
- **Web Development(Phát triển Web):** Phát triển web đề cập đến việc xây dựng, tạo và duy trì các trang web. Nó bao gồm các khía cạnh như thiết kế web, xuất bản web, lập trình web và quản lý cơ sở dữ liệu. Đó là việc tạo ra một ứng dụng hoạt động trên internet, tức là các trang web.
## Introduction to HTML5 and CSS(Giới thiệu về HTML5 và CSS):
### HTML5
- **HTML** là viết tắt của Hyper Text Markup Language. Nó được sử dụng để thiết kế các trang web bằng ngôn ngữ đánh dấu. HTML là viết tắt của ngôn ngữ Siêu văn bản và Đánh dấu. Siêu văn bản xác định liên kết giữa các trang web. Ngôn ngữ đánh dấu được sử dụng để xác định tài liệu văn bản trong thẻ xác định cấu trúc của các trang web. HTML 5 là phiên bản thứ năm và hiện tại của HTML. Nó đã cải thiện đánh dấu có sẵn cho các tài liệu và đã giới thiệu các giao diện lập trình ứng dụng:application programming interfaces(API) và Mô hình Đối tượng Tài liệu:Document Object Model(DOM).
### CSS
- **C**ascading **S**tyle **S**heets, hay còn được gọi là **CSS**, CSS cho phép áp dụng cả kiểu(Style) cho các trang web ,bạn có thể làm cho trang web theo cách mình muốn như thay đổi màu phông chữ , khoảng cách và nhiều thứ khác.
## PHP Introduction
- Thuật ngữ PHP được viết tắt từ _Hypertext Preprocessor_ .PHP là một ngôn ngữ kịch bản(scripting languege) phía máy chủ đc thiết kế đặc biệt để phát triển web. PHP là một mã nguồn mở, được tải xuống và sử dingj miễn phí.
## PHP Syntax
- Một tập lệnh được thực thi trên máy chủ và dả về kết quả của HTML được ghi trở laiij trình duyệt, nó thường có các thẻ HTML và PHP.
## PHP Data Types
**Các biến có thể lưu trữ dữ liệu thuộc các kiểu khác nhau và các kiểu dữ liệu khác nhau có thể làm những việc khác nhau:**
- **String** : Trả về chuỗi.
  `
  $a = "chuỗi";
  `
- **Integer(int)** : Trả về số nguyên.
  `
  $a = 1;
  `
- **Float** : Trả về dạng số thập phân.
  `
  $a = 2.5;
  `
- **Boolen** : Trả về đúng hoặc sai.
  `
  $x = true;
  $y = false;
  `
- **Array** : Trả về mảng.
  `
  $cars = array("Volvo","BMW","Toyota");
  `
- **Object** : Trả về 1 đối tượng.
```
<?php
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

    $myCar = new Car("black", "Volvo");
    echo $myCar -> message();
    echo "<br>";
    $myCar = new Car("red", "Toyota");
    echo $myCar -> message();
?>
```
- **Null** : Trả về null(Không có giá trị nào đc gán cho nó).
  `
  $x = "Hello world!";
  $x = null;
  `
- **Resource** : Nó là việc lưu trữ một tham chiếu đến các hàm và tài nguyên bên ngoài PHP.
## PHP Variables, Constants and Array
### Variables
- Các biến(Variables) trong chương trình được sử dụng để lưu trữ một số giá hoặc dữ liệu nào đó.Các biến có thể lưu chuỗi,giá trị kí tự,địa chỉ bộ nhớ và giá trị số.
- Mọi biến được khai báo trong PHP phải bắt đầu bằng dấu đô la ($), theo sau là tên biến.
### Constants
- Hằng số(Constands) là số nhận dạng hoặc tên đơn giản có thể được gán bất kỳ giá trị cố định nào .Tương tự như một biến ngoại trừ việc chúng không bao giờ có thể thay đổi được kể cả trong quá trình thực thi.
### Array
- Mảng(Array) trong PHP là một kiểu cấu trúc dữ liệu cho phép ta lưu trữ nhiều phần tử của kiểu dữ liệu tương tự dưới một biến duy nhất.Một mảng được tạo bằng cách sử dụng một hàm `array()` trong PHP hoặc có thể dùng bằng cách khai báo biến `$a = ["a","b","c"]`.
## PHP Operators
- Các toán tử(Operators) được sử dụng để thực hiện các phép toán đơn giản như cộng ,trừ ,nhân ,...
### Kí hiệu
| Operator | Name        | Syntax      | Operation                           |
|:---------|:------------|:------------|:------------------------------------|
| +        | Cộng        | $x + $y     | Tính tổng phép tính                 |
| -        | Trừ         | $x - $y     | Trừ phép tính                       |
| *        | Nhân        | $x * $y     | Nhân phép tính                      |
| /        | Chia        | $x / $y     | Chia phép tính                      |
|**        | Lũy thừa    | $x ** $y    | $x được nâng lên thành lũy thừa $y  |
|**        | Mô đun      | $x % $y     | Phần còn lại của $x chia cho $y     |
## Control Structures
### if else statement
- Câu lệnh if / else thực thi một khối mã nếu một điều kiện được chỉ định là đúng. Nếu điều kiện sai, một khối mã khác có thể được thực thi.
### else if statement
- Câu lệnh if ... elseif ... else thực thi các mã khác nhau cho nhiều hơn hai điều kiện.
### switch case
- Câu lệnh switch được sử dụng để thực hiện các hành động khác nhau dựa trên các điều kiện khác nhau.
- Syntax
```
switch (n) {
  case label1:
  code to be executed if n=label1;
  break;
  case label2:
  code to be executed if n=label2;
  break;
  case label3:
  code to be executed if n=label3;
  break;
  ...
  default:
  code to be executed if n is different from all labels;
  }
```
## Loops
- Muốn một khối mã chạy đi chạy lại một số lần nhất định thay vì viết đi viết lại 1 đoạn mã giống nhau ta sử dụng vòng lặp.
- **Trong PHP có các loại vòng lặp:**
### while
- Vòng lặp while thực thi một khối mã miễn là điều kiện được chỉ định là đúng.
```angular2html
while (condition is true) {
  code to be executed;
}
```
- Example
```angular2html
<?php
$x = 1;

while($x <= 5) {
  echo "The number is: $x <br>";
  $x++;
}
?>
```
### do while
- Vòng lặp do while lặp qua khối mã ít nhất 1 lần, sau đó nó sẽ kiểm tra điều kiện và lặp lại vòng lặp trong khi điều kiện được chỉ định là đúng.
```angular2html
<?php
$x = 1;

do {
  echo "The number is: $x <br>";
  $x++;
} while ($x <= 5);
?>
```
### for
- Lặp qua khối mã số lần nhất định, sử dụng khi biết số lần khối mã sẽ chạy.
```angular2html
<?php
for ($x = 0; $x <= 10; $x++) {
  echo "The number is: $x <br>";
}
?>
```
### foreach
- Chỉ sử dụng trong mảng, lặp qua từng cặp khóa và giá trị trong mảng.
```angular2html
<?php
$colors = array("red", "green", "blue", "yellow");

foreach ($colors as $value) {
  echo "$value <br>";
}
?>
```
## String Functions
- **Để xử lý chuỗi trong PHP, cung cấp rất nhiều hàm có sẵn để làm việc với chuỗi.**
- **Một số hàm phổ biến hay sử dụng:**


1. Hàm strlen(): sử dụng để xem độ dài của chuỗi.
```angular2html
<?php
 $string = "PHP is a programming language.";
 $length = strlen($string);
 echo $length;
?>
Output: 30
```
2. Hàm str_replace: dùng để thay thế 1 số ký tự trong chuỗi bằng 1 số ký tự khác.
`
   str_replace(Search, Replace, Subject)
`
```angular2html
<?php
 $string = "Hello Troposal";
 $search = "Hello";
 $replace = "Hi";
 $newString = str_replace($search, $replace, $string);
 echo $newString;
?>
Output: Hi Troposal
```
3. Hàm strstr(): hiển thị phần chuỗi kể từ lần xuất hiện tìm kiếm đầu tiên đến cuối chuỗi.
4. Hàm strtolower():      biến chuỗi thành chữ thường.
5. Hàm strtouper():       biến chuỗi thành chữ hoa.
6. Hàm str_word_count():  đếm các từ có trong chuỗi.
7. Hàm strrev():          dùng để đảo ngược chuỗi.
8. Hàm strpos(): dùng để xác định vị trí ban đầu của 1 chuỗi trong chuỗi gốc.
9. Hàm ucwords(): chuyển đổi chữ cái đầu tiên của các từ thành chữ hoa.
10. Hàm ucfirst(): chuyển chữ cái đầu tiên của chuỗi thành hoa.
11. Hàm lcfirst(): chuyển chữ cái đầu tiên của chuỗi thành chữ thường.
12. Hàm trim(): loại bỏ khoảng trắng ở đầu hoặc cuối chuỗi.

## Array Functions

1. Hàm array_filter(): Lọc các giá trị của một mảng bằng hàm gọi lại.
<details open>
<summary>Example</summary>

````
<?php
function test_odd($var)
  {
  return($var & 1);
  }

$a1=array(1,3,2,3,4);
print_r(array_filter($a1,"test_odd"));
?>
````
</details>
2. Hàm array_merge(): hợp nhất 2 mảng thành một.
<details open>
<summary>Example</summary>

```
<?php
$a1=array("red","green");
$a2=array("blue","yellow");
print_r(array_merge($a1,$a2));
?>
```
</details>
3. Hàm array_pop(): Xóa phần tử cuối của mảng.
<details open>
<summary>Example</summary>

```
<?php
$a=array("red","green","blue");
array_pop($a);
print_r($a);
?>
```
</details>
4. Hàm array_push(): thêm phần tử vào cuối mảng.
<details open>
<summary>Example</summary>

```
<?php
$a=array("red","green");
array_push($a,"blue","yellow");
print_r($a);
?>
```
</details>
5. Hàm array_search(): Tìm kiếm theo từ khóa và trả về key của nó trong mảng.
<details open>
<summary>Example</summary>

```
<?php
$a=array("a"=>"red","b"=>"green","c"=>"blue");
echo array_search("red",$a);
?>
```
</details>
6. Hàm array_shift(): Xóa 1 phần tử đầu mảng vả trả về phần tử đó.
<details open>
<summary>Example</summary>

```
<?php
$a=array("a"=>"red","b"=>"green","c"=>"blue");
echo array_shift($a);
print_r ($a);
?>
```
</details>
7. Hàm array_unshift(): Thêm phần tử vào đầu mảng.
<details open>
<summary>Example</summary>

```
<?php
$a=array("a"=>"red","b"=>"green");
array_unshift($a,"blue");
print_r($a);
?>
```
</details>
8. Hàm count(): Trả về số phần tử của mảng.
<details open>
<summary>Example</summary>

```
<?php
$cars=array("Volvo","BMW","Toyota");
echo count($cars);
?>
```
</details>
9. Hàm sort(): sắp xếp mảng.

## File handling