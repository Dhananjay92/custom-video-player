# Custom Video Player for Android

<h3>Introduction</h3>
<p>Custom Video Player is a library with simple and clean controllers that can be embedded anywhere in Android Applications. It can play single or multiple videos from URLs. Added auto mute, auto play to manage video player. Customized controllers and methods.</p>

<h3>Documentation</h3>
<b>Add to layout</b>

    <com.pavanpathro.custom_video_player.CustomVideoPlayer
        android:id="@+id/customVideoPlayer"
        android:layout_width="match_parent"
        android:layout_height="300dp" />

<b>Initialise Video Player</b>

    CustomVideoPlayer customVideoPlayer = findViewById(R.id.customVideoPlayer);

<b>Single Video</b>

    customVideoPlayer.setMediaUrl("https://www.rmp-streaming.com/media/bbb-360p.mp4");
    
<b>Auto Mute</b> (Default - false)
                       
    customVideoPlayer.enableAutoMute(true);


<b>Auto Play</b> (Default - true)
                       
    customVideoPlayer.enableAutoPlay(false);
    
<b>Set MinHeight</b>
                       
    customVideoPlayer.setMinHeight(300);
    
<b>Set MaxHeight</b> (Default - true)
                       
    customVideoPlayer.setMaxHeight(500);
    
<b>Manage Controllers</b> (Default - false)
                       
    customVideoPlayer.hideControllers(true);
    
    
<b>Example</b>
    
    customVideoPlayer.setMediaUrls(listOfVideos)
        .enableAutoMute(false)
        .enableAutoPlay(false)
        .hideControllers(false)
        .setOnPlaybackListener(this)
        .build();
    
<b>Video Controllers</b>
<br/>

<b>Play</b>
      
    customVideoPlayer.play();

<b>Pause</b>
     
    customVideoPlayer.pause();

<b>Stop</b>
 
    customVideoPlayer.stop();
    
<b>Samples</b>

<div>
    <img src="https://github.com/PavanKumarPatruni/custom-video-player/blob/master/Screen%20Shot%202018-08-17%20at%203.32.24%20AM.png">
</div>

<h3>Author</h3>
<b>Pavan Kumar Patruni (Email - pavanpathro@gmail.com)</b>

