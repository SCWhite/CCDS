# C語言背景

## C語言的由來
C語言最早由丹尼斯·里奇（Dennis Ritchie）為了在PDP-11電腦上運行的Unix系統所設計出來的程式語言，第一次發展在1969年到1973年之間。<br>
C源於BCPL語言，後者由馬丁·理察德（Martin Richards）於1967年左右設計實作。BCPL是一門"無類型"的程式語言：它僅能操作一種資料類型，即機器字（machine word）。1970年，肯·湯普遜為執行在PDP-7上的首個Unix系統設計了一個精簡版的BCPL，這個語言被稱為B語言，它也是無類型的。<br>
Unix最早運行在PDP-7上，是以組合語言寫成。在PDP-11出現後，丹尼斯·里奇與肯·湯普遜著手將Unix移植到PDP-11上，無類型的語言在PDP-11上愈發顯得合適。PDP-11提供了多種不同規格大小的基本物件：一位元組長的字元，兩位元組長的整型數以及四位元組長的浮點數。B語言無法處理這些不同規格大小的物件，也沒有提供單獨的操作符去操作它們。<br>
C語言最初嘗試通過向B語言中增加資料類型的想法來處理那些不同類型的資料。和大多數語言一樣，在C中，每個物件都有一個類型以及一個值；類型決定了可用於值的操作的含義，以及物件占用的儲存空間大小。<br>
1973年，Unix作業系統的核心正式用C語言改寫，這是C語言第一次應用在作業系統的核心編寫上。<br>
1975年C語言開始移植到其他機器上使用。史蒂芬·強生實作了一套「可移植編譯器」，這套編譯器修改起來相對容易，並且可以為不同的機器生成代碼。從那時起，C在大多數電腦上被使用，從最小的微型電腦到與CRAY-2超級電腦。C語言很規範，即使沒有一份正式的標準，你也可以寫出C程式，這些程式無須修改就可以執行在任何支援C語言和最小執行時環境的電腦上。<br>
C最初在小型機器上實作，並且繼承了一系列小語種程式語言的特點；與功能相比，C的設計者更傾向於簡單和優雅。此外，從一開始，C語言就是為系統級編程而設計，程式的執行效率至關重要，因此，C語言與真實機器能力的良好符合也就不足為奇。例如，C語言為典型硬體所直接支援的物件：字元，整數（也許有多種大小），以及浮點數（同樣可能有多種大小）提供了相應的基本資料類型。<br>
from wiki

**簡單的說**  
> C語言，於1969年至1973年間，由丹尼斯·里奇與肯·湯普遜， 以B語言為基礎，在貝爾實驗室設計、開發出來。  
