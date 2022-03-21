<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>최진호 - STARBUCKS</title>
    <link rel="stylesheet" href="./css/style.css">
    <link rel="shoutcut icon" href="./images/fv.png">
    <script src="./script/jquery-1.12.3.js"></script>
    <script src="https://kit.fontawesome.com/2d323a629b.js" crossorigin="anonymous"></script>
    <script>
        /* $(function(){
            $("#menubtn").click(function(){
                $("#menu").slideToggle();
            });
        });
        */
       $(function(){
           var $btnGnb = $('.menubtn');
           var $nav = $('#menu');
           $btnGnb.on('click', function(){
               $nav.slideToggle();
           }); //모바일 메뉴 클릭 이벤트
           $(window).on('load resize', function(){
               if ($(this).width() > 768) { //pc모드
                   $nav.show();
               } else { // mobile모드
                   $btnGnb.removeClass('.menubtn').next().hide();
               }
           });
       });
    //    .slideToggle(); - 선택한 요소가 보여지면 숨겨주고, 숨겨져 있으면 보여줌. (점차 접히고 펼쳐지는 구조)
    </script>
</head>
<body>
    <div id="wrap">
        <header>
            <div class="header_box">
                <div class="header_inner">
                    <h1 class="logo"><a href="./index.html"><img src="./images/logo.png" alt="로고"></a></h1>
                    <div class="menus">
                        <a href="#" class="menubtn"><i class="fas fa-bars"></i></a>
                        <nav id="menu">
                            <ul>
                                <li><a href="#">ABOUT</a></li>
                                <li><a href="#">MENU</a></li>
                                <li><a href="#">STORE</a></li>
                                <li><a href="#">COFFEE</a></li>
                                <li><a href="#">NEWS</a></li>
                            </ul>
                        </nav>
                    </div>
                </div>
            </div>
        </header>
        <div id="center">
            <div class="slide">
               <a href="#"><img src="./images/main_img.jpg" alt="메인이미지" class="topimg"></a>
               <p class="text"> Starbucks </p>
           </div>
            <div class="con">
                <div class="con1">
                    <div class="summary">
                        <a href="#">
                            <i class="thum1"></i>
                            <h2>스타벅스의 '콜롬비아 원두'</h2>
                            <p>자세히보기</p>
                        </a>
                    </div>
                </div>
                <div class="con2">
                    <div class="summary">
                        <a href="#">
                            <i class="thum2"></i>
                            <h2>스타벅스의 코리아만의 특별한 혜택</h2>
                            <p>자세히보기</p>
                        </a>
                    </div>
                </div>
                <div class="con3">
                    <div class="summary">
                        <a href="#">
                            <i class="thum3"></i>
                            <h2>크리스마스 신메뉴 출시!</h2>
                            <p>자세히보기</p>
                        </a>
                    </div>
                </div>
            </div>
            <div class="info">
                <div class="info_inner">
                    <div class="notice">
                        <h3>공지사항</h3>
                        <ul>
                            <li>
                                <a href="#">
                                    <span>스타벅스의 특별한 리워드</span>
                                    <span class="time">22-03-17</span>
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <span>기프트카드 빅이벤트!!</span>
                                    <span class="time">22-03-17</span>
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <span>스타벅스 블렌드 만나기!</span>
                                    <span class="time">22-03-17</span>
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <span>스타벅스 웰페이퍼 다운</span>
                                    <span class="time">22-03-17</span>
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="sns">
                    <div class="follow">
                        <p class="follow-info">최신정보를 여기서도 다운받으세요</p>
                        <ul>
                            <li><a href="#" class="twitter">Twitter</a></li>
                            <li><a href="#" class="facebook">Facebook</a></li>
                            <li><a href="#" class="google">Google+</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <footer>
            <div class="copyright">
                <p>(주) 스타벅스코리아 대표 : 송데이비드호섭 <br/>
                &copy;2022
                <strong>
                    <a href="mailto:starbucks@starbucks.co.kr">Starbucks Coffee Company.</a>
                </strong>
                All Rights Reserved.
                </p>
            </div>
        </footer>
    </div>
</body>
</html>
