# CSS3-Doraemon
DIV+CSS3实现的大雄和哆啦A梦（没有图片）
<!DOCTYPE html>
<html>
<head lang="en">
    <meta charset="UTF-8">
    <title>Doraemon</title>
    <style>
       #main{
    width:800px;
    height:600px;
    margin:50px auto;
    padding:50px 100px;
    background:#70E3FD;
}
.content-left,.content-right{
    float:left;
    overflow:hidden;
    position: relative;
    padding:10px 50px;
    height:600px;
    width:200px;
}
.content-left{
    margin-left:50px;
}
.content-right{
    padding: 0 100px;
    width:300px;
    margin-left:-90px;
    margin-top:25px;
}
.head{
    position:relative;
    left:40px;
    float:left;
    width:130px;
    height:160px;
    border:2px solid black;
    -webkit-border-radius:60px;
    -moz-border-radius:60px;
    border-radius: 60px;
    position:relative;
    z-index:30;
    background:#fadbc6;
}
.hair1{
    position: absolute;
    top:-1px;
    left:0;
    z-index:5;
    width:130px;
    height:60px;
    background:black;
    -webkit-border-radius:45px 45px 5px 0;
    -moz-border-radius:45px 45px 5px 0;
    border-radius:45px 45px 5px 0;
}
.hair1>span:last-child,
.hair1>span:first-child{
    position:absolute;
    width:20px;
    height:20px;
    -webkit-border-radius:20px 0px 20px 0;
    -moz-border-radius:20px 0px 20px 0;
    border-radius: 20px 0px 20px 0;

}
.hair1>span:first-child{
    top:20px;
    left:112px;
    border-top:1px solid black;
    border-left:1px solid black;
    -webkit-transform: rotate(30deg) ;
    -moz-transform: rotate(30deg);
    -ms-transform: rotate(30deg);
    -o-transform: rotate(30deg);
    transform:rotate(30deg) ;
}
.hair1>span:last-child{
    top:12px;
    left:105px;
    border-bottom:1px solid black;
    border-right:1px solid black;
    -webkit-transform: rotate(-10deg) ;
    -moz-transform: rotate(-10deg);
    -ms-transform: rotate(-10deg);
    -o-transform: rotate(-10deg);
    transform:rotate(-10deg) ;
}
.hair2{
    position: absolute;
    top:38px;
    left:0;
    z-index:10;
    width:130px;
    height:40px;
    background:#fadbc6;
    -webkit-border-radius:50%;
    -moz-border-radius: 50%;
    border-radius:50%;
}
.face{
    z-index:20;
    position:absolute;
    top:53px;
    left:0;
    width:120px;
    height:90px;
    -webkit-border-radius:0 0 60px 60px;
    -moz-border-radius: 0 0 60px 60px;
    border-radius: 0 0 60px 60px;
}
.hair2>span:first-child,
.hair2>span:last-child{
    position:absolute;
    width:40px;
    -webkit-border-radius:50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
}
.hair2>span:first-child{
    top:9px;
    left:15px;
    border-top: 2px solid black;
    border-left: 2px solid black;
    -webkit-transform: rotate(-16deg);
    -moz-transform: rotate(-16deg);
    -ms-transform: rotate(-16deg);
    -o-transform: rotate(-16deg);
    transform: rotate(-16deg);
}
.hair2>span:last-child{
    top:10px;
    left:80px;
    border-top: 2px solid black;
    border-left: 2px solid black;
    -webkit-transform: rotate(20deg);
    -moz-transform: rotate(20deg);
    -ms-transform: rotate(20deg);
    -o-transform: rotate(20deg);
    transform: rotate(20deg);
}
.left-eye,
.right-eye{
    position: absolute;
    top:0;
    width:50px;
    height:60px;
    -webkit-border-radius:50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    background: #fff;
    border:1px solid black;
}
.left-eye{
    left:12px;
}
.right-eye{
    right:4px;
}
.left-eye-blackball,
.right-eye-blackball{
    position: absolute;
    top:21px;
    width:12px;
    height:18px;
    background:black;
    -webkit-border-radius:50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
}
.left-eye-blackball{
    right:6px;
}
.right-eye-blackball{
    left:6px;
    top:21px;
}
.right-eye-ball,
.left-eye-ball{
    position: absolute;
    top:6px;
    width:4px;
    height:6px;
    background:#fff;
    -webkit-border-radius:50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
}
.left-eye-ball{
    right:3px;
}
.right-eye-ball{
    left:3px;
}
.nose{
    position:absolute;
    bottom:32px;
    left:57px;
    width:12px;
    height:9px;
    background:transparent;
    -webkit-border-radius:50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    border:1px solid black;
}
.mouth{
    position:absolute;
    bottom:10px;
    left:35px;
    width:59px;
    height:27px;
    background:transparent;
    -webkit-border-radius:50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    border-bottom:3px solid black;
    border-top:none;
}
.left-ear,
.right-ear{
    position:absolute;
    top:82px;
    right:60px;
    z-index:10;
    border:1px solid black;
    width:20px;
    height:40px;
    -webkit-border-radius:50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    background:#fadbc6;
}
.left-ear{
    left:76px;
    -webkit-transform: rotate(-15deg);
    -moz-transform: rotate(-15deg);
    -ms-transform: rotate(-15deg);
    -o-transform: rotate(-15deg);
    transform: rotate(-15deg);
}
.right-ear{
    right:60px;
    -webkit-transform: rotate(15deg);
    -moz-transform: rotate(15deg);
    -ms-transform: rotate(15deg);
    -o-transform: rotate(15deg);
    transform: rotate(15deg);
}
.left-ear>span:first-child,
.left-ear>span:last-child{
    border:1px solid black;
    width:5px;
    position:relative;
    top:13px;
    left:5px;
}
.left-ear>span:first-child{
    width:8px;
    top:7px;
    left:8px;
}
.left-ear>span:last-child{
    width:5px;
    top:13px;
    left:5px;
}
.right-ear>span:first-child,
.right-ear>span:last-child{
    border:1px solid black;
    position:relative;
    left:8px;
}
.right-ear>span:first-child{
    width:8px;
    top:7px;
}
.right-ear>span:last-child{
    width:5px;
    top:13px;
}
.neck{
    position:absolute;
    top:-10px;
    left:82px;
    width:45px;
    height:15px;
    border-radius:50%;
    border:1px solid black;
    background:#fadbc6;
    z-index:40;
}
.part-body{
    position: relative;
    margin-top:162px;
    z-index:10;
}
.tripe{
    position: absolute;
    top:0;
    left:55px;;
    width:100px;
    height:120px;
    background:#AF0819;
    border:2px solid black;
    -webkit-border-radius:12px 12px 8px 8px;
    -moz-border-radius: 12px 12px 8px 8px;
    border-radius: 12px 12px 8px 8px;
    z-index:20;
}
.right-neckline,
.left-neckline{
    position: absolute;
    width:20px;
    height:35px;
    background:#fff;
    border:2px solid black;
}
.left-neckline{
    position: absolute;
    top:-11px;
    left:20px;
    -webkit-transform: rotate(80deg) skew(30deg);
    -moz-transform: rotate(80deg) skew(30deg);
    -ms-transform: rotate(80deg) skew(30deg);
    -o-transform: rotate(80deg) skew(30deg);
    transform: rotate(80deg) skew(30deg);
}
.right-neckline{
    top:-10px;
    right:20px;;
    -webkit-transform: rotate(-15deg) skew(30deg);
    -moz-transform: rotate(-15deg) skew(30deg);
    -ms-transform: rotate(-15deg) skew(30deg);
    -o-transform: rotate(-15deg) skew(30deg);
    transform: rotate(-15deg) skew(30deg);
}
.left-leg,
.right-leg{
    position: absolute;
    top:0;
    width:31px;
    height:140px;
    background:#AF0819;
    border:2px solid black;
    -webkit-border-radius:10px 10px 5px 5px;
    -moz-border-radius: 10px 10px 5px 5px;
    border-radius: 10px 10px 5px 5px;
    z-index:0;
}
.left-leg{
    left:26px;
    -webkit-transform: rotate(25deg);
    -moz-transform: rotate(25deg);
    -ms-transform: rotate(25deg);
    -o-transform: rotate(25deg);
    transform: rotate(25deg);
}
.right-leg{
    right:13px;
    -webkit-transform: rotate(-25deg);
    -moz-transform: rotate(-25deg);
    -ms-transform: rotate(-25deg);
    -o-transform: rotate(-25deg);
    transform: rotate(-25deg);
}
.right-hand,.left-hand{
    position:relative;
}
.left-hand>div:first-child,
.right-hand>div:first-child{
    position: absolute;
    top:130px;
    width:28px;
    height:50px;
    border:2px solid black;
    background:#FADBC6;
    z-index:20;
}
.left-hand>div:first-child{
    left:-17px;
    border-right:none;
    -webkit-border-radius: 12px 5px 13px 25px;
    -moz-border-radius: 12px 5px 13px 25px;
    border-radius: 12px 5px 13px 25px;
    -webkit-transform: rotate(25deg);
    -moz-transform: rotate(25deg);
    -ms-transform: rotate(25deg);
    -o-transform: rotate(25deg);
    transform: rotate(25deg);
}
.right-hand>div:first-child{
    right:-30px;
    border-left:none;
    -webkit-border-radius: 5px 12px 25px 13px;
    -moz-border-radius: 5px 12px 25px 13px;
    border-radius: 5px 12px 25px 13px;
    -webkit-transform: rotate(-25deg);
    -moz-transform: rotate(-25deg);
    -ms-transform: rotate(-25deg);
    -o-transform: rotate(-25deg);
    transform: rotate(-25deg);
}
.left-hand>div:first-child span{
    position: absolute;
    width:7px;
    height:14px;
    border-right:2px solid black;
}
.left-hand>div:first-child span:first-child{
    bottom:5px;
    left:-3px;
}
.left-hand>div:first-child span:nth-child(2){
    height:20px;
    bottom:0;
    left:3px;
}
.left-hand>div:first-child span:nth-child(3){
    height:25px;
    bottom:0px;
    left:10px;
}
.left-hand>div:first-child span:nth-child(4){
    height:30px;
    bottom:2px;
    left:19px;
}
.right-hand>div:first-child span{
    position: absolute;
    width:7px;
    border-left:2px solid black;
}
.right-hand>div:first-child span:first-child{
    height:30px;
    bottom:2px;
    left:0px;
}
.right-hand>div:first-child span:nth-child(2){
    height:25px;
    bottom:0px;
    left:7px;
}
.right-hand>div:first-child span:nth-child(3){
    height:20px;
    bottom:0;
    left:14px;
}
.right-hand>div:first-child span:nth-child(4){
    height:14px;
    bottom:5px;
    left:21px;
}
.right-big-finger,
.big-finger{
    position: absolute;
    bottom:-183px;
    width:7px;
    height:40px;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    border:2px solid black;
    background:#FADBC6;
    z-index:5;
}
.big-finger{
    left:10px;
    -webkit-transform: rotate(17deg);
    -moz-transform: rotate(17deg);
    -ms-transform: rotate(17deg);
    -o-transform: rotate(17deg);
    transform: rotate(17deg);
    background:#FADBC6;
}
.right-big-finger{
    right:-3px;
    -webkit-transform: rotate(-17deg);
    -moz-transform: rotate(-17deg);
    -ms-transform: rotate(-17deg);
    -o-transform: rotate(-17deg);
    transform: rotate(-17deg);
    background:#FADBC6;
}
.shorts{
    position: absolute;
    top:120px;
    left:55px;
    width:100px;
    height:50px;
    background:#00417D;
    border:2px solid black;
    -webkit-border-radius: 5px 5px 10px 10px;
    -moz-border-radius: 5px 5px 10px 10px;
    border-radius: 5px 5px 10px 10px;
}
.shorts>span{
    position: absolute;
    bottom:0;
    left:0;
    width:50px;
    height:15px;
    border-right:2px solid black;
}
.leg1{
    position: relative;
    width:100%;
    left:55px;
    top:334px;
}
.left-leg1,
.right-leg1{
    position: absolute;
    bottom:-9px;
    width:40px;
    height:170px;
    background:#fff;
    border:2px solid black;
    border-bottom: none;
    z-index:20;
}
.right-leg1{
    right:103px;
}
.left-leg1{
    left:8px;
}
.left-leg1>div:first-child,
.right-leg1>div:first-child{
    position: absolute;
    top:0;
    left:0;
    width:40px;
    height:100px;
    background:#FADBC6;
    border-bottom:2px solid black;
    -webkit-border-radius: 0 0 3px 3px;
    -moz-border-radius: 0 0 3px 3px;
    border-radius: 0 0 3px 3px;
}
.foot-left,.foot-right{
    position: absolute;
    bottom:-43px;
    width:40px;
    height:60px;
    background:#fff;
    border-bottom:2px solid black;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
}
.foot-left{
    left:3px;
    z-index:30;
    -webkit-transform: rotate(50deg);
    -moz-transform: rotate(50deg);
    -ms-transform: rotate(50deg);
    -o-transform: rotate(50deg);
    transform: rotate(50deg);
}
.foot-right{
    right:98px;
    z-index:40;
    -webkit-transform: rotate(-50deg);
    -moz-transform: rotate(-50deg);
    -ms-transform: rotate(-50deg);
    -o-transform: rotate(-50deg);
    transform: rotate(-50deg);
}
.foot-right-shoe,
.foot-left-shoe{
    position: absolute;
    bottom:-65px;
    width:70px;
    height:80px;
    background:#00417D;
    border-bottom:2px solid black;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    z-index:10;
}
.foot-left-shoe{
    left: -22px;
    -webkit-transform: rotate(76deg);
    -moz-transform: rotate(76deg);
    -ms-transform: rotate(76deg);
    -o-transform: rotate(76deg);
    transform: rotate(76deg);
}

.foot-right-shoe{
    right: 77px;
    -webkit-transform: rotate(-76deg);
    -moz-transform: rotate(-76deg);
    -ms-transform: rotate(-76deg);
    -o-transform: rotate(-76deg);
    transform: rotate(-76deg);
}
.foot-left-shoe1,.foot-right-shoe1 {
    position: absolute;
    bottom:-71px;
    width:70px;
    height:85px;
    background:#fff;
    border-bottom:2px solid black;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    z-index:5;
}
.foot-left-shoe1{
    left: -22px;
    -webkit-transform: rotate(76deg);
    -moz-transform: rotate(76deg);
    -ms-transform: rotate(76deg);
    -o-transform: rotate(76deg);
    transform: rotate(76deg);
}
.foot-right-shoe1{
    right: 77px;
    -webkit-transform: rotate(-76deg);
    -moz-transform: rotate(-76deg);
    -ms-transform: rotate(-76deg);
    -o-transform: rotate(-76deg);
    transform: rotate(-76deg);
}
.a-head{
    position:relative ;
    margin-top:120px;
    width:274px;
    height:250px;
    border:2px solid black;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    background: #0298D7;

}
.a-face{
    width:245px;
    height:210px;
    border:2px solid black;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    margin-top:40px;
    z-index:0;
    background: #fff;
    position: relative;
    left:12px;
}
.a-right-eye,.a-left-eye{
    position: absolute;
    top:0;
    width:54px;
    height:64px;
    border:2px solid black;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    background: #fff;
}
.a-left-eye{
    left:79px;
}
.a-right-eye{
    right:79px;
}
.a-right-blackball,.a-left-blackball{
    position: absolute;
    top:20px;
    width:20px;
    height:25px;
    background: black;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
}
.a-left-blackball{
    right:5px;
}
.a-right-blackball{
    left:5px;
}
.a-right-ball,.a-left-ball{
    position: absolute;
    top:6px;
    width:10px;
    height:13px;
    background: #fff;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    z-index:10;
}
.a-left-ball{
    right:3px;
}
.a-right-ball{
    left:3px;
}
.a-nose{
    position: absolute;
    top:13px;
    left:104px;
    width:32px;
    height:32px;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    border:2px solid black;
    background:#AD1118;
    z-index:30;
}
.empty-nose{
    position: absolute;
    top:7px;
    left:8px;
    width:13px;
    height:13px;
    background: #fff;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
}
.a-lip-right,
.a-lip-left{
    position: absolute;
    top:39px;
    width:65px;
    height:58px;
    border:2px solid black;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    z-index:10;
    background: #fff;
    z-index:10;
}
.a-lip-middle{
    position: absolute;
    left:20px;
    bottom:83px;
    width:200px;
    height:40px;
    background: #fff;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    z-index:10;
    background:#AD0C11;
}
.a-lip-left{
    left:-10px;
}
.a-lip-right{
    right:-10px;
}
.a-mustache-left,
.a-mustache-right{
    position: absolute;
    top:42px;
    width:48px;
    height:46px;
    border:2px solid transparent;
    z-index:20;
    background: #fff;
    -webkit-border-radius: 5px;
    -moz-border-radius: 5px;
    border-radius: 5px;
}
.a-mustache-left{
    left:30px;
    -webkit-transform: rotate(-12deg);
    -moz-transform: rotate(-12deg);
    -ms-transform: rotate(-12deg);
    -o-transform: rotate(-12deg);
    transform: rotate(-12deg);
}
.a-mustache-right{
    right:30px;
    -webkit-transform: rotate(12deg);
    -moz-transform: rotate(12deg);
    -ms-transform: rotate(12deg);
    -o-transform: rotate(12deg);
    transform: rotate(12deg);
}
.a-mustache-right>span:first-child,
.a-mustache-right>span:nth-child(2),
.a-mustache-right>span:nth-child(3),
.a-mustache-left>span:first-child,
.a-mustache-left>span:nth-child(2),
.a-mustache-left>span:nth-child(3){
    position:absolute;
    width:50px;
    border:2px solid black;
}
.a-mustache-right>span:first-child,
.a-mustache-right>span:nth-child(2),
.a-mustache-right>span:nth-child(3){
    right:0;
    left:0;
}
.a-mustache-left>span:first-child{
    right:-15px;
    top:-5px;
    -webkit-transform: rotate(22deg);
    -moz-transform: rotate(22deg);
    -ms-transform: rotate(22deg);
    -o-transform: rotate(22deg);
    transform: rotate(22deg);
}
.a-mustache-left>span:nth-child(2){
    right:-10px;
    top:10px;
    -webkit-transform: rotate(12deg);
    -moz-transform: rotate(12deg);
    -ms-transform: rotate(12deg);
    -o-transform: rotate(12deg);
    transform: rotate(12deg);
}
.a-mustache-left>span:nth-child(3){
    right:-10px;
    top:25px;
}
.a-mustache-right>span:first-child{
    left:-15px;
    top:-5px;
    -webkit-transform: rotate(-22deg);
    -moz-transform: rotate(-22deg);
    -ms-transform: rotate(-22deg);
    -o-transform: rotate(-22deg);
    transform: rotate(-22deg);
}
.a-mustache-right>span:nth-child(2){
    top:10px;
    left:-10px;
    -webkit-transform: rotate(-12deg);
    -moz-transform: rotate(-12deg);
    -ms-transform: rotate(-12deg);
    -o-transform: rotate(-12deg);
    transform: rotate(-12deg);
}
.a-mustache-right>span:nth-child(3){
    left:-10px;
    top:25px;
}
.groove{
    position: absolute;
    top:40px;
    left:119px;
    width:0px;
    height:46px;
    border:2px solid black;
}
.a-mouth{
    position: absolute;
    left:20px;
    bottom:24px;
    width:200px;
    height:84px;
    border:2px solid black;
    -webkit-border-radius: 10px 10px 100px 100px ;
    -moz-border-radius: 10px 10px 100px 100px ;
    border-radius: 10px 10px 100px 100px ;
    background:#AD0C11;
}
.a-tongue{
    position: absolute;
    bottom:-3px;
    width:150px;
    height:52px;
    border:2px solid black;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    left:24px;
    background: #CC300C;
}
.a-body{
    position: relative;
    left:40px;
    width:190px;
    height:150px;
    border:2px solid black;
    background:#0190C9;
    -webkit-border-radius: 20px 20px 5px 5px;
    -moz-border-radius: 20px 20px 5px 5px;
    border-radius: 20px 20px 5px 5px;
    z-index:10;
}
.a-neck{
    position:absolute;
    top:-20px;
    left:10px;
    width:170px;
    height:16px;
    border:2px solid black;
    background:#AA100D;
    -webkit-border-radius: 10px;
    -moz-border-radius: 10px;
    border-radius: 10px;
    z-index:10;
}
.a-bell{
    position:absolute;
    top:5px;
    left:60px;
    width:46px;
    height:46px;
    border:2px solid black;
    background:#D8B719;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    z-index:20;
}
.a-bell>span:first-child{
    position:absolute;
    top:15px;
    left:0;
    width:44px;
    height:3px;
    border:2px solid black;
    -webkit-border-radius: 7px;
    -moz-border-radius: 7px;
    border-radius: 7px;
}
.a-bell>span:nth-child(2){
    position:absolute;
    top:25px;
    left:19px;
    width:8px;
    height:8px;
    border:2px solid black;
    background: #57514B;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
}
.a-bell>span:nth-child(3){
    position:absolute;
    top:35px;
    left:24px;
    height:13px;
    border-left:2px solid black;
}
.pocket{
    position: absolute;
    left:20px;
    top:-10px;
    width:150px;
    height:110px;
    border:2px solid black;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    background:#fff;
    z-index:0;
}
.pocket>span{
    position: absolute;
    left:20px;
    bottom:10px;
    width:110px;
    height:44px;
    border:2px solid black;
    -webkit-border-radius:0 0 50% 50%;
    -moz-border-radius:0 0 50% 50%;
    border-radius:0 0 50% 50%;
}
.a-middle{
    position: absolute;
    left:71px;
    bottom:-18px;
    width:40px;
    height:36px;
    border:2px solid black;
    border-bottom:none;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    background: #70E3FD;
}
.a-middle-up{
    position: absolute;
    left:113px;
    bottom:18px;
    width:40px;
    height:30px;
    background: #70E3FD;
    -webkit-border-radius: 40%;
    -moz-border-radius: 40%;
    border-radius: 40%;
    z-index:10;
}
.a-leg{
    width:150px;
    height:40px;
    position: relative;
}
.a-right-leg,
.a-left-leg{
    position: absolute;
    bottom: 8px;
    width:96px;
    height:60px;
    border:2px solid black;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    background: #fff;
}
.a-left-leg{
    left:15px;
}
.a-right-leg{
    right:-101px;
}
.a-right-side,
.a-left-side{
    position: absolute;
    bottom:200px;
    width:104px;
    height:140px;
    z-index:0;
}
.a-left-side{
    left:42px;
}
.a-right-side{
    right:62px;
}
.a-right-hand,
.a-left-hand{
    position: absolute;
    top:10px;
    width:64px;
    height:64px;
    border:2px solid black;
    background: #fff;
    -webkit-border-radius: 50%;
    -moz-border-radius: 50%;
    border-radius: 50%;
    z-index:30;
}
.a-left-hand{
    left:-22px;
}
.a-right-hand{
    right:-22px;
}
.a-right-leg1,
.a-left-leg1{
    position: absolute;
    bottom:-3px;
    width:40px;
    height:110px;
    border:2px solid black;
    background: #0190C9;
    -webkit-border-radius: 10px;
    -moz-border-radius: 10px;
    border-radius: 10px;
    z-index:20;
}
.a-left-leg1{
    left:50px;
    -webkit-transform: rotate(-55deg);
    -moz-transform: rotate(-55deg);
    -ms-transform: rotate(-55deg);
    -o-transform: rotate(-55deg);
    transform: rotate(-55deg);
}
.a-right-leg1{
    right:50px;
    -webkit-transform: rotate(56deg);
    -moz-transform: rotate(56deg);
    -ms-transform: rotate(56deg);
    -o-transform: rotate(56deg);
    transform: rotate(56deg);
    bottom:-2px;
}
    </style>
</head>
<body>
    <div id="main">
        <div class="content-left">
            <div class="left-ear">
                <span></span>
                <span></span>
            </div>
            <div class="right-ear">
                <span></span>
                <span></span>
            </div>
            <div class="head">
               <div class="hair1">
                   <span></span>
                   <span></span>
               </div>
                <div class="hair2">
                    <span></span>
                    <span></span>
                </div>
                <div class="face">
                    <div class="left-eye">
                        <div class="left-eye-blackball">
                            <div class="left-eye-ball"></div>
                        </div>
                    </div>
                    <div class="right-eye">
                        <div class="right-eye-blackball">
                            <div class="right-eye-ball"></div>
                        </div>
                    </div>
                    <div class="nose"></div>
                    <div class="mouth"></div>
                </div>
            </div>
            <div class="part-body">
                <div class="neck"></div>
                <div class="tripe">
                    <div class="left-neckline"></div>
                    <div class="right-neckline"></div>
                </div>
                <div class="shorts">
                    <span></span>
                </div>
                <div class="left-leg"></div>
                <div class="right-leg"></div>
            </div>
            <div class="leg1">
                <div class="left-leg1">
                    <div></div>
                </div>
                <div class="right-leg1">
                    <div></div>
                </div>
                <div class="foot-left"></div>
                <div class="foot-left-shoe"></div>
                <div class="foot-left-shoe1"></div>
                <div class="foot-right"></div>
                <div class="foot-right-shoe"></div>
                <div class="foot-right-shoe1"></div>
            </div>
            <div class="left-hand">
                <div>
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                </div>
                <div class="big-finger"></div>
            </div>
            <div class="right-hand">
                <div>
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                </div>
                <div class="right-big-finger"></div>
            </div>
        </div>
        <div class="content-right">
            <div class="a-head">
                <div class="a-face">
                    <div class="a-nose">
                        <div class="empty-nose"></div>
                    </div>
                    <div class="a-lip-left"></div>
                    <div class="a-lip-middle"></div>
                    <div class="a-mustache-left">
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>
                    <div class="groove"></div>
                    <div class="a-lip-right"></div>
                    <div class="a-mustache-right">
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>
                    <div class="a-mouth">
                        <div class="a-tongue"></div>
                    </div>
                </div>
                <div class="a-left-eye">
                    <div class="a-left-blackball">
                        <div class="a-left-ball"></div>
                    </div>
                </div>
                <div class="a-right-eye">
                    <div class="a-right-blackball">
                        <div class="a-right-ball"></div>
                    </div>
                </div>
            </div>
            <div class="a-body">
                <div class="a-neck">
                    <div class="a-bell">
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>
                </div>
                <div class="pocket">
                    <span></span>
                </div>
                <div class="a-middle"></div>
            </div>
            <div class="a-left-side">
                <span class="a-left-hand"></span>
                 <span class="a-left-leg1"></span>
            </div>
            <div class="a-right-side">
                <span class="a-right-hand"></span>
                <span class="a-right-leg1"></span>
            </div>
            <div class="a-leg">
                <span class="a-left-leg"></span>
                <span class="a-middle-up"></span>
                <span class="a-right-leg"></span>
            </div>
        </div>
    </div>
</body>
</html>
