## report
When I set the bandwidth limit to Slow 3G in Chrome(92.0.4515.159（Official Build）（x86_64）) and press click twice, the no-cache image in the iframe disappea
rs. The reason seems to be that when you call a no-cache image in an iframe, if you delete the img DOM before the im
age finishes loading and cancel the loading, the data of the same image in that screen will be lost. (Not tested in firefox, safari)

Chrome (92.0.4515.159（Official Build）（x86_64）)で 回線速度をSlow 3Gにして clickを2回押すと、iframe 内のno-cache画像が消える。
原因は iframeでno-cache画像を呼び出した時に、画像の読み込みが終わる前にそのimg DOMを消して読み込みキャンセルすると、その画面の同じ画像のデータがなくなるためのようだった。
(Chromeのみ確認で、firefox, safariでは未確認)
