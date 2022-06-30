# YouTube-clone-
YouTube clone 
---------------------------------------------------------------------------------
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://kit.fontawesome.com/ff6d44ecaf.js" crossorigin="anonymous"></script>

    <!-- Google font icon -->
    <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">

    <!-- CSS Link -->

 

    <title>Youtube Home Clone!</title>
    <style>
        * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: sans-serif;
    cursor: pointer;
  }
  
  /* Navbar Starts */
  
  i {
    margin: 5px;
    color: #525151;
  }
  a{
    text-decoration: none;
    color: rgb(70, 69, 69);
  }
  
  ::placeholder {
    padding-left: 7px;
  }
  
  .navBar {
    align-items: center;
    margin: 0 10px;
  }
  
  .navBar .navbar_items {
    display: flex;
    margin: 2px 12px;
    justify-content: space-between;
    align-items: center;
  }
  
  .navBar .navbar_item {
    display: flex;
    align-items: center;
  }
  
  .navBar .navbar_item .navBar_logo {
  }
  .navBar .navbar_item .navBar_logo_img {
    margin-left: 40px;
  }
  
  .navBar_search {
    display: flex;
    align-items: center;
  }
  
  .navBar_search .navBar_Search_input {
    padding: 8px 0;
    width: 35rem;
    border: rgb(201, 53, 53) 1px solid;
    border-radius: 2px;
  }
  
  .navBar_search .navBar_search_icon {
    padding: 6px 18px;
    margin-left: -5px;
    border: gray 1px solid;
    border-radius: 2px;
  
    background-color: #dbd8d8;
  }
  
  .navBar_search .navBar_search_mic {
    background-color: #dad8d8;
    padding: 7px;
    border-radius: 50%;
  }
  
  .navBar_icons {
    display: flex;
    align-items: center;
  }
  
  .navBar_icons .navBar_icons_user {
    background-color: #dad8d8;
    padding: 7px;
    border-radius: 50%;
    border-color: darkred;
  }
  
  /* //  Navebar ends
    
    //Sidebar starts */
  
  .core_sidebar {
    height: calc(100vh - 70px);
    display: flex;
    overflow: hidden;
  }
  
  .sidebar {
    width: 70px;
    height: 100%;
    /* background-color: #245323; */
  }
  .sidebar_icons {
    text-align: center;
    margin-top: 4px;
    margin-left: 10px;
  }
  
  .sidebar_icon {
    text-align: center;
    margin-bottom: 10px;
  }
  
  /* //Sidebar Ends */
  
  .core_sidebar2 {
    height: calc(100vh - 70px);
    display: flex;
    overflow: hidden;
  }
  
  .sidebar2 {
    width: 250px;
    height: 100%;
    background-color: #faffff;
    overflow-y: scroll;
  }
  
  .sidebar_icons2 {
    display: flex;
    text-align: left;
    padding: 8px 30px;
  }
  
  .sidebar_icons2:hover {
    background-color: rgb(231, 231, 231);
  }
  
  .sidebar_icon2 a {
    color: gray;
    border-color: crimson;
  }
  
  .sidebar_navbar {
    margin-left: 1rem;
    margin-top: -10px;
    color: rgb(207, 71, 71);
    font-weight: bold;
  }
  
  /* Fullside bar Ends */
  
  /* // Video Suggestions starts */
  
  .videoSuggestions {
    display: flex;
    flex-direction: row;
    width: 100%;
    margin-left: 24px;
    overflow-x: scroll;
  }
  
  .video_suggestion {
    display: flex;
    flex-direction: row;
    align-items: center;
    padding: 30px 0;
    height: 30px;
    /* background-color: rgb(76, 59, 94); */
  }
  
  .video_suggestion_tag {
    text-decoration: none;
    font-size: 14px;
    background-color: #dad8d8;
    color: #242323;
    padding: 8px 20px;
    margin: 0 5px;
    border-radius: 20px;
  }
  
  .video_suggestion_tag:hover{
    background-color: #807d7d;
    color: black;
  }
  
  .hr_line {
    margin-left: 6rem;
  }
  
  /* Video Listing */
  
  .videos_list {
    width: 90%;
    height: 90%;
    margin-top: 70px;
    padding: 25px 15px;
    overflow-y: scroll;
    position: fixed;
    clear: both;
    margin-left: 100px;
    background-color: rgb(245, 241, 241);
  }
  
  .videos {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    flex-wrap: wrap;
  }
  
  .single_video {
    width: 320px;
    margin-right: 5px;
    margin-bottom: 30px;
  }
  
  .video_thumbnail {
    width: 310px;
    height: 170px;
  }
  
  .video_thumbnail iframe {
    object-fit: cover;
    height: 100%;
    width: 100%;
  }
  
  .video_time {
    color: white;
    background-color: black;
    padding: 2px 5px;
    float: right;
    z-index: 1;
    /* margin-top: -20px; */
  }
  .video_details {
    display: flex;
    margin-top: 5px;
  }
  .video_details .channel_img img {
    width: 40px;
    border-radius: 50%;
    margin-left: -5px;
  }
  
  .video_title {
    display: flex;
    flex-direction: column;
    margin-left: 10px;
  }
  
  .video_title h4 {
    font-size: 14px;
    color: rgb(43, 42, 42);
    /* line-height: 20px; */
  }
  
  .video_details,
  h4,
  span,
  p {
    text-decoration: none;
    color: #525151;
    font-size: 14px;
    /* margin-left: 5px; */
  }
  
  @media only screen and (max-width: 600px) {
    #search_desktop {
      display: none;
    }
  }
    </style>

</head>

<body>
    <!-- Navbar Starts -->

    <div class="navBar">
        <div class="navbar_items">
            <div class="navbar_item">
                <div class="navBar_home">
                    <a href="#" id="btn" onclick="toggleHide()"><i class="material-icons">
                            menu</i></a>
                </div>
                <div class="navBar_logo">
                    <a href="https://www.youtube.com/"><img src="../public/images/gif/YTLogo.gif" alt="youtube logo"
                            class="navBar_logo_img" style="width: 120px; "></a>
                            
            </div>

            <div class="navBar_search" id="search_desktop">
                <div>
                    <input type="text" name="" value="" placeholder="Search" class="navBar_Search_input">
                </div>

                <div>
                    <a href="#"><i class="material-icons  navBar_search_icon" style="font-size: 20px;">
                            search
                        </i></a>

                </div>
                <div>
                    <a href="#"><i class="material-icons navBar_search_mic">
                            mic
                        </i></a>
                </div>
            </div>

            <div class="navBar_icons">

                <div>
                    <a href="../08_New Video Upload/Video_Upload_part1.html"><i class="material-icons">
                            file_upload
                        </i></a>
                </div>

                <div>
                    <a href="../13_Studio/Studio.html"><i class="material-icons">
                            apps
                        </i></a>
                </div>

                <div>
                    <a href="#"><i class="material-icons">
                            notifications
                        </i></a>
                </div>

                <div>
                    <a href="../03_Login page/01_google_Login_Page.html"><img src="../public/images/webdevelopment.jpg" alt="user logo"
                            title="Sign in" width="40px"></a>
                </div>
            </div>
        </div>
    </div>
    <hr class="hr_line">
    <!-- Navbar ends -->

    <!-- Sidebar Starts -->
    <div class="core_sidebar">
        <div class="sidebar" id="sidebar">

            <div class="sidebar_icons">
                <div style="color: red;" class="sidebar_icon">
                    <a href="#"><i class="material-icons" style="color: red;">
                            home
                        </i></a>
                    <p style="font-size: 12px;"><a href="./index.html">Home</a></p>
                </div>
                <div class="sidebar_icon">
                    <a href="../09_explore/explore.html"><i class="material-icons">
                            explore
                        </i></a>
                    <p style="font-size: 12px;">Explore</p>
                </div>

                <div class="sidebar_icon">
                    <a href="../05_Single video/singleVideoPage.html"><i class="material-icons">
                            subscriptions
                        </i></a>
                    <p style="font-size: 12px;">Subscriptions</p>
                </div>

                <div class="sidebar_icon">
                    <a href="../01_Home page/index.html"><i class="material-icons">
                            video_library
                        </i></a>
                    <p style="font-size: 12px;">Library</p>
                </div>
            </div>
        </div>

        <!-- Sidebar Ends -->


        <!-- ON CLICK SIDEBAR STARTS -->

        <!-- Sidebar Starts -->
        <div class="core_sidebar2" id="full_Sidebar" style="display: none; width: 70px;">
            <div class="sidebar2">

                <div class="sidebar_icons2" style=" padding-top: 15px;background-color: rgb(231, 231, 231);">

                    <!-- Icon1 -->

                    <div style="color: red;" class="sidebar_icon2">
                        <a href="#"><i class="material-icons" style="color: red;">
                                home
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Home</p>
                    </div>

                </div>

                <!-- icon2 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                explore
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Explore</p>
                    </div>

                </div>

                <!-- icon2 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                subscriptions
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Subscriptions</p>
                    </div>

                </div>

                <hr>
                <!-- icon3 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                video_library

                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Library</p>
                    </div>

                </div>


                <!-- icon4 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                history
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>History</p>
                    </div>

                </div>

                <!-- icon5 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                watch_later
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Watch later</p>
                    </div>

                </div>

                <!-- icon6 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                thumb_up
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Likes</p>
                    </div>

                </div>
                <hr>

                <!-- icon7 -->
                <p style="color: gray; margin-left: 8px;"><strong>MORE FROM YOUTUBE</strong></p>
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                play_circle_filled
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>YouTube Video Premium</p>
                    </div>

                </div>

                <!-- icon8 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                theaters
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Movies</p>
                    </div>
                </div>
                <hr>

                <!-- icon9 -->
                <p style="color: gray; margin-left: 8px;"><strong>FUN & LEARN TOGETHER</strong></p>

                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                sports_esports
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Gaming</p>
                    </div>

                </div>

                <!-- icon10 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                online_prediction
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Live</p>
                    </div>

                </div>

                <!-- icon11 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                emoji_objects
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Learning</p>
                    </div>

                </div>


                <!-- icon12 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                emoji_events
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Sports</p>
                    </div>

                </div>
                <hr>

                <!-- icon13 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                settings
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Settings</p>
                    </div>

                </div>

                <!-- icon14 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                assistant_photo
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Report history</p>
                    </div>

                </div>

                <!-- icon15 -->
                <div class="sidebar_icons2">
                    <div class="sidebar_icon2">
                        <a href="#"><i class="material-icons">
                                contact_support
                            </i></a>
                    </div>
                    <div class="sidebar_nav">
                        <p>Help</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- ON CLICK SIDEBAR Ends -->

        <!-- Video Suggestions starts -->
        <div class="videoSuggestions">

            <div class="video_suggestion">
                <a href="../01_Home page/index.html" class="video_suggestion_tag"
                    style="color: white; background-color: black;">all</a>
            </div>

            <div class="video_suggestion">
                <a href="../04_Single page-home/singlePage-home.html" class="video_suggestion_tag">Learn</a>
            </div>

            <div class="video_suggestion">
                <a href="../06_Music/singlePage-home.html" class="video_suggestion_tag">Music</a>
            </div>
            <div class="video_suggestion">
                <a href="../11_manas Mishra/manas.html" class="video_suggestion_tag">REACT.JS</a>
            </div>

            <div class="video_suggestion">
                <a href="../07_Comedy/singlePage-home.html" class="video_suggestion_tag">Comedy</a>
            </div>

            <div class="video_suggestion">
                <a href="../05_Single video/singleVideoPage.html" class="video_suggestion_tag">FOOD</a>
            </div>

            <div class="video_suggestion">
                <a href="../12_Sandeep Maheshwari/motivation.html" class="video_suggestion_tag">AWS</a>
            </div>

            <div class="video_suggestion">
                <a href="../04_Single page-home/singlePage-home.html" class="video_suggestion_tag">HTML</a>
            </div>

            <div class="video_suggestion">
                <a href="../04_Single page-home/" class="video_suggestion_tag">JavaScript</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">Java</a>
            </div>

            <div class="video_suggestion">
                <a href="../04_Single page-home/singlePage-home.html" class="video_suggestion_tag">Coding</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">python</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">coding</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">Songs</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">Sass</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">scss</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">Css</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">C#</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">CSS</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">HTML</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">JavaScript</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">Java</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">Coding</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">python</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">pPowerBI</a>
            </div>

            <div class="video_suggestion">
                <a href="#" class="video_suggestion_tag">C#</a>
            </div>
        </div>
        <!-- Video Suggestions Ends -->

        <!-- Video List Starts -->

        <div class="videos_list">
            <div class="videos">
                <!-- Video1 -->
                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/DHvZLI7Db8E"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">6:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="channel logo">
                        </div>
                        <div class="video_title">
                            <h4>How The The System Works in Backend</h4>
                            <p>JavaScript Masterych <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>771,000 views. 2 mothes Ago</p>
                        </div>
                    </div>

                </div>
                <!-- Video 2 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="120px" height="auto" src="https://www.youtube.com/embed/4r6WdaY3SOA"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">11:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="channel logo">
                        </div>
                        <div class="video_title">
                            <h4>How The The System Works in Backend</h4>
                            <p>JavaScript Masterych <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>895,000 views. 11 mothes Ago</p>
                        </div>
                    </div>

                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/zSt-KI0HryY"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">11:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Ways to add Java Script to Web Pages?</h4>
                            <p>Apna College<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>17,446 views. Jul 6, 2021</p>
                        </div>
                    </div>

                </div>

                <!-- Video3 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/HkWxvB1RJq0"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">8:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Higher-Order Functions ft. Functional Programming | Namaste JavaScript</h4>
                            <p>Namaste JavaScript <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>6,546,695 views. 8 mothes Ago</p>
                        </div>
                    </div>

                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/VY6MZGPKR5c"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">12:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>What is Django Capable of? | Companies That Use It</h4>
                            <p>freeCodeCamp.org <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>182,852 views. Mar 3, 2020</p>
                        </div>
                    </div>

                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/9exK6rLAR7g"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">50:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>ReactJS Interview Questions and Answers | ReactJS Tutorial</h4>
                            <p>edureka!<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>2,560 viewsJul 21, 2021</p>
                        </div>
                    </div>

                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/PkZNo7MFNFg"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">12:43</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Learn JavaScript - Full Course for Beginners</h4>
                            <p>freeCodeCamp.org <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>6,766,695 views. Dec 10, 2018</p>
                        </div>
                    </div>

                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/zSt-KI0HryY"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">11:02</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Biggest Enemy of our Success - How to overcome Fear of losing ?</h4>
                            <p>Apna College<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>48,691 views. Aug 7, 2021</p>
                        </div>
                    </div>

                </div>


                <!-- Video5 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/j59qQ7YWLxw"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Build A Calculator With JavaScript Tutorial</h4>
                            <p>Namaste JavaScript <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>561,535 views. Apr 16, 2019</p>
                        </div>
                    </div>

                </div>

                <!-- Video 6 -->
                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/TAP5B_XlVa0"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="./Images/code with harry.png" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Should you use Bootstrap & Tailwind CSS or stick to Vanilla CSS?
                            </h4>
                            <p>CodeWithHarry <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>34,971 viewsJul 25, 2021</p>
                        </div>
                    </div>

                </div>


                <!-- Video 7 -->
                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/6mbwJ2xhgzM"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="./Images/code with harry.png" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Introduction to HTML, CSS, JavaScript & How websites work? |
                            </h4>
                            <p>CodeWithHarry <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>1,823,062 views. Dec 25, 2019</p>
                        </div>
                    </div>

                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/n0kikYKo3nA"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">11:02</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Biggest Enemy of our Success - How to overcome Fear of losing ?</h4>
                            <p>Apna College<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>48,691 views. Aug 7, 2021</p>
                        </div>
                    </div>

                </div>

                <!-- Video8 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/BNC6slYCj50"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>let & const in JS 🔥Temporal Dead Zone | | Namaste JavaScript</h4>
                            <p>Namaste JavaScript <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>87,722 views. Nov 5, 2020</p>
                        </div>
                    </div>

                </div>

                <!-- Video9 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/j59qQ7YWLxw"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Build A Calculator With JavaScript Tutorial</h4>
                            <p>Namaste JavaScript <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>561,535 views. Apr 16, 2019</p>
                        </div>
                    </div>

                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/RBSGKlAvoiM"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="./Images/edureka.png" alt="">
                        </div>
                        <div class="video_title">
                            <h4>CloudOps vs DevOps : Which One Should You Use | What Is CloudOps</h4>
                            <p>edureka!<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>2,434 views. Streamed live on Aug 9, 2021</p>
                        </div>
                    </div>

                </div>

                <!-- Video10 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/eBTBG4nda2A"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>setTimeout + Closures Interview Question 🔥 | Namaste 🙏 JavaScript </h4>
                            <p>Namaste JavaScript <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>100,839 viewsDec 7, 2020</p>
                        </div>
                    </div>
                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/2lRQTdpwhFk"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">03:02</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>How JavaScript Works ?</h4>
                            <p>Apna College<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>37,174 views. Jun 24, 2021</p>
                        </div>
                    </div>

                </div>


                <!-- Video 2 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/ngc9gnGgUdA"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">11:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="./Images/JavaScript Masterych.png" alt="channel logo">
                        </div>
                        <div class="video_title">
                            <h4>Full Stack MERN Project - Build and Deploy an App | React + Redux, Node, Express,
                                MongoDB </h4>
                            <p>JavaScript Masterych <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>468,619 views. Oct 30, 2020</p>
                        </div>
                    </div>

                </div>

                <!-- Video3 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/iLWTnMzWtj4"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>How JavaScript Code is executed? ❤️& Call Stack | Namaste JavaScript</h4>
                            <p>Namaste JavaScript <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>160,109 views. Oct 20, 2020</p>
                        </div>
                    </div>

                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/RBSGKlAvoiM"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Data Structures Easy to Advanced Course - Full Tutorial from a Google Engineer</h4>
                            <p>freeCodeCamp.org <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>3,200,055 views. Sep 19, 2019</p>
                        </div>
                    </div>

                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/RBSGKlAvoiM"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="./Images/edureka.png" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Django Vs Flask | Django Vs Flask: Which is better for your Web Application?</h4>
                            <p>edureka!<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>113,537 views. Premiered Feb 7, 2020</p>
                        </div>
                    </div>

                </div>

                <!-- Video5 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/SHINoHxvTso"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>FIRST CLASS FUNCTIONS 🔥ft. Anonymous Functions | Namaste JavaScript <p>Namaste
                                    JavaScript<span class="material-icons">
                                        check_circle
                                    </span></p>
                                <p>64,555 views. Dec 15, 2020</p>
                        </div>
                    </div>

                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/cnT1oW5_ePM"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">03:02</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>2.1 Data Types & Type Modifiers | Data Structures & Algorithms Course in C++</h4>
                            <p>Apna College<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>707,306 views. Oct 10, 2020</p>
                        </div>
                    </div>

                </div>

                <!-- Video5 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/btj35dh3_U8"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Callback Functions in JS ft. Event Listeners 🔥| Namaste JavaScript</h4>
                            <p>Namaste JavaScript<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>82,140 views. Dec 20, 2020</p>
                        </div>
                    </div>

                </div>

                <!-- Video5 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/btj35dh3_U8"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Callback Functions in JS ft. Event Listeners 🔥| Namaste JavaScript</h4>
                            <p>Namaste JavaScript<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>82,140 views. Dec 20, 2020</p>
                        </div>
                    </div>

                </div>


                <!-- Video 6 -->
                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/DYdVXqXhWyw"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="./Images/code with harry.png" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Use this Frontend Backend combination to become a successful Web Developer!
                            </h4>
                            <p>CodeWithHarry <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>189,850 views. May 24, 2021</p>
                        </div>
                    </div>
                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/DJckAUyEwR0"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">06:43</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>QnA : Coding ke beginners doubt | Aapne coding kahan se seekhi ?</h4>
                            <p>Apna College<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>94,915 views. Aug 5, 2021</p>
                        </div>
                    </div>

                </div>
                <!-- Video5 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/zdp0zrpKzIE"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>map, filter & reduce 🙏 Namaste JavaScript Ep. 19 🔥</h4>
                            <p>Namaste JavaScript<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>68,672 views. Jul 21, 2021</p>
                        </div>
                    </div>

                </div>

                <!-- Video 6 -->
                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/DYdVXqXhWyw"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="./Images/code with harry.png" alt="">
                        </div>
                        <div class="video_title">
                            <h4>What does a Software engineer do in a Company? 🔥🔥
                            </h4>
                            <p>CodeWithHarry <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>262,409 views. Aug 2, 2021</p>
                        </div>
                    </div>
                </div>

                <!-- Video1 -->
                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/377AQ0y6LPA"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="channel logo">
                        </div>
                        <div class="video_title">
                            <h4>ECommerce Web Shop - Build & Deploy an Amazing App | React.js, Commerce.js, Stripe</h4>
                            <p>JavaScript Masterych <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>384,162 views. Nov 28, 2020</p>
                        </div>
                    </div>
                </div>

                <!-- Video1 -->
                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/LYWgPSbPDfQ"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="channel logo">
                        </div>
                        <div class="video_title">
                            <h4>Full Stack MERN Project - Build and Deploy an App | React + Redux, Node, Express,
                                MongoDB</h4>
                            <p>JavaScript Masterych <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>69,758 views. May 16, 2021</p>
                        </div>
                    </div>
                </div>



                <!-- Video1 -->
                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/g7T23Xzys-A"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="channel logo">
                        </div>
                        <div class="video_title">
                            <h4>JavaScript Crash Course - Learn JavaScript in 2021</h4>
                            <p>JavaScript Masterych <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>43,115 views. Jan 1, 2021</p>
                        </div>
                    </div>
                </div>


                <!-- Video5 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/8zKuNo4ay8E"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Asynchronous JavaScript & EVENT LOOP from scratch 🔥 | Namaste JavaScript </h4>
                            <p>Namaste JavaScript<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>123,070 views. Dec 27, 2020</p>
                        </div>
                    </div>

                </div>

                <!-- Video 6 -->
                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/W7kSd1nSrJI"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="./Images/code with harry.png" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Single Page Applications: Why & When to use React/Angular/Vue.js?
                            </h4>
                            <p>CodeWithHarry <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>163,025 views. May 9, 2021</p>
                        </div>
                    </div>
                </div>

                <!-- Video4 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/tLKKmouUams"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>FastAPI Course for Beginners</h4>
                            <p>freeCodeCamp.org <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>11,556 viewsAug 12, 2021</p>
                        </div>
                    </div>

                </div>

                <!-- Video5 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/eBTBG4nda2A"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>setTimeout + Closures Interview Question 🔥 | Namaste 🙏 JavaScript </h4>
                            <p>Namaste JavaScript<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>100,924 views. Dec 7, 2020</p>
                        </div>
                    </div>

                </div>

                <!-- Video 6 -->
                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/tnJBalPzeAo"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="./Images/code with harry.png" alt="">
                        </div>
                        <div class="video_title">
                            <h4>How deploy a Django application using Nginx & Gunicorn in Production
                            </h4>
                            <p>CodeWithHarry <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>15,133 views. Jun 6, 2021</p>
                        </div>
                    </div>
                </div>

                 <!-- Video5 -->

                 <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/btj35dh3_U8"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Callback Functions in JS ft. Event Listeners 🔥| Namaste JavaScript</h4>
                            <p>Namaste JavaScript<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>82,140 views. Dec 20, 2020</p>
                        </div>
                    </div>

                </div>


                <!-- Video5 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/Fnlnw8uY6jo"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Hoisting in JavaScript 🔥(variables & functions) | Namaste JavaScript </h4>
                            <p>Namaste JavaScript<span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>147,037 views. Oct 21, 2020</p>
                        </div>
                    </div>
                </div>

                <!-- Video10 -->

                <div class="single_video">

                    <div class="video_thumbnail">
                        <div><iframe width="560" height="315" src="https://www.youtube.com/embed/qikxEIxsXco"
                                title="YouTube video player" frameborder="0"
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                                allowfullscreen></iframe></div>
                        <p class="video_time">2:34</p>
                    </div>

                    <div class="video_details">
                        <div class="channel_img">
                            <img src="../public/images/webdevelopment.jpg" alt="">
                        </div>
                        <div class="video_title">
                            <h4>Closures in JS 🔥 | Namaste JavaScript</h4>
                            <p>Namaste JavaScript <span class="material-icons">
                                    check_circle
                                </span></p>
                            <p>112,825 views. Dec 1, 2020</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Video List Ends -->
    </div>
<script src="../public/script/yt clone.js"></script>
</body>
</html>
------------------------------------------------------------------------------------------------------
function toggleHide() {
    let button = document.getElementById('btn');
    let fullNavbar = document.getElementById('full_Sidebar');
    let sidebar = document.getElementById('sidebar');
    if (sidebar.style.display != 'none') {
        sidebar.style.display = 'none';
        fullNavbar.style.display = 'block'
    } else {
        fullNavbar.style.display = 'none';
        sidebar.style.display = 'block';
    }

}
