# Banking-app


#HTML code

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <script src="https://kit.fontawesome.com/79529b3781.js" crossorigin="anonymous"></script>
    <title>Banking Application</title>
</head>
<body>
    <div class="selector-menu">
        <a href="#"><i class="fas fa-university fa-2x" alt="Home"></i></a>
        <a href="#"><i class="fas fa-search-dollar fa-2x" alt="Transactions"></i></a>
        <a href="#" class="current"><i class="fas fa-paper-plane fa-2x" alt="Send Money"></i></a>
        <a href="#"><i class="fas fa-store fa-2x"></i></a>
        <a href="#"><i class="fas fa-mobile-alt fa-2x"></i></a>
      </div>
      <div class="menu-container">
        <div class="header-img">
          <div class="overlay"></div>
          <div class="balance">
            <h1>Balance</h1>
            <div>
              <i class="fas fa-money-bill-alt"></i>
              <p>$35000.49</p>
            </div>
          </div>
        </div>
  
        <ul class="list">
          <li class="item">
            <a href="#">UNO</a>
            <p>$150000.00</p>
          </li>
          <li class="item">
            <a href="#">Sparks trust</a>
            <p>$900.77</p>
          </li>
          <li class="item">
            <a href="#">Covid relief</a>
            <p>$2500.88</p>
          </li>
          <li class="item">
            <a href="#">Childrens relief</a>
            <p>$1400.09</p>
          </li>
        </ul>
      </div>
    </body>
  
</body>
</html>





#CSS CODE:



:root{
    background: rgb(42,171,81);
  background: linear-gradient(90deg, rgba(42,171,81,1) 0%, rgba(5,154,20,1) 65%, rgba(2,56,38,1) 100%);
}
*{
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}

body{
    background: var(--background-color);
    font-family: sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
}

a {
    text-decoration: none;
    outline: none;
}

ul li {
    list-style: none;
    display: flex;
    align-items: center;
    justify-content: space-between;
    cursor: pointer;
}

ul li:hover p{
    transform: scale(1.5);
    opacity: 1;
}
ul li:hover a{
    opacity: 1;
}

i{
    color: #fff;
}

.selector-menu {
    display: flex;
    align-items: center;
    margin-bottom: 25px;
}

.selector-menu a {
    background: rgba(0,0,0,0.3);
    display: flex;
    align-items: center;
    justify-content: center;
    width: 75px;
    height: 60px;
}
.selector-menu a:hover:not(:focus){
    background: rgba(0,0,0,0.6);
}
.selector-menu a:focus {
    transform: scale(1.2);
    background: rgba( 0,0,0, 0.9);
    box-shadow: 0 0 10px 2px rgba(0,0,0,0.6);
}

.menu-container{
    width: 300px;
}

.header-img{
    background:url("https://thefinancialbrand.com/wp-content/uploads/2017/03/regions_bank_branch_tellers-565x377.jpg") no-repeat right/cover;
    height: 150px;
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
    position: relative;
}

.overlay{
    background: rgba(0,0,0,0.2);
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
    position: absolute;
    width: 100%;
    height: 100%;
}

.balance{
    color: #fff;
    position: absolute;
    bottom: 20px;
    left: 20px;
    
}

.balance h1 {
    font-size:1.6rem;
}

.balance div{
    display: flex;
    align-items: center;
    
}

.balance p{
    font-size: 1.2rem;
    font-weight: bold;
    padding:5px;
}

.list a, .list p{
    color: #000;
    opacity: 0.4;;
}
.item {
    background: #fff;
    padding: 20px;
}

.item:not(:last-child){
    border-bottom: 1px solid #dedede;
}
.item:last-child{
    border-bottom-left-radius: 5px ;
    border-bottom-right-radius: 5px;
}

