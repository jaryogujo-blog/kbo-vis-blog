---
sectionid: time-series
sectionclass: h2
parent-id: related-works
title: 시계열 자료 시각화
number: 3100
---
대상이 되는 KBO 리그 자료는 연대기적으로 나열된 시계열 자료(Time-series data)다. 프로젝트 진행 시 영감을 받은 성공적인 시계열 자료 시각화 프로젝트들을 정리했다.   

> [Horizon graph][2]
> ![호리호리](http://dl.dropbox.com/s/6duntelzs1btpt0/horizon.png)
>
>*image from [the article of Jeffery Heer et al.](http://homes.cs.washington.edu/~jheer/files/zoo/)*

Horizon graph는 공간 효율적인 시계열 자료 시각화 방법이다. 시계열 자료의 빈도 영역(frequency domain)을 접어올려 y축 방향의 공간을 탄력적으로 활용할 수 있다. 이를 통해 다수의 시각화를 수직방향으로 병치하여 확인할 수 있다.

> [Fluxflow][4]
>
> ![플럭스플로-](http://dl.dropbox.com/s/o1n1zkytxgbp9oi/fluxflow.PNG) 
>
> *image from [the paper of Jian Zhao et al.](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=6876013)*

Fluxflow는 소셜 미디어(social media)에서 수집한 시계열 자료를 다차원으로 분석하기 위해 고안된 시각화 방법이다. 시계열의 전반적인 특징을 요약하여 보여주는 _디스크 형태의 글리프(glyph)_를 사용한다.

> [Pinas view][3]
>
> ![트리트리](http://dl.dropbox.com/s/ifpj6uj33v38x3k/pinusview_360.png)
>
> *image from [the paper of Mike Sips et al.](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?tp=&arnumber=6327296)*

Pinas view는 구간 별로 aggregation된 시계열 자료의 경향을 한눈에 보여주는 시각화다. 그림에서 자료의 맨 가운데 값인 '01년도를 어떤 시간 간격(time interval)의 중점으로 두고 그 크기를 점점 키워간다고 해보자. 처음에는 단 하나의 시점(time point)만을 나타내겠지만 최후에는 시계열 자료 전체를 포함하게 된다. 이 시각화에서 수직방향의 상승이 의미하는 바가 그것이다. 위치에 할당된 색은 그 시계열 구간의 대표값을 나타낸다.

[info_vis]: http://www.infovis-wiki.net/index.php?title=Information_Visualization
[visual_cue]: http://www.infovis-wiki.net/index.php?title=Visual_Cue
[glyph]: http://www.infovis-wiki.net/index.php?title=Glyph
[ui]: https://ko.wikipedia.org/wiki/%EC%82%AC%EC%9A%A9%EC%9E%90_%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4
[1]: http://www.nytimes.com/newsgraphics/2013/09/28/eli-manning-milestone/
[2]: http://www.stonesc.com/Vis08_Workshop/DVD/Reijner_submission.pdf
[3]: http://gfzpublic.gfz-potsdam.de/pubman/item/escidoc:100075:1/component/escidoc:100074/7_GISDAY-2012_sips_pinus_bib.pdf%3Bjsessionid=554A634777B67F600FFE69D67CE829F5
[4]: https://www.youtube.com/watch?v=OZMubJ0v32Q
[5]: https://namu.wiki/w/KBO%20%EB%A6%AC%EA%B7%B8
[6]: https://ko.wikipedia.org/wiki/KBO_%EB%A6%AC%EA%B7%B8
[7]: http://www.koreabaseball.com/History/Top/Hitter.aspx
[8]: http://www.nytimes.com/2006/04/02/sports/20060402_BONDS_GRAPHIC.html?_r=0