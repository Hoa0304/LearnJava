# Java
## Nội dung bài học 

### [1. Kiểu dữ liệu]()
### [2. Array]()
### [3. Method]()
### [4. Toán tử ba ngôi (Ternary operator)]()
### [5. Câu lệnh điều kiện]()
### [6. Vòng lặp (Loop)]()


### 1. Kiểu dữ liệu 
<details>
<summary>Các kiểu dữ liệu nguyên thủy (Primitive Data Types)</summary>

1. Kiểu Boolean :

Kiểu __Boolean__ chỉ sử dụng lưu trữ cho 2 giá trị: true và false. Mục đích kiểu
Boolean thường được cho những câu điều kiện rẽ nhánh.

```java
boolean isDone = false
```

2. Kiểu byte :

Kiểu dữ liệu __Byte__ dùng để lưu trữ kiểu số nguyên có kích cỡ bằng 1 byte (8
bit). Giá trị có thể lưu được nằm trong khoảng từ -128 ( -2^7) đến 127 (2^7-
1).
```java
byte a = 100
```

3. Kiểu Short :

Kiểu dữ liệu __Short__ dùng để lưu trữ kiểu số nguyên có kích cỡ bằng 2 byte (16
bit). Giá trị có thể lưu được nằm trong khoảng từ -32,768 (-2^15) đến 32,767
(2^15-1).

```java
short a = 10000
```

4. Kiểu Int :

Kiểu dữ liệu __Int__ dùng để lưu trữ kiểu số nguyên có kích cỡ bằng 4 byte (32
bit). Giá trị có thể lưu được nằm trong khoảng từ -2,147,483,648 (-2^31) đến
2,147,483,647 (2^31-1)
5. Kiểu Long : 

Kiểu dữ liệu __Long__ dùng để lưu trữ kiểu số nguyên có kích cỡ bằng 8 byte. Giá
trị có thể lưu lưu được nằm trong khoảng từ -9,223,372,036,854,775,808 (-
2^63) đến 9,223,372,036,854,775,807 (2^63-1). Giá trị gán cần có kí tự ‘l’
phía sau.

6. Kiểu Float :

Kiểu dữ liệu __Float__ dùng để lưu trữ số thực có kích cỡ bằng 4 byte (32 bit). Giá
trị có thể lưu được nằm trong khoảng từ -3.4028235 x 10^38 đến -
3.4028235 x 10^38. Giá trị gán cần có kí tự ‘_f_’ phía sau.

```java
float a = 2.51f
```

7. Kiểu Double :

Kiểu dữ liệu __Double__ dùng để lưu trữ số thực có kích cỡ bằng 8 byte (64 bit).
Giá trị có thể lưu nằm trong khoảng từ -1.7976931348623157 x 10^308 đến
-1.7976931348623157 x 10^308. Giá trị gán có thể có hoặc không kí tự ‘d’
phía sau.
```java
double a = 2.52.d or double a = 2.52
```

8. Kiểu Char : 

Kiểu dữ liệu __Char__ dùng để lưu trữ kí tự có kích cỡ bằng 2 byte. Bản chất Char
lưu trữ code Unicode nhưng khi lại hiển thị ra ‘kí tự’ ứng với mã đó. Giá trị có
thể lưu trữ nằm trong khoảng ‘u0000’ đến ‘uffff’.

</details>

<details>
<summary>Các kiểu dữ liệu tham chiếu (Reference Types)</summary>

_Kiểu dữ liệu tham chiếu_ là kiểu dữ liệu của đối tượng. Biến của kiểu dữ liệu
tham chiếu chỉ chứa địa chỉ của đối tượng dữ liệu tại bộ nhớ Stack. Đối tượng
dữ liệu lại nằm ở bộ nhớ Heap. Một số kiểu dữ liệu cụ thể như các mảng
(Array), lớp đối tượng (Class) hay kiểu lớp giao tiếp (Interface).

```java
String name = "CamHoa"
```

<details>
<summary>Lớp bao (wrapper class)</summary>

> wrapper class (lớp bao) là một lớp được cung cấp để đóng gói các kiểu dữ liệu nguyên thủy (primitive data types) thành các đối tượng (objects). Mỗi kiểu dữ liệu nguyên thủy có một wrapper class tương ứng.

- Boolean: Đóng gói kiểu dữ liệu boolean.
- Byte: Đóng gói kiểu dữ liệu byte.
- Short: Đóng gói kiểu dữ liệu short.
- Integer: Đóng gói kiểu dữ liệu int.
- Long: Đóng gói kiểu dữ liệu long.
- Float: Đóng gói kiểu dữ liệu float.
- Double: Đóng gói kiểu dữ liệu double.
- Character: Đóng gói kiểu dữ liệu char.

```java
int number = 10;
Integer integerNumber = Integer.valueOf(number); // Chuyển đổi kiểu dữ liệu int thành Integer

// Hoặc có thể sử dụng cách viết ngắn gọn hơn
Integer integerNumber = number; 
// Autoboxing: tự động chuyển đổi kiểu dữ liệu int thành Integer
```
</details>
</details>
<br></br>



### 3. Method (Phương thức)
<details>
<summary>Cú pháp</summary>

_Sử dụng method để tái sử dụng lại code_

```java
access_specifier modifier type name (params){
    body
}
```

Trong đó : 
- access_specifier : chỉ định truy cập vào phương thức (public , private, protected)
- modifier : gán thuộc tính cho method (static, abstract,final)
- type : kiểu dữ liệu trả về (int,double,void : không có kiểu dữ liệu trả về "hàm k có return")
- params : chứa kiểu dữ liệu và tên của tham số 
</details>

<br></br>

### Tổng kết
```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        System.out.println("Hello world!");
        getinput();
    }
    public static void getinput(){
        int a;
        int b;
        int c;
        Scanner sc =  new Scanner(System.in);
        a = sc.nextInt();
        b=sc.nextInt();
        c = sc.nextInt();
        float d;
        d = Float.parseFloat(sc.nextLine());
        int[] ab = {1,2,3,4,5};
        int[] ac = new int[4];
        if(a>0){
            for(int i = 0;i<b;i++){
                System.out.println(i);
            }
            while(a!=0){
                a--;
                System.out.println(a);
            }
        }else{
            int max = (b>c) ? b :c;
            System.out.println(max);
        }

        do{
            b--;
            System.out.println(b);
        }while (b!=0);
        switch (c){
            case 1:
                System.out.println("Mot");
        }
    }
}
```