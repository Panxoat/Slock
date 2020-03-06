<template>
    <div id = "grid">
        <div class = "login_grid">
            <div>
                <img src="../assets/ico.png" width="10%">
                <p class = "slock">SLOCK.</p>
                <p class = "infoSlock">새로운 기숙사 문관리 시스템</p>
            </div>
            <div class = "login_box">
               <p class = "idBox"><input class = "inputBox" type="text" name="id" placeholder="학생이름"></p>
               <p><input class = "inputBox" type="password" name="password" placeholder="비밀번호"></p>
               <p class = "loginStillBox"><input type="checkbox" id="stillLogin"><label for="stillLogin"><span class = "loginOption">로그인 상태 유지</span></label></p>
            </div>
            <div class = "submitBtn">
                <img src="../assets/submit.png" width="16%">
            </div>
            <div class = "helpDiv">
                <p class = "loginHelp">계정 생성</p>
                <p class = "loginHelp">로그인이 안 되시나요?<span class = "version">V0.1</span></p>
            </div>          
        </div>
        <div class = "image_grid">
            <div class = "div_image">
                <img src="../assets/model.png" width="45%">
            </div>
        </div>
    </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@500&display=swap');

body {
    margin: 0;
    padding: 0;
}

html {
    font-size:62.5%;
}

#grid {
    display: grid;
    grid-template-columns: 40% 60%;
    height:100vh;
}

.slock {
    color:white;
    font-size: 7.2rem;
    font-family: 'Roboto', sans-serif;
    letter-spacing: 0.4rem;
    margin-bottom:-4%;
}

.infoSlock {
    color:white;
    font-size:2.1rem;
    font-weight: 300;
    font-family: 'Noto Sans KR', sans-serif;
}

.login_grid {
    padding-top : 5.2%;
    padding-left:12%;
    background-color : #292929;
}

.image_grid {
    background-image : url('../assets/image_grid.png');
}

.div_image {
    text-align: center;
    padding-top:20%;
}

.login_box {
    padding-top:3%;
    padding-bottom:5%;
}

.idBox{
    padding-bottom:2%;
}

.loginStillBox {
    padding-top:5%;
}

.loginOption {
    color:white;
    font-size:2rem;
    font-family: 'Noto Sans KR', sans-serif;
    padding-left:3%;
}

.inputBox {
    padding : 3.5%;
    width:50%;
    border-radius: 8px;
    border:none;
    background:#bdbdbd;
}

.inputBox::placeholder{
    font-size:1.5rem;
    color:#777777;
    font-family: 'Noto Sans KR', sans-serif;
}

.submitBtn {
    padding-left:20%;
    padding-top: 10%;
}

.helpDiv {
    padding-top: 10%;
}

.loginHelp {
    color:#777777;
    font-size:1.5rem;
    font-weight: 500;
    font-family: 'Noto Sans KR', sans-serif;
}

.version {
    padding-left:30%;
}

</style>