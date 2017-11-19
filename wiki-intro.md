# Functional Programming

_關於 subroutine programming(子程序編程)，可以參考 procedural programming(序列化編程)_

_https://en.wikipedia.org/wiki/Procedural_programming_

**在電腦科學裡，functional programming 是一種 programming paradigm(編程范型)**

_(編程范型是什麼，請參考這兩篇)_

_https://stackoverflow.com/questions/4243187/whats-the-difference-between-design-patterns-and-architectural-patterns_ 

_https://stackoverflow.com/questions/4787799/difference-between-programming-paradigm-design-pattern-and-application-architec_ 

_http://allthingsjavascript.com/blog/index.php/2017/04/20/what-is-the-difference-between-a-programming-paradigm-and-a-design-pattern/_  

**一種用來建造電腦程式的結構的風格 - 核心概念是將我們寫程式的運算部分，寫的跟 mathematical functions 一模一樣，並且去避免「改變 state」以及任何「非常數的資料」**

**他是一種 declarative(宣告式的) programming paradigm(編程范型)，這代表了我們寫程式的時候會只使用 expressions(表達式) 以及 declarations(宣告)，而不去使用 statement(聲明)**

_https://goo.gl/f9iuun_ 

_https://stackoverflow.com/questions/1013385/what-is-the-difference-between-a-function-expression-vs-declaration-in-javascrip_  

**在 functional code(函數式編程的程式碼) 中，一個 function 的 return (輸出值)，只會被這個 function 所呼叫的所有 argument (參數) 影響，所以呼叫同一個 function f 兩次，並且給它完全一樣的參數 x，這兩個 function 每次都會輸出完全一樣的結果 f(x)**

**這跟不少有序列化特性的程式碼，像是他們會去閱讀 local 或是 global 的 state，並且會根據不同時間呼叫，以及產生不同的 result，有極大的對比**

**完全 eliminate(消除) side effects(副作用)，也就是在 function 執行中，不去閱讀，或改動任何跟 function input 無關的 state，可以產生更簡潔以及易懂的程式行為，這也就是 functional programming 想要解決的核心問題之一**

**Functional programming 的由來是來自於 lambda calculus(λ運算)，一個在 1930 年代為了研究 「computability(可運算問題)」 、「Entscheidungsproblem(可判定性問題)」、「function definition(函數定義)」、「funcion application(函數應用)」、以及 「recursion(遞迴)」 ****所發展的 formal system(形式系統)**

_https://en.wikipedia.org/wiki/Lambda_calculus_

_https://en.wikipedia.org/wiki/Formal_system_ 

_https://en.wikipedia.org/wiki/Computability_ 

_https://en.wikipedia.org/wiki/Entscheidungsproblem_ 

_https://en.wikipedia.org/wiki/Function_application_  

**許多 functional programming languages(函數式編程語言) 可以被視為 「λ運算」後續發展以及實作，有另一種著名的 declarative programming paradigm(宣告式編程范型) -「logic programming(邏輯式編程)」，是基於 relations (數學關係) 的**

_https://en.wikipedia.org/wiki/Finitary_relation_

**作為對比，imperative programming(指令式編程) 會使用原始碼中的各種指令來改變 state，最簡單的範例就是 assignment(賦值)** **指令式編程中，的確也有所謂的 function，但不是數學定義上的那種，而是一種接近 subroutine 的東西  
他們可以有各種 side effect，並且有可能會改變到程式裡的 state，所以這類的 function 常常會忽略掉 return 值**

_https://en.wikipedia.org/wiki/Imperative_programming_

_https://en.wikipedia.org/wiki/Assignment_(computer_science)_ 

**因為這些特性，這些 function 基本上是缺乏 referential transparency(引用透明度) 的，也就是，你明明寫了兩個一模一樣的 expression，卻可能在程式運作的不同時間點得到不同的運算結果**

**Functional programming 已經在 academia(學術圈) 被廣為重視了，雖然在商業上之前並沒有  
但是在一些支援 functional programming 的傑出程式語言像是 Common Lisp、Scheme、Clojure、Wolfram Language(Mathematica)、Racket、Erlang、OCaml、Haskell、F#，也在不少工業及商業軟體上被許多組織採用** 

**JavaScript，世界上做廣為流傳的程式語言，也同時有著「無型別 functional language」 的特性，並同時融合了 imperative(指令式) 以及 OO(物件導向式) 的范型**

**Functional programming 也同時被一些專業領域的 programming language 所使用，像是 R(統計學)、J, K, Q(用於金融分析的 Kx Systems)、XQuery/XSLT(XML)、Opal** 

**廣為使用的宣告式語言，像是 SQL、Lex/Yacc 也使用了不少 functional programming 的元素，特別是避開「可改動的變數」**

**就算你使用一個沒有特別設計來寫 functional programming 的語言，你也一樣可以使用 functional 的風格來寫，舉例而言，指令式的語言 Perl，常常被教科書拿來當作範例，如何在指令式語言中融合 functional programming 的理念**

**在 PHP 中也是同樣的，C++ 11、Java 8、C# 3.0，也同時加入了能支援 functional 風格的功能，Julia 程式語言也同時提供了 functional programming 的風格，Scala 算是一個有趣的例子，他常常被使用 functional style 寫成，但是他存在著一個灰色地帶，因為他對於 side effect 以及 可變的 state 有著彈性的定義**