# aigo-indigenous-language-tts

## Preface 前言

隨著數位科技普及化與行動學習潮流到來，及原住民族語言隨人口老化逐漸失傳，相關教材及語言傳承需求持續增長，然而委外配音成本高，非常浪費人事及時間成本。台灣原住民族語言的書寫，從聖經、聖詩譯本、族語教材及坊間各種書寫文本，以羅馬拼音最為通行，透過AI自然語言處理研發智能配音模組，將輸入的文字自動合成為更擬真人、自然流暢的音檔，以取代委外高成本的配音成本，也能解決語言失傳的問題。
<br>
## Updates 更新紀錄
將Tacotron成功移植到網站(本機)
<br>

## Data samples 資料樣本

### To be contiuned
<br>

## 模型

使用 2017年Google推出的論文作為模型
[Tacotron: Towards End-to-End Speech Synthesis ](https://arxiv.org/pdf/1703.10135.pdf) 

## Usage 使用方法

執行 Train Test Tacotron.ipynb 檔案
![image](https://user-images.githubusercontent.com/45057687/137441558-759f6f8a-a926-4d81-859b-8ee9be35220c.png)

將會loading我們已經訓練好了檔案
![image](https://user-images.githubusercontent.com/45057687/137447822-9c75b7f2-8d22-4655-a5cc-f964d1681993.png)

執行到最下面可開啟網站
![image](https://user-images.githubusercontent.com/45057687/137441675-6477e9b6-954b-42cf-b561-b8124a6547db.png)

可以使用本團隊示範用的範本 M1_trv_test.txt裡面的句子
在符號 *|* 左邊是原本的音檔的檔名
![image](https://user-images.githubusercontent.com/45057687/137448616-2cedc33a-0f6e-4eb6-93cf-35d8a988eba5.png)

輸入至我們的textarea
提交後下方即會呈現這個音檔的結果
![image](https://user-images.githubusercontent.com/45057687/137449030-c8e4c51a-276c-4535-b0fc-73cecc06e209.png)

如果需要知道Alignment的結果 
可以將 _figures_ 設為True
``` bash
synthesis_speech(model, text=input_text, figures=True, path=wav_path+wav_name)
```


<br>

## Citing
```
@misc{AI.FREE2020,
  author = {Po-Chuan Chen, Chung-Chia Cheng, You-Qian Lee},
  title = {aigo-indigenous-language-tts},
  year = {2021},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/AI-FREE-Team/aigo-indigenous-language-tts}},
}
```
