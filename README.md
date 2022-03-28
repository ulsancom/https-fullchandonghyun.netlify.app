# ulsancom.github.io
@@ -1,333 +1,333 @@
<!DOCTYPE html>
<html lang="en-US">
<head>
    <meta charset="UTF-8">
    <meta content="IE=edge" http-equiv="X-UA-Compatible">
    <meta content="width=device-width, initial-scale=1" name="viewport">
    <title>최원영과 이소민의 결혼식</title>
    <meta content="최원영과 이소민의 결혼식에 와서 축하해주세요~!" name="description"/>
    <meta property="og:image" content="images/pic2.jpeg">
    <meta property="fb:app_id" content="781066922265598" />
    <meta property="fb:admins" content="Choi.Anderson"/>
    <link href="images/favicon/apple-touch-icon.png" rel="apple-touch-icon" sizes="180x180">
    <link href="images/favicon/favicon-32x32.png" rel="icon" sizes="32x32" type="image/png">
    <link href="images/favicon/favicon-16x16.png" rel="icon" sizes="16x16" type="image/png">
    <link href="https://fonts.googleapis.com/css?family=Dosis:400,500" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=Great+Vibes" rel="stylesheet">
    <link href="css/ekko-lightbox.css" rel="stylesheet">
    <link href="styles/main.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=Gamja+Flower|Gugi|Noto+Serif+KR|Stylish|Sunflower:300"
          rel="stylesheet">
    <script src="https://code.jquery.com/jquery-2.2.1.js"></script>
    <link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script src="https://cdn.emailjs.com/sdk/2.3.2/email.min.js" type="text/javascript"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/remarkable/1.7.1/remarkable.js" type="text/javascript"></script>
    <script type="text/javascript">
        function sendMail() {
            (function () {
                emailjs.init("user_yjLL5xG0A3kkOCH5BGIDh");
                emailjs.send("wedding-mail", "gift_send", {
                    name: $("#sender-name").value,
                    gift: $("#gift-name").text(),
                    message: $("#sender-message").value
                }).then(function (response) {
                    console.log("SUCCESS. status=%d, text=%s", response.status, response.text);
                }, function (err) {
                    console.log("FAILED. error=", err);
                });
            })();
        }
        function findGetParameter(parameterName) {
            var result = null,
                tmp = [];
            location.search
                .substr(1)
                .split("&")
                .forEach(function (item) {
                  tmp = item.split("=");
                  if (tmp[0] === parameterName) result = decodeURIComponent(tmp[1]);
                });
            return result;
        }
        $(document).ready(function () {
            function getText(){
                var result = null;
                $.ajax( { url: "https://raw.githubusercontent.com/AndersonChoi/wedding-card/master/README.md",
                        type: 'get',
                        dataType: 'html',
                        async: false,
                        success: function(data) { result = data; }
                    }
                );
                FileReady = true;
                return result;
            }
            var markdown_source = getText();
            var comment_contents = markdown_source.split("축하의 말")[1];
            var md = new Remarkable();
            $("#comments").append(md.render(comment_contents));
            
            if(findGetParameter('gift')=='false'){
                $('#gifts').hide();
            }
        });
    </script>
</head>
<body id="top">
<header></header>
<div id="fb-root"></div>
<script async defer crossorigin="anonymous" src="https://connect.facebook.net/ko_KR/sdk.js#xfbml=1&version=v3.2"></script>
<div class="page-content">
    <div class="div">
        <div class="ww-home-page" id="home">
            <div class="ww-wedding-announcement d-flex align-items-center justify-content-start">
                <div class="container ww-announcement-container">
                    <p class="ww-couple-name ww-title" style="font-size:4.0em">Wonyoung & Somin</p>
                    <p class="h2 mt-5 ww-title" style="font-family: 'Gugi', cursive; font-size:1.0em">
                        | WE ARE GETTING MARRIED |
                    </p>
                    <p class="h2 mt-5 ww-title"
                       style="font-family: 'Noto Serif KR', serif; font-size:1.0em; letter-spacing:-1px">
                        <b style="font-size:1.4em;">2019. 05. 18. SAT PM 02:30</b>
                        <br>부산 해운대 센텀시티 센텀사이언스파크 23층
                    </p>
                </div>
            </div>
        </div>
        <div class="ww-nav-bar sticky-top bg-light">
            <nav class="navbar navbar-expand-lg navbar-light">
                <div class="container">
                    <button aria-controls="ww-navbarNav" aria-expanded="false" aria-label="Toggle navigation"
                            class="navbar-toggler"
                            data-target="#ww-navbarNav" data-toggle="collapse" type="button">
                        <span class="navbar-toggler-icon"></span>
                    </button>
                    <div class="collapse navbar-collapse text-uppercase" id="ww-navbarNav">
                        <ul class="navbar-nav ml-auto">
                            <li class="nav-item"><a class="nav-link smooth-scroll" href="#home">Home</a></li>
                            <li class="nav-item"><a class="nav-link smooth-scroll" href="#couple">Couple</a></li>
                            <li class="nav-item"><a class="nav-link smooth-scroll" href="#events">Events</a></li>
                            <li class="nav-item"><a class="nav-link smooth-scroll" href="#gallery">Gallery</a></li>
                        </ul>
                    </div>
                </div>
            </nav>
        </div>
        <div class="ww-section" id="couple">
            <div class="container">
                <h2 class="h1 text-center pb-3 ww-title" style="font-family: 'Noto Serif KR', serif;">신랑 & 신부</h2>
                <div class="row text-center">
                    <div class="col-md-6">
                        <div class="mt-3">
                            <h3 class="h2 ww-title" style="font-family: 'Sunflower', sans-serif; font-size:1.5em">
                                이소민</h3>
                            <img alt="Groom" class="img-fluid" src="images/pic8.jpeg"/>
                        </div>
                    </div>
                    <div class="col-md-6">
                        <div class="mt-3">
                            <h3 class="h2 ww-title" style="font-family: 'Sunflower', sans-serif; font-size:1.5em">
                                최원영</h3>
                            <img alt="Bride" class="img-fluid" src="images/pic9.jpeg"/>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="ww-section bg-light" id="events">
            <div class="container ww-wedding-event">
                <h2 class="h1 text-center pb-3 ww-title" style="font-family: 'Noto Serif KR', serif;">초대합니다</h2>
                    <div class="col text-center mb-5">
                        <h6 style="font-family: 'Noto Serif KR', serif;">
                            1463<br>
                            (만난지 4년+1일 되는날 결혼 = 1463일)
                        </h6>
                    </div>
                <div class="row">
                    <div class="col-md-7 col-sm-12">
                        <div class="my-3">
                            <div class="h4">웨딩 본식</div>
                            <ul>
                                <li>
                                    <i class="text-muted fas fa-map-marker-alt"></i>
                                    <span class="pl-2 text-muted">부산 해운대 우동 센텀사이언스 파크 23층</span>
                                </li>
                                <li class="pt-2">
                                    <i class="text-muted far fa-calendar-alt"></i>
                                    <span class="pl-2 text-muted">2019년 5월 18일, 2:30PM</span>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-md-5 col-sm-12">
                        <div class="my-3">
                            <img alt="Wedding Party" class="img-fluid" src="images/wedding-party.jpg"/>
                        </div>
                    </div>
                </div>
                <div class="row">
                    <div class="col-md-7 col-sm-12">
                        <div class="my-3">
                            <div class="h4">식사</div>
                            <ul>
                                <li>
                                    <i class="text-muted fas fa-map-marker-alt "></i>
                                    <span class="pl-2 text-muted">부산 해운대 우동 센텀사이언스 파크 지하 1층 더파티 센텀점</span>
                                </li>
                                <li class="pt-2">
                                    <i class="text-muted far fa-calendar-alt "></i>
                                    <span class="pl-2 text-muted">2019년 5월 18일, 2:30PM - 4:30PM</span>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-md-5 col-sm-12">
                        <div class="my-3"><img alt="Reception" class="img-fluid" src="images/reception.jpg"/></div>
                    </div>
                </div>
            </div>
        </div>
        <div class="ww-section" id="gallery">
            <div class="ww-photo-gallery">
                <div class="container">
                    <h2 class="h1 text-center pb-3 ww-title" style="font-family: 'Noto Serif KR', serif;">포토 갤러리</h2>
                    <div class="ww-gallery">
                        <div class="card-columns">
                            <div class="card" data-groups="[&quot;party&quot;,&quot;wedding&quot;]">
                                <a data-gallery="ww-gallery" data-toggle="lightbox">
                                    <img alt="Gallery Pic 2" class="img-fluid" src="images/pic2.jpeg"/>
                                </a>
                            </div>
                            <div class="card" data-groups="[&quot;vacation&quot;]">
                                <a data-gallery="ww-gallery" data-toggle="lightbox">
                                    <img alt="Gallery Pic 3" class="img-fluid" src="images/pic3.jpeg"/>
                                </a>
                            </div>
                            <div class="card" data-groups="[&quot;party&quot;,&quot;vacation&quot;]">
                                <a data-gallery="ww-gallery" data-toggle="lightbox">
                                    <img alt="Gallery Pic 4" class="img-fluid" src="images/pic4.jpeg"/>
                                </a>
                            </div>
                            <div class="card" data-groups="[&quot;vacation&quot;]">
                                <a data-gallery="ww-gallery" data-toggle="lightbox">
                                    <img alt="Gallery Pic 5" class="img-fluid" src="images/pic6.jpeg"/>
                                </a>
                            </div>
                            <div class="card"
                                 data-groups="[&quot;wedding&quot;,&quot;ceremony&quot;,&quot;party&quot;]">
                                <a data-gallery="ww-gallery" data-toggle="lightbox">
                                    <img alt="Gallery Pic 6" class="img-fluid" src="images/pic7.jpeg"/>
                                </a>
                            </div>
                            <div class="card" data-groups="[&quot;vacation&quot;]">
                                <a data-gallery="ww-gallery" data-toggle="lightbox">
                                    <img alt="Gallery Pic 7" class="img-fluid" src="images/pic5.jpeg"/>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
       <div class="ww-section parallax-window  text-white" data-parallax="scroll" data-image-src="images/gift/gift-background.jpg" id="gifts">
            <div class="ww-gift-section">
                <div class="container">
                    <h2 class="h1 text-center pb-3 ww-title" style="font-family: 'Noto Serif KR', serif;">Gift for our
                        wedding</h2>
                    <div class="col text-center mb-5">
                        <h6 style="font-family: 'Noto Serif KR', serif;">
                            저희 부부가 앞으로 살아나갈 일상에<br>
                            오래도록 특별한 기억을 선물하고 싶으신가요?<br>
                            그렇다면 고민하는 대신 아래 목록을 참고해 주세요.<br>
                            저희가 필요로 하는 물건들을 정리해 두었습니다.<br>
                            애정어린 마음으로 보내주신 선물은<br>
                            가까이 두어 오래도록 아껴 쓰고,<br>
                            소중하게 간직하겠습니다.
                            <br><br>
                            (아래 선물버튼을 눌러 신랑, 신부에게 예약메시지를 보내세요!)
                        </h6>
                    </div>
                    <div class="ww-gift">
                        <div class="gift-columns">
                            <div class="gift">
                                <img alt="와인셀러" class="img-fluid gift-img gift-selected" src="images/gift/wineceller.png"/>
                                <div class="btn-group gift-btn-group" role="group">
                                    <button class="btn btn-default gift-btn"
                                            onclick="window.open('https://smartstore.naver.com/dhk00840/products/4311205513')">
                                        <i class="fa fa-search"></i></button>
                                    <button class="btn btn-default gift-btn gift-send" data-name="와인셀러"
                                            onclick="alert('다른분에게 예약된 선물입니다.');"><i
                                            class="fa fa-gift"></i></button>
                                </div>
                            </div>
                            <div class="gift">
                                <img alt="전동클렌저" class="img-fluid gift-img gift-selected"
                                     src="images/gift/philips_clenser.png"/>
                                <div class="btn-group gift-btn-group" role="group">
                                    <button class="btn btn-default gift-btn"
                                            onclick="window.open('https://www.philips.co.kr/c-p/BSC111_06/visapure-mini-facial-cleanser')">
                                        <i class="fa fa-search"></i></button>
                                    <button class="btn btn-default gift-btn gift-send" data-name="전동클렌저"
                                            onclick="alert('다른분에게 예약된 선물입니다.');"><i
                                            class="fa fa-gift"></i></button>
                                </div>
                            </div>
                            <div class="gift">
                                <img alt="드라이기" class="img-fluid gift-img gift-selected" src="images/gift/dyson.png"/>
                                <div class="btn-group gift-btn-group" role="group">
                                    <button class="btn btn-default gift-btn"
                                            onclick="window.open('https://www.kr.dyson.com/products/hair-care/dyson-supersonic-hair-dryer')">
                                        <i class="fa fa-search"></i></button>
                                    <button  class="btn btn-default gift-btn gift-send" data-name="드라이기"
                                             onclick="alert('다른분에게 예약된 선물입니다.');"><i
                                            class="fa fa-gift"></i></button>
                                </div>
                            </div>
                            <div class="gift">
                                <img alt="믹서기" class="img-fluid gift-img gift-selected" src="images/gift/blender.png"/>
                                <div class="btn-group gift-btn-group" role="group">
                                    <button class="btn btn-default gift-btn"
                                            onclick="window.open('http://jenniferoom.co.kr/product/detail.html?product_no=85&cate_no=24&display_group=1')">
                                        <i class="fa fa-search"></i></button>
                                    <button  class="btn btn-default gift-btn gift-send" data-name="믹서기"
                                             onclick="alert('다른분에게 예약된 선물입니다.');"><i
                                            class="fa fa-gift"></i></button>
                                  
