<html lang="en">
<title>W3.CSS Template</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<!-- 外部連結到    -->
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Raleway">
 <!-- 定義格式 圖片大小 字體大小 透明度   -->
<style>
    body,
    h1,
    h2,
    h3,
    h4,
    h5 {
        font-family: "Raleway", sans-serif
    }

    .w3-third img {
        margin-bottom: -6px;
        opacity: 0.8;
        cursor: pointer
    }

    .w3-third img:hover {
        opacity: 1
    }
</style>

<body class="w3-light-grey w3-content" style="max-width:1600px">

    <!-- 定義文字 顏色 大小 位置 -->
    <nav class="w3-sidebar w3-bar-block w3-white w3-animate-left w3-text-grey w3-collapse w3-top w3-center"
        style="z-index:3;width:300px;font-weight:bold" id="mySidebar"><br>
        <h3 class="w3-padding-64 w3-center"><b>SOME<br>NAME</b></h3>
        <!-- 每個項目連結到的位置  id方式做的超連結   -->
        <a href="javascript:void(0)" onclick="w3_close()"
            class="w3-bar-item w3-button w3-padding w3-hide-large">CLOSE</a>
        <a href="#" onclick="w3_close()" class="w3-bar-item w3-button">PORTFOLIO</a>
        <a href="#about" onclick="w3_close()" class="w3-bar-item w3-button">ABOUT ME</a>
        <a href="#contact" onclick="w3_close()" class="w3-bar-item w3-button">CONTACT</a>
    </nav>

    <!-- Top menu on small screens -->
    <header class="w3-container w3-top w3-hide-large w3-white w3-xlarge w3-padding-16">
        <span class="w3-left w3-padding">SOME NAME</span>
        <a href="javascript:void(0)" class="w3-right w3-button w3-white" onclick="w3_open()">☰</a>
    </header>

    <!-- 手機小屏幕上打開可以疊加 -->
    <div class="w3-overlay w3-hide-large w3-animate-opacity" onclick="w3_close()" style="cursor:pointer"
        title="close side menu" id="myOverlay"></div>

    <!-- 整個網頁的元素左邊間距 -->
    <div class="w3-main" style="margin-left:300px">

        <!--小螢幕上下邊界設定間距 -->
        <div class="w3-hide-large" style="margin-top:83px"></div>

        <!--照片連結位置 大小 說明圖片 -->
        <div class="w3-row">
            <div class="w3-third">
                <img src="natureboy.jpeg" style="width:100%" onclick="onClick(this)"
                    alt="A boy surrounded by beautiful nature">
                <img src="girl_mountain.jpeg" style="width:100%" onclick="onClick(this)"
                    alt="What a beautiful scenery this sunset">
                <img src="girl.jpeg" style="width:100%" onclick="onClick(this)" alt="The Beach. Me. Alone. Beautiful">
            </div>
         <!--照片連結位置 大小 說明圖片 -->
            <div class="w3-third">
                <img src="boy.jpeg" style="width:100%" onclick="onClick(this)"
                    alt="Quiet day at the beach. Cold, but beautiful">
                <img src="man_bench.jpeg" style="width:100%" onclick="onClick(this)"
                    alt="Waiting for the bus in the desert">
                <img src="natureboy.jpeg" style="width:100%" onclick="onClick(this)"
                    alt="Nature again.. At its finest!">
            </div>
         <!--照片連結位置 大小 說明圖片 -->
            <div class="w3-third">
                <img src="girl.jpeg" style="width:100%" onclick="onClick(this)" alt="Canoeing again">
                <img src="girl_train.jpeg" style="width:100%" onclick="onClick(this)" alt="A girl, and a train passing">
                <img src="closegirl.jpeg" style="width:100%" onclick="onClick(this)" alt="What a beautiful day!">
            </div>
        </div>

        <!-- 圖片分頁1.2.3.4按鈕 -->
        <div class="w3-center w3-padding-32">
            <div class="w3-bar">
                <a href="#" class="w3-bar-item w3-button w3-hover-black">«</a>
                <a href="#" class="w3-bar-item w3-black w3-button">1</a>
                <a href="#" class="w3-bar-item w3-button w3-hover-black">2</a>
                <a href="#" class="w3-bar-item w3-button w3-hover-black">3</a>
                <a href="#" class="w3-bar-item w3-button w3-hover-black">4</a>
                <a href="#" class="w3-bar-item w3-button w3-hover-black">»</a>
            </div>
        </div>

        <!-- 點選圖片可以放大-->
        <div id="modal01" class="w3-modal w3-black" style="padding-top:0" onclick="this.style.display='none'">
            <span class="w3-button w3-black w3-xlarge w3-display-topright">×</span>
            <div class="w3-modal-content w3-animate-zoom w3-center w3-transparent w3-padding-64">
                <img id="img01" class="w3-image">
                <p id="caption"></p>
            </div>
        </div>

        <!-- 自介的區域 顏色 字 大小 圖片位置 內文 -->
        <div class="w3-container w3-dark-grey w3-center w3-text-light-grey w3-padding-32" id="about">
            <h4><b>About Me</b></h4>
            <img src="avatar_hat.jpeg" alt="Me" class="w3-image w3-padding-32" width="600" height="650">
            <div class="w3-content w3-justify" style="max-width:600px">
                <h4>My Name</h4>
                <p>Some text about me. I love taking photos of PEOPLE. I am lorem ipsum consectetur adipiscing elit, sed
                    do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
                    exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure
                    dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur
                    sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum
                    consectetur adipiscing elit, sed do eiusmod tempor
                    incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation
                    ullamco laboris nisi ut aliquip ex ea commodo consequat.
                </p>
                <p>mail: example@example.com</p>
                <p>tel: 5353 35531</p>
                <hr class="w3-opacity">
                 <!-- 技巧分析 字體透明度 條狀百分比呈現 -->
                <h4 class="w3-padding-16">Technical Skills</h4>
                <p class="w3-wide">Photography</p>
                <div class="w3-white">
                    <div class="w3-container w3-padding-small w3-center w3-grey" style="width:95%">95%</div>
                </div>
                <p class="w3-wide">Web Design</p>
                <div class="w3-white">
                    <div class="w3-container w3-padding-small w3-center w3-grey" style="width:85%">85%</div>
                </div>
                <p class="w3-wide">Photoshop</p>
                <div class="w3-white">
                    <div class="w3-container w3-padding-small w3-center w3-grey" style="width:80%">80%</div>
                </div>
                 <!-- 下載履歷表的按鈕 -->
                <p><button class="w3-button w3-light-grey w3-padding-large w3-margin-top w3-margin-bottom">Download
                        Resume</button></p>
                <hr class="w3-opacity">
                <!-- 定義"個人收費"樣式-->
                <h4 class="w3-padding-16">How much I charge</h4>
                <div class="w3-row-padding" style="margin:0 -16px">
                    <!-- basic表格定義風格 細項內說明 最下面給予一個sign up按鈕-->
                    <div class="w3-half w3-margin-bottom">
                        <ul class="w3-ul w3-white w3-center w3-opacity w3-hover-opacity-off">
                            <li class="w3-black w3-xlarge w3-padding-32">Basic</li>
                            <li class="w3-padding-16">Web Design</li>
                            <li class="w3-padding-16">Photography</li>
                            <li class="w3-padding-16">5GB Storage</li>
                            <li class="w3-padding-16">Mail Support</li>
                            <li class="w3-padding-16">
                                <h2>$ 10</h2>
                                <span class="w3-opacity">per month</span>
                            </li>
                            <li class="w3-light-grey w3-padding-24">
                                <button class="w3-button w3-white w3-padding-large">Sign Up</button>
                            </li>
                        </ul>
                    </div>

                    <!-- pro表格定義風格 細項內說明 最下面給予一個sign up按鈕-->
                    <div class="w3-half">
                        <ul class="w3-ul w3-white w3-center w3-opacity w3-hover-opacity-off">
                            <li class="w3-black w3-xlarge w3-padding-32">Pro</li>
                            <li class="w3-padding-16">Web Design</li>
                            <li class="w3-padding-16">Photography</li>
                            <li class="w3-padding-16">50GB Storage</li>
                            <li class="w3-padding-16">Endless Support</li>
                            <li class="w3-padding-16">
                                <h2>$ 25</h2>
                                <span class="w3-opacity">per month</span>
                            </li>
                            <li class="w3-light-grey w3-padding-24">
                                <button class="w3-button w3-white w3-padding-large">Sign Up</button>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>

        <!--資料輸入表格 name email message   -->
        <!--文字位置 使用新視窗 input元素 -->
        <div class="w3-container w3-light-grey w3-padding-32 w3-padding-large" id="contact">
            <div class="w3-content" style="max-width:600px">
                <h4 class="w3-center"><b>Contact Me</b></h4>
                <p>Do you want me to photograph you? Fill out the form and fill me in with the details :) I love meeting
                    new people!</p>
                <form action="/action_page.php" target="_blank">
                    <div class="w3-section">
                        <label>Name</label>
                        <input class="w3-input w3-border" type="text" name="Name" required>
                    </div>
                    <div class="w3-section">
                        <label>Email</label>
                        <input class="w3-input w3-border" type="text" name="Email" required>
                    </div>
                    <div class="w3-section">
                        <label>Message</label>
                        <input class="w3-input w3-border" type="text" name="Message" required>
                        <!--寄送資料按鈕  -->
                    </div>
                    <button type="submit" class="w3-button w3-block w3-black w3-margin-bottom">Send Message</button>
                </form>
            </div>
        </div>

        <!-- 網頁底風格設置 分三欄 -->
        <footer class="w3-container w3-padding-32 w3-grey">
            <div class="w3-row-padding">
                <div class="w3-third">
                     <!-- 第一欄  info -->
                    <h3>INFO</h3>
                    <p>Praesent tincidunt sed tellus ut rutrum. Sed vitae justo condimentum, porta lectus vitae,
                        ultricies congue gravida diam non fringilla.</p>
                </div>
                     <!-- 第二欄 blog psots 設定圖片位置 右邊間距 大小 -->
                <div class="w3-third">
                    <h3>BLOG POSTS</h3>
                     <!-- 第二項第一個內容設定 -->
                    <ul class="w3-ul">
                        <li class="w3-padding-16 w3-hover-black">
                            <img src="workshop.jpeg" class="w3-left w3-margin-right" style="width:50px">
                            <span class="w3-large">Lorem</span><br>
                            <span>Sed mattis nunc</span>
                        </li>
                         <!-- 第二項第2個內容設定 -->
                        <li class="w3-padding-16 w3-hover-black">
                            <img src="gondol.jpeg" class="w3-left w3-margin-right" style="width:50px">
                            <span class="w3-large">Ipsum</span><br>
                            <span>Praes tinci sed</span>
                        </li>
                    </ul>
                </div>
                 <!-- 第三欄 popular tags設定每一個tag的風格設定-->
                <div class="w3-third">
                    <h3>POPULAR TAGS</h3>
                    <p>
                        <span class="w3-tag w3-black w3-margin-bottom">Travel</span> <span
                            class="w3-tag w3-dark-grey w3-small w3-margin-bottom">New York</span> <span
                            class="w3-tag w3-dark-grey w3-small w3-margin-bottom">London</span>
                        <span class="w3-tag w3-dark-grey w3-small w3-margin-bottom">IKEA</span> <span
                            class="w3-tag w3-dark-grey w3-small w3-margin-bottom">NORWAY</span> <span
                            class="w3-tag w3-dark-grey w3-small w3-margin-bottom">DIY</span>
                        <span class="w3-tag w3-dark-grey w3-small w3-margin-bottom">Ideas</span> <span
                            class="w3-tag w3-dark-grey w3-small w3-margin-bottom">Baby</span> <span
                            class="w3-tag w3-dark-grey w3-small w3-margin-bottom">Family</span>
                        <span class="w3-tag w3-dark-grey w3-small w3-margin-bottom">News</span> <span
                            class="w3-tag w3-dark-grey w3-small w3-margin-bottom">Clothing</span> <span
                            class="w3-tag w3-dark-grey w3-small w3-margin-bottom">Shopping</span>
                        <span class="w3-tag w3-dark-grey w3-small w3-margin-bottom">Sports</span> <span
                            class="w3-tag w3-dark-grey w3-small w3-margin-bottom">Games</span>
                    </p>
                </div>
            </div>
        </footer>

        <div class="w3-black w3-center w3-padding-24">Powered by <a href="https://www.w3schools.com/w3css/default.asp"
                title="W3.CSS" target="_blank" class="w3-hover-opacity">w3.css</a></div>

        <!-- End page content -->
    </div>

      <!--側邊三條可以打開選擇項目  -->
    <script>
        // 打開右邊選單
        function w3_open() {
            document.getElementById("mySidebar").style.display = "block";
            document.getElementById("myOverlay").style.display = "block";
        }

        function w3_close() {
            document.getElementById("mySidebar").style.display = "none";
            document.getElementById("myOverlay").style.display = "none";
        }

        // 圖片
        function onClick(element) {
            document.getElementById("img01").src = element.src;
            document.getElementById("modal01").style.display = "block";
            var captionText = document.getElementById("caption");
            captionText.innerHTML = element.alt;
        }

    </script>


</body>

</html
