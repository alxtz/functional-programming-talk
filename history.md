# History(歷史)

Lambda Calculus 提供了描述 function 和運算的理論基礎，相較於一種程式語言，Lambda Calculus 更像是種數學上的抽象，但是它幾乎是現今所有 functional programming languages 的基礎  
另一個相近的理論公式，「combinatory logic」常常被認為是 Lambda Calculus 的高層抽象，並優於他的核心概念  
Combinatory logic 和 Lambda Calculus 是為了解決同一個問題而被開發出來的，那就是為數學的運算基礎提供更清楚的運算方法

最早的 functional 語言是 Lisp，最早開發於 1950 年的晚期，為了提供開發 IBM 700/700 的 MIT 科學家 John MacCarthy 使用  
Lisp 最早介紹了不少函數式編程的 paradigmatic 特性，儘管 Lisp 最早屬於一種 multi-paradigm 的語言，每次有新的 paradigm 被發展，都會將這些概念融入裡面  
早期的 dialects ，像是 Scheme 或 Clojure，或是像 Dylan 或 Julia 這樣的 offshoots(分枝)，都是 sought to(力求) 簡化、以及裡論化 Lisp，使用 functional 的理論核心來做到這件事情，同時，Common Lisp 也被開發了出來，他是一種被設計來保存並更新相較於舊的這些 paradigmatic 特性

Information Processing Language(資訊處理語言, IPL)，常常被引用來當做第一個基於電腦的 FP 語言，他是一種組語風格的語言，專門用來操作資料 list，值得一提的是，他開始有了 generator 的概念，基本上就是一個 function，他可以去拿另一個 function 來當作參數，並且，基於他是一個組語等級的語言，程式碼同時也是 data，所以 IPL 可以被當作有著 higher-order functions  
然而，其實 IPL 也同時著重在改變 list 的結構

Kenneth E. Iverson 在 1960 年初開發了 APL，在他 1962 年的書中「A Programming Language」中做了介紹，APL 是 John Backus 的「FP」的重要影響，在 1990 年初，Iverson 和 Roger Hui 開發了 J，在 1990 年中，Arthur Whitney，一個之前跟 Iverson 合作的人，創造了 K，是一種在金融行業和 Q 一起廣泛使用的語言

John Backus 在1977 年的 Turing Award 課堂「Can Programming Be Liberated From the von Neumann Style？A Functional Style and its Algebra of Programs」這堂課中介紹了 FP，他將函數式的程式定義為，使用一種 hierarchical way 大綱式的組合方法，來建構你的程式，很像是代數般的程式  
用現代語言來解釋，這代表著 functional programming program 遵照著「prinicple of compositionality」(組合律)，Backus 的論文使得 functional programming 的研究開始變得火熱，儘管其實他的論文強調的是 「functional-level programming」而不是我們現今將他與 Lambda Calculus 相關起來的 Functional Programming  

在 1970 年代，ML在愛丁堡大學被 Robin Milner 所開發出來，同時 SASL 以及 Miranda 也被發明了，以及NLP，NLP 是基於 「Kleene Recursion Equations」的，並且在他們展示他們在 program 轉換的研究中初次被介紹，Burstall, MacQueen, Sannella 後來合作開發了提供多型型態檢查的語言 ML，並創造了 Hope，ML最終開發成了不少分枝，包含了 OCaml，Standard ML，同時 Scheme 的發展，一個簡潔並且 Lexical Scope，以及沒那麼 pure 的 Lisp 分枝，在後來影響重大的 Lambda Papers，以及經典的 1985 textbook「Structure and Interpretation of Computer Programs」中被提及，並在廣泛的程式語言社群中帶來了重視

在 1980 年代， Per Martin-Lof 發展了 intuitionistic type theory(同時被稱作 constructive type theory)，他將 functional programs 及 constructive proofs 的數學證明組成了 dependent types，這帶來了不同的強大互動性理論證明基礎，並且影響了後續許多 functional programming language 的進展  
Haskell Language 在 1987 年代開始成為了一個共識，並且為 functional programming 的研究形成了一個公開標準，不少實作都在 1990 年後陸續出現