# テクノロジー（藤原） 11/1授業

```
(kogadoom:~/workspace $ git clone git@github.com:kogatoshi/lecture-1101.git
Cloning into 'lecture-1101'...
Warning: Permanently added 'github.com,192.30.253.113' (RSA) to the list of known hosts.
remote: Counting objects: 3, done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
kogadoom:~/workspace $ pry
[1] pry(main)> num=2
=> 2
[2] pry(main)> if nume % =2
SyntaxError: unexpected '='
if nume % =2
           ^
[2] pry(main)> if nume % 2==0
[2] pry(main)*   puts
[2] pry(main)*   puts"偶然です"
[2] pry(main)* end
NameError: undefined local variable or method `nume' for main:Object
Did you mean?  num
from (pry):2:in `__pry__'
[3] pry(main)> puts "偶数です。" if num % 2 == 0
偶数です。
=> nil
[4] pry(main)> num = 1000
=> 1000
[5] pry(main)> if num >=1500
[5] pry(main)*   puts"送料無料です"
[5] pry(main)* elsif 0 < num && num < 1500
[5] pry(main)*   puts "送料300円です。"
[5] pry(main)* else
[5] pry(main)*   puts "入力が間違ってます。"
[5] pry(main)*
[5] pry(main)* end
送料300円です。
=> nil
[6] pry(main)> num = rand 3
=> 2
[7] pry(main)>
[8] pry(main)> case num
[8] pry(main)* when 0
[8] pry(main)*   puts"
[8] pry(main)*   puts"吉です"
[8] pry(main)* when 1
[8] pry(main)* puts "凶です"
SyntaxError: unexpected tIDENTIFIER, expecting end-of-input
puts "凶です"
               ^
[8] pry(main)> when 1
SyntaxError: unexpected keyword_when, expecting end-of-input
when 1
    ^
[8] pry(main)> num = rand 3
=> 0
[9] pry(main)> case num
[9] pry(main)* when 0
[9] pry(main)*   puts"吉です"
[9] pry(main)* when 1
[9] pry(main)*   puts "凶です"
[9] pry(main)* else
[9] pry(main)*   puts "大凶です"
[9] pry(main)* end
吉です
=> nil
[10] pry(main)> def triangle(b, h)
[10] pry(main)*   result = b * h / 2.0
[10] pry(main)*   result
[10] pry(main)* end
=> :triangle
[11] pry(main)> Array#empty?
=> Array
[12] pry(main)> name = [1, 2, 3].empty?
=> false
[13] pry(main)> []. empty
NoMethodError: undefined method `empty' for []:Array
Did you mean?  empty?
from (pry):32:in `__pry__'
[14] pry(main)> name = gets

=> "\n"
[15] pry(main)> 10.times do |i|
[15] pry(main)*   print i, ", "
[15] pry(main)* end
0, 1, 2, 3, 4, 5, 6, 7, 8, 9, => 10
[16] pry(main)> a = ["りんご", "みかん", "ぶどう"]
=> ["りんご", "みかん", "ぶどう"]
[17] pry(main)> a.each do |item|
[17] pry(main)*   puts "おいしい" + item + "だよ"
[17] pry(main)* end
おいしいりんごだよ
おいしいみかんだよ
おいしいぶどうだよ
=> ["りんご", "みかん", "ぶどう"]
[18] pry(main)>
```