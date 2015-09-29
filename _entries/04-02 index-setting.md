---
sectionid: index-setting
sectionclass: h2
parent-id: data-manipulation
title: 성적, 성향 지표 선정
number: 4200
---

수집한 자료로부터 시즌별 팀의 성적, 성향을 나타내는데 사용될 지표를 선정했다. 직관적으로 이해할 수 있으면서도 본래의 함의를 왜곡하지 않도록 다음과 같은 점들을 고려했다. 

**Q1.  무엇을 지표로 할 것인가?**

개인 단위가 아닌 팀 전체의 특성을 표현해야 한다. 감독의 영향을 반영해야 한다.

**Q2. 어떤 기록을 사용할 것인가?**

이 프로젝트의 목적은 복잡한 시각적 분석 도구를 만드는 것은 아니다. 한정된 공간 안에 팀의 특성을 직관적으로 나타내야 한다. 
팀 단위의 야구 통계를 높은 수준으로 추상화하면 크게 공격, 수비로 나눌 수 있으며, 아래와 같이 정의할 수 있다.

>**공격**
> - 어떤 득점루트, 어떤 패턴으로 얼마나 **득점**했는가
> 
>**수비** 
>- 어떤 득점루트, 어떤 패턴으로 얼마나 **실점**했는가

이를 구체적으로 분석하기 위해서는 상황별 통계자료가 필요하나, 구할 수 없었다. 
이 프로젝트에서는 시즌 혹은 재임한 감독을 기준으로 **공격력**과 **수비력**의 전반적인 변화를 확인하기 위해 **시즌 별 총 득점, 실점**을 사용했다.
 
**Q3. 어떻게 지표(Index)화할 것인가?**

득점과 실점을 각각 공격력과 수비력에 대응시키려면 다음 두 조건을 만족해야 한다.
>1. 시즌 내에서 팀 간의 비교가 가능해야 함
>2. 서로 다른 시즌 간의 비교가 가능해야 함

두 번째 조건을 만족시키기 위해 시즌 별 리그 특성으로부터 독립된 지표를 사용해야 한다. 비모수적(non-parametric)인 방법과 모수적(parametric)인 방법으로 구할 수 있다.

> **모수적 방법**  
> - 측정된 자료가 특정한 분포(ex. 정규 분포)로부터 나오는 것을 가정한 방법
> *예) 평균, 표준편차*
> 
> **비모수적 방법**
> - 측정된 자료가 특정한 분포로부터 나오는 것을 가정하지 않는 방법
> *예) 중간값, 순위*

각 시즌별로 득점, 실점의 분포가 다르기 때문에 정규화를 하려면 많은 고려가 필요하다. 순위를 비교하는 것이 더 안전하다. 그러나 순위는 시각적인 요소로 치환하여 비교하기 어렵고, 정보를 많이 생략한다. 이 프로젝트에서는 모수적인 방법을 사용했다.


**Q4. 어떻게 보여줄 것인가?**

공격력과 수비력 비교의 경우의 수는 다음과 같은 양상을 띌 것이다.

> **공격력(수비력) 단일 비교**
> 
> 1. 한 팀의 시즌 별 공격력(수비력) 비교
> 2. 한 팀의 재임 감독 별 공격력(수비력) 비교
> 3. 여러 팀의 특정 시즌 공격력(수비력) 비교
> 4. 한 감독의 재임시기 별 공격력(수비력) 비교
> 
> **공격력-수비력 연관 비교**
> 
> 1. 한 팀의 시즌 별 공격력-수비력 편차 비교
> 2. 한 팀의 재임 감독 별 공격력-수비력 편차 비교
> 3. 여러 팀의 특정 시즌 공격력-수비력 편차 비교
> 4. 한 감독의 재임시기 별 공격력-수비력 편차 비교 

공격력과 수비력을 각각 비교하는 것도 중요하나 그 편차를 보는 것 또한 의미가 있다. 전자가 공격/수비 부문의 팀의 성취를 나타낸다면 후자는 공격, 수비의 균형을 나타낸다. 이는 팀의 개성을 드러내는 가장 기본적인 값이며 팀 간의 절대적인 전력 차로부터 독립적이다.



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