<template>
	<div class="intro">
        <div class="left_column">
            <div class="left_bg"></div>
        </div>
        <div class="right_column">
            <div class="right_bg"></div>
        </div>

        <img class="m_logo" src="/M_logo.png" alt="M_logo">
        <img class="m_logo_circle" src="/M_logo_circle.png" alt="M_logo_circle">
    </div>
</template>

<script>

export default {
  name: 'Intro',
}
</script>

<style>
body, html {
    overflow: hidden;
    animation: 4s disableOverflow forwards;
}

.intro {
    display: block;
    animation: 4s disabledIntro forwards;
}

.intro .m_logo {
    position: absolute;
    bottom: 35%;
    margin-left: auto;
    margin-right: auto;
    left: 0;
    right: 0;
    text-align: center;
    animation: 1.5s animationFirstMLogo forwards;
}

.intro .m_logo_circle {
    position: absolute;
    bottom: 35%;
    margin-left: auto;
    margin-right: auto;
    left: 0;
    right: 0;
    text-align: center;
    animation: 3s animationSecondMLogo forwards;
}

.intro {
    width: 100%;
    height: 100vh;
    display: flex;
}
.intro .left_column,
.intro .right_column {
    width: 50%;
}

.intro .right_column {
    display: flex;
    flex-flow: row-reverse;
}

.intro .left_bg {
    background: #FAFAFA;
    width: 0%;
    height: 100%;
    animation: 1.3s left-animate forwards;
    animation-timing-function: linear;
}
.intro .right_bg {
    background: #000;
    width: 100%;
    height: 100%;
    animation: 1.3s right-animate forwards;
    animation-timing-function: linear;
}

@keyframes left-animate {
  0% {
    width: 0%;
  }
  100% {
    width: 100%;
  }
}
@keyframes right-animate {
  0% {
    width: 0%;
  }
  40% {
    transform: rotateY(90deg);
  }
  100% {
    width: 100%;
  }
}

@keyframes animationFirstMLogo {
    0% {
        display: none;
        opacity: 0;
    }
    100% {
        display: block;
        opacity: 1;
    }
}
@keyframes animationSecondMLogo {
    0% {
        display: none;
        opacity: 0;
    }
    50% {
        display: none;
        opacity: 0;
    }
    100% {
        display: block;
        opacity: 1;
    }
}

@keyframes disabledIntro {
    0% {
        display: flex;
        height: 100vh;
    }
    90% {
        display: flex;
        height: 100vh;
    }
    100% {
        visibility: hidden;
        height: 0px;
    }
}

@keyframes disableOverflow {
    0% {
        overflow: hidden;
    }
    90% {
        overflow: hidden;
    }
    100% {
        overflow: unset;
    }
}
</style>