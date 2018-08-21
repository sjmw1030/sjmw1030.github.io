---
layout: post
title: 새로운 취미 Unity로 게임만들기
img: unity.png
---

<blockquote>
큐브로 Floor를 만들고, 캡슐을 랜덤으로 움직이는 첫번째 코딩! Transform을 직접변경해 보았습니다. 
Vector3 변수를 만들어서 z 값에만 난수를 대입해 봤습니다.그리고 Quaternion.Euler를 호출하여 x값을 랜덤으로 회전해 보았어요.
다음 번에는 tansform.Translate() 메서드를 사용하여 게임 오브젝트의 현재 위치에서 게임 오브젝트가 향한 방향을 기준으로 움직이는 코딩을 해보겠습니다.
</blockquote>

{% highlight html %}
void Update () 
{
  if (Input.GetKeyDown (KeyCode.A)) 
  {
    float rnd = Random.Range (1.5f, 2.0f);
    this.transform.position = new Vector3 (1.5f, 1.5f, rnd);
  }

  if (Input.GetKeyDown (KeyCode.B)) 
  {
    float rnd = Random.Range (0.0f, 360.0f);
    this.transform.rotation = Quaternion.Euler (rnd, 0.0f, 0.0f);
  }
}
{% endhighlight %}

|  컨텐츠명   |    내용 확인 |
|----------|-------------:|
| Unity Editor 변경하기 | <a href="http://sjmw1030.blog.me/220735857880"> 바로가기 </a> |
| Unity 내 맘대로 이동하기 | <a href="http://sjmw1030.blog.me/220735990501"> 바로가기 </a> |
| Unity, Rotate 활용 | <a href="http://sjmw1030.blog.me/220736194029"> 바로가기 </a> |
| Unity 합체 그리고 분리 ^^ | <a href="https://sjmw1030.blog.me/220736217604"> 바로가기 </a> |
| Unity 다른파일의 컴포넌트 호출하기 | <a href="https://sjmw1030.blog.me/220738151104"> 바로가기 </a> |
| Unity Prefab 코딩| <a href="http://sjmw1030.blog.me/220738345015"> 바로가기 </a> |
| Unity, Rigidbody & Collider (중력과 충돌) | <a href="http://sjmw1030.blog.me/220738356026"> 바로가기 </a> |
| Unity, Material | <a href="http://sjmw1030.blog.me/220738359918"> 바로가기 </a> |
| Unity 효과음 넣기 | <a href="https://sjmw1030.blog.me/220742117043"> 바로가기 </a> |
| Unity GUI 2D 표시하기 | <a href="https://sjmw1030.blog.me/220743062203"> 바로가기 </a> |
| Unity 타이틀 화면에서 게임화면으로 이동하기 | <a href="https://sjmw1030.blog.me/220743960775"> 바로가기 </a> |
| Unity, 부드럽게 이동하고 점프하기 | <a href="https://sjmw1030.blog.me/220745050543"> 바로가기 </a> |
| Unity 카메라 따라 다니게 하기 | <a href="https://sjmw1030.blog.me/220748038536"> 바로가기 </a> |
{: .table .table-striped .table-hover}
