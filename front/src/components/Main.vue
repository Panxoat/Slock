<template>
    <div id = "grid">
        <div class = "login_grid">
            <div>
                <img src="../assets/ico.png" width="10%">
                <p class = "slock">{{msg}}</p>
                <p class = "infoSlock">새로운 기숙사 문관리 시스템</p>
            </div>
            <div class = "login_box">
                <input type="text" class="form__field" placeholder="학생이름" name="name" id='name' required autocomplete="off"/>
                <label for="name" class="form__label">학생이름</label>
            </div>
            <div class="login_box2">
                <input type="password" class="form__field" placeholder="비밀번호" name="password" id='password' required autocomplete="off"/>
                <label for="password" class="form__label">비밀번호</label>
                <p class = "loginStillBox"><input type="checkbox" id="stillLogin"><label for="stillLogin"><span class = "loginOption">로그인 상태 유지</span></label></p>              
            </div>
            <div class = "submitBtn">
                <img class = "default" src = "../assets/submit.png">
                <img class = "defaultHover" src = "../assets/submit_hover.png">
            </div>
            <div class = "helpDiv">
                <span class = "HelpCreate">계정 생성</span><br><br>
                <span class = "HelpWrong">로그인이 안 되시나요?</span><span class = "version">V0.1</span>
            </div>          
        </div>
        <div class = "image_grid">
            <div class = "div_image">
                <img src="../assets/model.png" width="45%">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data () {
        return {
            msg : 'SLOCK.',
        }
    }
}

</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@500&display=swap');

.form__field {
  width: 60%;
  border: 0;
  border-bottom: 2px solid #777777;
  outline: 0;
  font-size: 1.3rem;
  color: white;
  padding: 7px 0;
  background: transparent;
  transition: border-color 0.2s;

  &::placeholder {
    color: transparent;
  }

  &:placeholder-shown ~ .form__label {
    font-size: 1.8rem;
    cursor: text;
    top: 20px;
  }
}

.form__label {
  position: absolute;
  top: 0;
  display: block;
  transition: 0.2s;
  font-size: 1rem;
  color: #777777;
}

.form__field:focus {
  ~ .form__label {
    position: absolute;
    top: 0;
    display: block;
    transition: 0.2s;
    font-size: 1rem;
    color: #777777;
    font-weight:700;    
  }
    padding-bottom: 6px;
    border-bottom: 2px solid #6C63FF;
    font-weight: 700;
    border-width: 3px;
}

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
    position:relative;
    padding: 15px 0 0;
    margin-top: 10px;
    width:100%;
    padding-top: 2%;
    padding-bottom:3%;
}

.login_box2 {
    position:relative;
    padding: 15px 0 0;
    margin-top: 10px;
    width:100%;
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

.submitBtn {
    top:5%;
    margin-left: 22%;
    width:12%;
    height:8%;
    position: relative;
}

.submitBtn img {
    left: -5%;
    top:-15%;
    width:110%;

    position: absolute;
}

.submitBtn > .defaultHover {
    opacity: 0;
    translate: opacity 1s;
}

.submitBtn:hover > .defaultHover {
    opacity: 1;
}

.helpDiv {
    padding-top: 20%;
}

.HelpCreate, .HelpWrong {
    color:#777777;
    font-size:1.5rem;
    font-weight: 500;
    font-family: 'Noto Sans KR', sans-serif;
}

.HelpCreate:hover, .HelpWrong:hover {
    color:white;
    cursor: pointer;
}

.version {
    padding-left:32%;
    color:#777777;
    font-size:1.5rem;
    font-weight: 500;
    font-family: 'Noto Sans KR', sans-serif;
}

</style>