<template>

 <main>
    <div class="logoImage">
        <img src="..\src\assets\gitlogo.png" height=85px; width= 85px;>
    </div>
    <h1 id="heading">Sign in to GitHub</h1>
   
<form class="gitsign" id="form00">
    <div class="userlabel">
        <label id="userlbl">Username or email address</label>
    </div>
    <div class="userinput">
        <input type="email" id="userinpt">
    </div>
    <div class="passwordlabel">
        <label id="passlbl">Password</label>
        <a id="forgotpass" href="#">Forgot password?</a>
    </div>
    <div class="passwordinput">
        <input type="password" id="passinpt">
    </div>
    <div class="signin">
     <button id="signbtn" type="submit">Sign in</button>
    </div>
</form>
      <p class="paragraph">New to GitHub?
             <a href="#">Create an account</a>
      </p>
</main>

</template>>

<style>
::root{
    --base-text-weight-light: 300;
}
 *{ 
    box-sizing: border-box;
    /* font-family: 'Inconsolata', monospace; */
}
main{
    display: grid;
    justify-content: center;
    margin: 150px;
    font-family: -apple-system,BlinkMacSystemFont,"Segoe UI","Noto Sans",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji";
}
#forgotpass{
    /* right: 0; */
    margin-left: 65px;
}
.logoImage{
    display: grid;
    justify-content: inherit;
}

#heading{
    font-size: 24px;
    font-weight: var(--base-text-weight-light, 300);
    letter-spacing: -0.5px;
    display: block;
    font-size: 2em;
    margin-block-start: 0.67em;
    margin-block-end: 0.67em;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
    margin-left: 24px;
}

.userinput{
    margin-top: 4px;
    margin-bottom: 16px;
}

#userinpt,#passinpt{
    display: block;
    width: 100%;

     
}

.passwordlabel{
    --base-text-weight-normal: 400;
    margin-bottom: 4px;
}

.signin{
    margin-top: 16px;
}

#signbtn{
    display: block;
    width: 100%;
    text-align: center;
}

.paragraph{
    padding: 16px 16px;
    text-align: center;
    border-radius: 6px;
    border: 2px solid #d0d7de;
    transition: 0.50s;
}

.gitsign{
    padding: 20px 12px;
    font-size: 14px;
    background-color: #f6f8fa;
    border: 2px solid #d0d7de; ;
    border-top: 6px;
    border-radius: 6px 6px 6px 6px;
}
#userinpt,#passinpt{
  
    font-size: 14px; 
    line-height: 25px; 
    color: var(--color-fg-default);
    vertical-align: middle; 
    background-repeat: no-repeat;
    background-position: right 8px center;
    border: 2px solid #d0d7de;
    border-radius: 6px;
    /* box-shadow: var(--color-primer-shadow-inset); */
    transition: 80ms cubic-bezier(0.33, 1, 0.68, 1);
    /* transition-property: color,background-color,box-shadow,border-color; */
    transition:0.50s
}

#signbtn{
  color: #ffffff;
  background-color:#1f883d;
  border-color: rgba(31,35,40,0.15);;
}
a{
    text-decoration: none;
}

#signbtn{
    position: relative;
    display: inline-block;
    padding: 5px 16px;
    font-size: 14px;
    font-weight: var(--base-text-weight-medium, 500);
    line-height: 20px;
    white-space: nowrap;
    vertical-align: middle;
    cursor: pointer;
    -webkit-user-select: none;
    user-select: none;
    border: 1px solid;
    border-radius: 6px;
    -webkit-appearance: none;
    appearance: none;
    transition: 0.50s;
} 

/* hover affects code below*/
#userinpt:hover,#passinpt:hover{

    background-color: #f8f7f7;
              
}
#signbtn:hover{
   background: #3d6e4c;
}
.paragraph:hover{
    background-color:#f6f8fa ;

}
</style>

<!-- <script>
let form = document.getElementById('form00')
form.addEventListner('submit'),(e)=> {
    let userName = document.getElementById('userinpt').value
    let userPass = document.getElementById('passinpt').value

    //local storage

    localStorage.setItem('userinpt',userName)
    localStorage.setItem('passinpt',userPass)

    alert('Your details are saved in localstorage!')
}
</script> -->