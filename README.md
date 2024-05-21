body 利用display:flex 將畫面置中
在body中加入container position設置為relative
在container中加入兩個form表單 position都設置為absolute
兩者的移動是利用transform向右移動100%、過度動畫則是利用animation、顯示則是透過opacity 0跟1的轉換
初始位置都在左側 設置left:0 ，sign-up先設置隱藏

其他第三方登入的icon 來源為fontawesome

接著建立一個toggleContainer 在此建立轉換註冊與登入畫面的按鈕
初始位置在form的右側 設置left:50% position也設置為absolute 並設置左下與左上的圓角
並在其中建立一個relative的toggle width設置為200% 在其中建立兩個toggle-panel 註冊及登入轉換的按鈕及文字
因為width為兩倍 所以會有一半超出container 但需要將toggle置於container中 為此設置left:-100%
兩個toggle-panel分別為左右兩側 其中設置按鈕 
點下時則是透過js 設置監聽器在註冊及登入的按鈕轉換container的class "active" 以此來符合css中設置好的class
左側panel預設位置 設置為 transform:translateX(-200%)
右側panel預設位置 設置為 transform:translateX(200%)

當container有active這個class時 右側的toggle-panel transform:translateX(0) (滑入container中)
沒有active時則是 左側的toggle-panel transform:translateX(0)
而toggle-container 也在有active時將位置移至-100% transform:translateX(-100%) 並將圓角改為右上右下


study coding from youtube video : AsmrProg 
https://www.youtube.com/watch?v=PlpM2LJWu-s&list=WL&index=2&t=877s
