<template>
    <div id="page-container">
        <!-- <img alt="Vue logo" src="@/assets/logo.png"> -->
        <div class="page">
            <div id="page-1">
                <img class="profile-pic" alt="David Han" src="@/assets/DavidHanProfilePic.png">
                <div class="greeting">Hi! I'm David Han</div>
                <div class="self-proclamation">developer, outdoor enthusiast, beer nerd</div>    
            </div>
            <svg aria-hidden="true" data-prefix="fas" data-icon="chevron-down" class="theres-more" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path fill="currentColor" d="M207.029 381.476L12.686 187.132c-9.373-9.373-9.373-24.569 0-33.941l22.667-22.667c9.357-9.357 24.522-9.375 33.901-.04L224 284.505l154.745-154.021c9.379-9.335 24.544-9.317 33.901.04l22.667 22.667c9.373 9.373 9.373 24.569 0 33.941L240.971 381.476c-9.373 9.372-24.569 9.372-33.942 0z"></path></svg>
        </div>        
    </div>
</template>


<style lang="scss" scoped>

// $padding_value: 30px;
$padding_value: 0px;

#page-container {
    position: relative;
    top: $padding_value;
    left: $padding_value;
    height: unquote("calc(100% - #{$padding_value} - #{$padding_value})");
    width: unquote("calc(100% - #{$padding_value} - #{$padding_value})");
    // padding: $padding_value;
    background-color: #1a1a1a;
    // border-radius: 5px; 

    padding: 0 40px;

    .page {
        position: relative;
        height: 100%;

        #page-1 {
            // padding-top: 50%;
            
            position: relative;
            top: 50%;
            transform: translateY(-50%);

            .profile-pic {
                position: relative;                
                max-width: 60%;
                border-radius: 50%;
            }

            .greeting {
                margin-top: 10px;
                font-size: 36px;
            }

            .self-proclamation {
                margin-top: 10px;
                font-size: 24px;
            }
        }

        .theres-more {
            position: absolute;
            // margin-top:40%;
            bottom: 5%;

            width: 10%;
            background-color: #1a1a1a;
            stroke: #ccc;

            left: 50%;
            transform: translateX(-50%);            
        }
    }
    
}
</style>
