# Correspondences
Electronic music based on the poem Correspondences by Baudelaire.


Open the program launch.maxpat first,
and follow the instruction at the upper left cornor.
If you fail to automatically launch files,
please follow the launch process below

<<<<<<< HEAD

 # Launch Process

1. Open audio_player.maxpat, gran.maxpat and Correspondances_Section1_Pitchshift_2.maxpat (in the folder Seesion1). Then, open main.maxpat

2. Turn on audio and make sure the main output is unmute. Press key 'M' to unmute main output.
=======
Launch Process

1. open main.maxpat
2. open vocovocoder.maxpat
3. open Correspondences-Seesion1
4. open EQ&Filter.maxpat
5. turn on all volume
>>>>>>> baecff50a2182685f1e75e2f48b132b17a924a1d



Demonstration

For audio demonstration
<<<<<<< HEAD
Soundcloud: https://soundcloud.com/user-347478993-140218940/0629-rehearsal

For video demonstration
Youtube: https://youtu.be/rRHc1kgiS0Q



Explanation of each patch


Launch.maxpat（作者王博君）

此Patch用來自動開啟所需要的檔案，請按照上方所寫的步驟使用。
可以照著規則任意增加需要開啟的檔案，惟須注意main.maxpat必須最後一個開啟。

使用步驟
Step 1: Drag the folder of these programs, Correspondances.

Step 2: Click the button

Step 3: Save this program for automatically launch files when open this lauching program.


main.maxpat （作者王博君）

Main Patch，功用是監控和調整不同Patch之間的音量，並且驅動其他Patch。
我的設計是右邊的區塊作為Gain Controller，監控並調整個別的Patch內部的輸出，避免在輸出到Main Patch前就爆掉了。
下方是總輸出，監控並調整最後的輸出。


Correspondances_1_Final.maxpat

Patch的主控區：

控制音樂的開始與結束。

除了可以直接在電腦上操作以外，
我們亦在表演時的手機介面上，放置開關，以利隨時做調整。

作品第一段的核心：

此為Baudelaire - "Correspondances"的全詩朗誦音檔。
希望在一開始，能夠呈現詩詞裡最純粹的抑揚頓挫，而往後再加以變化、變形。

四組cycle～音堆：

運用delay由左至右，循序漸進地疊加出整首作品的background。
而其中，每組音堆利用counter區分成0和1，再以line～使其做出漸強漸弱的效果。

音量控制區：

因應不同需求，以line物件將音量由弱轉強、或由強轉弱。
運用四組音堆攀高近似12個半音，以在作品最後增加張力：
作法為在表演時的手機介面上，放置trigger鍵，等待表演的張力到達飽和時，便觸發它，使原本在background的四組音堆，以不同的速率，透過相乘半音的倍數1.05964，以line往上攀升，推進到作品的高點。


gran.maxpat （作者林劭奇）

此patch為粒狀合成，皆由手機控制，紫色為驅動所有聲音檔的開關；橘色為驅動背景低音往上爬升的開關。


audio_player.maxpat （作者王博君）

這個Patch是連接四隻手機播放音檔的部分，我的設計是用Syntien的Motion功能。
手機的Roll（側轉）改變音檔播放的速度，也就是講話的音高；Pitch（仰角）改變音量，因此可以搭配手勢表現出Dynamic；我把Yaw（手機平行地面的方向）切割成三個區塊，正面90度（十點半至一點半方向）是 "Correspondances"，左面90度（七點半至十點半方位）是 "La nature est un temple" ，右面90度是（一點半至四點半方位）是 "où de vivants piliers“ 。


=======
Soundcloud: https://soundcloud.com/user-347478993-140218940/rehearsal-in-0610/s-80bxBGMLFWy

For video demonstration
Youtube: https://youtu.be/Ht001UGP3mk
>>>>>>> baecff50a2182685f1e75e2f48b132b17a924a1d
