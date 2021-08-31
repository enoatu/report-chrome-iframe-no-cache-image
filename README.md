## report
回線速度をSlow 3Gにして clickを2回押すと、iframe 内のno-cache画像が消える
原因は iframeでno-cache画像を呼び出した時に、画像の読み込みが終わる前にそのimg DOMを消して読み込みキャンセルすると、その画面の同じ画像のデータがなくなるためのようだった
(Chromeのみ確認で、firefox, safariでは未確認)
