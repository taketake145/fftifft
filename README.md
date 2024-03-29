# プログラムの説明
  - 9~18行目 : 画像を読み込み、画像のサイズを測り規定値より大きかったらリサイズする処理。
  - 20~26行目：画像を2次元フーリエ変換し、その平均と標準偏差を求める処理。
  - 28,29行目：オリジナル画像を表示する処理。
    -plt.subplot(a,b,c)は画像を並べて表示させるためのモノ。
  - 31~33行目：2次元フーリエ変換した画像を表示する処理。
  - 35~48行目：画像と同じサイズの枠を表示する処理。
  - 50~57行目：マウスの操作を読み込むために必要な処理。
  - 61~64行目：クリックしたときの処理
  - 66~68行目：クリックを解除したときの処理
  - 70~72行目：マウスを動かしたときの処理
  - 74~76行目：キーボードを押下したときの処理
  - 78~80行目：キーボードを押下を解除したときの処理
  - 82~148行目：クリックしたところのフーリエ変換のパラメータを表示し、それを重ね合わせたものを表示する処理。
  
# 使用方法
  - 12行目で画像のアドレスを指定。
  - 実行すると5つの画像が並んで表示されるため、下段の真ん中の画像をCtrlを押しながらクリックする。
  - するとリアルタイムで逆フーリエ変換が行われる。
  
# 使用したバージョン
  - Python 3.7.3
  - import numpy
  - import numpy.fft.fftpack as fftpack
  - from PIL import Image
  - import matplotlib.pyplot as plt
  
# 参考にしたサイト
  - 「２次元フーリエ変換／逆変換の解説 Two-dimensional Fourier Transform Demo」https://www.youtube.com/watch?v=pCVdNYvORVw&feature=plcp
  - 「Windows用Portable PsychoPy / VisionEgg」 http://www.s12600.net/psy/etc/python.html
    - 表示方法をYouTubeの表示のように変更した。
