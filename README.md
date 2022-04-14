# Sogaeting
## Toy Project 
서울 주요지역내에서 소개팅을 목적으로한 식당 정보를 정리해보고자 한다 <br>
-Data : 구글맵 가로수길,성수,강남,합정,이태원 근처 레스토랑을 키워드로 검색하여 나온 식당의 리뷰<br>
-방법론 : 리뷰의 언급된 단어 중 소개팅과 관련이 있는 단어(ex:분위기,데이트)가 언급된 빈도를 카운트하여 각식당의 소개팅랭킹 점수로 활용(mecab사용)<br>
-시각화 : 구글맵의 주소정보를 지오코딩하여 [태블로 대시보드](https://public.tableau.com/app/profile/.36194374/viz/sogaeting/1_1?publish=yes)의 지도로 시각화<br>
<br>

전체 크롤링된 가게 수는 840개이며 이중 리뷰가 없는 90개를 제외하고 
750개 식당의 리뷰의 단어 분포는 아래와 같음
![](https://postfiles.pstatic.net/MjAyMjAzMzBfNCAg/MDAxNjQ4NjQ2Nzg3MjEy.hE8OT7ErYjXPML5GlyDLczurD5kuxdO4Hm00Mp3fHUsg.pmQHYTItDLh7IIL09NC_pv2LsyhqqUuOjdlaCVMXsFkg.PNG.ps712/image.png?type=w773)
<br>
![](https://postfiles.pstatic.net/MjAyMjAzMzBfNjMg/MDAxNjQ4NjQ2NzY5MTM3.HdWSWuMQmbZ4vTf_e9rnxYZYnD0H1nqF9fYW4gAvdxAg.Ak2Ugva-0LciS4xCPKEojYJGCZ7Koyn1cjZxluf_KOAg.PNG.ps712/image.png?type=w773)
<br>
Wordcloud<br>
![](https://postfiles.pstatic.net/MjAyMjAzMzBfMTcx/MDAxNjQ4NjQ2ODA1MTE1.PjXMYSXjBfm5q0C4VLq2JisS4ZmIMB5DWVwcm1sUMkUg.vbBN4Q9TswgS6hDmWAgycbu_z5iijTyRoEit_a2FkJsg.PNG.ps712/image.png?type=w773)

<리뷰 중 소개팅 관련 단어 추출>
![](https://postfiles.pstatic.net/MjAyMjAzMzBfMjU5/MDAxNjQ4NjQ2ODg3MTMx.t18EX4gaVBOquBjyLpic_WV2mEyv6X-ACe_f8eikSA4g.HFQARl84_0YTb9Vwlszx1UErHifsfAyXD8LWHlyXPPMg.PNG.ps712/image.png?type=w773)

이후 각주소의 지오코딩을 하여 위도 경도를 삽입한 후 태블로로 시각화함<br>
[대시보드보기](https://public.tableau.com/app/profile/.36194374/viz/sogaeting/1_1?publish=yes)
<div class='tableauPlaceholder' id='viz1649941186699' style='position: relative'><noscript><a href='#'><img alt='빅데이터 기반 소개팅 장소 추천가로수길, 강남, 성수, 이태원, 합정의 구글지도 리뷰 분석하여 소개팅 장소 추천 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;so&#47;sogaeting&#47;1_1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='sogaeting&#47;1_1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;so&#47;sogaeting&#47;1_1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1649941186699');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='1000px';vizElement.style.height='827px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='1000px';vizElement.style.height='827px';} else { vizElement.style.width='100%';vizElement.style.height='827px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>


