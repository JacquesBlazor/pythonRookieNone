# pythonRookieNote
pythonRookieNote

補充對新手入門 Python 時一些基本而重要資訊提供參考:

1. Python IDLE 的套件管理程式是 pip.exe, 安裝 IDLE 後可以在命令提示字元輸入
-   pip --version, 如果出現找不到 pip, 安裝時要勾 PATH, 沒勾可以自己加.

2. 在 Python 裡是透過 import 來匯入套件, 內建的函式像是 print(), 不需要套件.

3. 套件其實就是函式庫, 透過 pip 安裝的套件是由 PiPy <a href=https://pypi.org/ target=_blank rel=nofollow>https://pypi.org/</a> 來的.

4. 安裝套件的方式是在命令列輸入 pip install &lt;套件名稱&gt;,
   例如: pip install virtualenvwrapper

5. 但有時你會看到 conda install 的指令. conda 是另一個套件管理程式.
   它安裝的來源不是同一個. 安裝後套件的目錄也不是同一個.

6. 有些套件在安裝 IDLE 後就裝好了, 只是沒有匯入. 像是 os 套件, sys 套件等.

7. 套件和模組有時是指同一個東西. 它們只差一個 __init__ 檔案外大致相同.

8. import sys 套件後有很多資訊可以參考, 例如:
   分別輸入:
-   (a) sys.executable -&gt; 可以看到目前 python 直譯器的目錄位置
-   (b) sys.path -&gt; 可以看到套件匯入時的順序.
-   (c) sys.path.append('路徑名') -&gt; 可以暫時新增要匯入的模組的檔案路徑
-   (d) sys.builtin_module_names -&gt; 可以查看 Python 所有內建的模組名稱

9. import os 套件後也些資訊可以參考, 例如:
-   (a) os.getcwd() -&gt; 可以知道目前的工作目錄, 如果讀/寫檔案會在這個目錄

10. 而 pip 也是可以 import pip, 也有些資訊可以參考, 例如:
-   (a) pip.__path__ -&gt; 可以看到 pip 目前放在哪個目錄,
       套件的目錄名稱通常為 /site-packages 通常在那個 pip 的上一層

11. 另外兩個常用指令 dir 和 help 可以找到很多基本資訊. 像是:
-   (a) help('modules') -&gt; 可以查看本機所有可用的模組
-   (b) dir(\_\_builtins\_\_) -&gt; 可以查看內建函數和物件

12. 同一台電腦裡有時候會有多個 python 的執行檔, 特別是用虛擬環境時.

13. Python 的虛擬環境其實只是一個資料夾, 它不是虛擬機器的意思.

14. 透過建立 Python 的虛擬環境, 電腦上會有多個 python 的直譯程式.
    彼此是獨立互不關聯的.

15. 由於 python有v2和v3兩個版本, 同時每個套件又有n個不同的版本, 有些套件
    和套件間的相依套件/模組會互相衝突.使用虛擬環境 (意思是建一個資料夾
    放可執行 Python 的環境) 可以將不同版本的python和套件庫獨立出來.

16. 虛擬環境的產生也有很多不同的方式. 有用 PyCharm IDE 產生的, 用 conda
    產生的, 用 pip venv, virtualenv 或用 virtualenvwrapper等很多種.

17. Python 程式是用縮排而非括號來區隔程式區塊, 縮排要用空白而非tab, 使用
    tab 縮排會產生執行上的問題. 在使用編輯器時要記得把 tab 轉成空白.

18. 有些程式碼撰寫規範, 像是 PEP8 有空閒的話可以參考看看.我是沒看過.XD

19. Python 的 IDEL 可以在 config-extensions.def 檔案裡外掛一些功能.
    像是 ClearWindows.py 可以在 IDLE 的功能表新增清理畫面的功能.

20. Python 的 IDLE 也有內建的除錯功能, 也可以匯入 import pdb 來除錯.

21. Python 的 List(列表), Tuple(元組) 類似其他語言的陣列(Array), 但
    Python 在 3.3 開始還有另一個內建的 array(陣列) 型別 (import array)
    以及 NumPy 套件的 np.array 型別, 剛開始學 Python 時很容易弄混.

22. Python 直譯器是由 C 寫成的, 而 CPython 是官方的實作. 也有其他的實作.

23. 如果想知道 Python 內建的關鍵字(識別字)，可以 import keyword 匯入keyword 套件

-    print(keyword.kwlist)
